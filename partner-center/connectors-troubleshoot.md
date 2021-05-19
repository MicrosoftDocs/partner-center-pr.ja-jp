---
title: 共同販売紹介コネクタのトラブルシューティング
ms.topic: how-to
ms.date: 09/21/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 共同販売コネクタの使用に関する一般的な質問への回答について学習します。 共同販売コネクタのトラブルシューティング方法については、この FAQ を参照してください。
author: sroy
ms.author: sroy
ms.localizationpriority: medium
ms.openlocfilehash: 49a2b6e5461dacbe87c34b36805a5c240c2e5fd1
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/19/2021
ms.locfileid: "110148348"
---
# <a name="troubleshoot-co-sell-referrals-connectors"></a><span data-ttu-id="e1da6-104">共同販売紹介コネクタのトラブルシューティング</span><span class="sxs-lookup"><span data-stu-id="e1da6-104">Troubleshoot co-sell referrals connectors</span></span>

<span data-ttu-id="e1da6-105">**適用対象**: Dynamics 365 CRM |Salesforce CRM</span><span class="sxs-lookup"><span data-stu-id="e1da6-105">**Applies to**: Dynamics 365 CRM | Salesforce CRM</span></span>

<span data-ttu-id="e1da6-106">**適切なロール**: 紹介管理者|CRM のシステム管理者またはシステム カスタマイザー</span><span class="sxs-lookup"><span data-stu-id="e1da6-106">**Appropriate roles**: Referrals admin | System admin or system customizer on the CRM</span></span>

 ## <a name="questions-and-answers-about-pre-requisites"></a><span data-ttu-id="e1da6-107">前提条件に関する質問と回答</span><span class="sxs-lookup"><span data-stu-id="e1da6-107">Questions and answers about pre-requisites</span></span>

1. <span data-ttu-id="e1da6-108">環境に対して試用版の共同販売紹介コネクタ ソリューションを使用できますか?</span><span class="sxs-lookup"><span data-stu-id="e1da6-108">Can you use a trial co-sell referrals connectors solution for your environment?</span></span>

<span data-ttu-id="e1da6-109">テスト/ステージング環境を使用している場合は、試用版ソリューションを選択できます。</span><span class="sxs-lookup"><span data-stu-id="e1da6-109">If you are on the test/staging environment, you can opt for trial solution.</span></span> <span data-ttu-id="e1da6-110">コネクタの有料版は、AppSource で 1 か月あたり 15 米国ドルで利用できます。</span><span class="sxs-lookup"><span data-stu-id="e1da6-110">The paid version of the Connectors is available in AppSource at US$ 15/month.</span></span> <span data-ttu-id="e1da6-111">有料接続では、1 日あたり 10,000 回の API 呼び出しが行われます。</span><span class="sxs-lookup"><span data-stu-id="e1da6-111">With the paid connection, you will be getting 10K API calls per day.</span></span> <span data-ttu-id="e1da6-112">コネクタは、参照 API の上パートナー センターラッパーです。</span><span class="sxs-lookup"><span data-stu-id="e1da6-112">The Connectors are wrappers on top of Partner Center referral APIs.</span></span> <span data-ttu-id="e1da6-113">コネクタ ソリューションが パートナー センター 側または CRM 側の案件で Create または **Update** イベントに対して実行されるたびに、API 呼び出しが行されます。</span><span class="sxs-lookup"><span data-stu-id="e1da6-113">Whenever the connector solutions run for a **Create** or **Update** event on the opportunities on either Partner Center or the CRM side, an API call is made.</span></span>

2. <span data-ttu-id="e1da6-114">CRM 環境でセクションを作成するには、どのようなロールが必要ですか?</span><span class="sxs-lookup"><span data-stu-id="e1da6-114">What role do you need to create sections in CRM environment?</span></span>

<span data-ttu-id="e1da6-115">システム管理者またはシステム カスタマイザーであるユーザーは、すべてのユーザーに変更を適用できます。</span><span class="sxs-lookup"><span data-stu-id="e1da6-115">Users who are system admins or system customizers can apply changes for everyone.</span></span> <span data-ttu-id="e1da6-116">ただし、すべてのアプリ ユーザーは、システムをカスタマイズし、カスタマイズの一部を他のユーザーと共有することもできます。</span><span class="sxs-lookup"><span data-stu-id="e1da6-116">All app users, however,  can personalize the system and even share some of their customizations with others.</span></span> 

3. <span data-ttu-id="e1da6-117">パートナーの販売者は、パートナーがビジネスに取り組む上で特別なパートナー センター?</span><span class="sxs-lookup"><span data-stu-id="e1da6-117">Do partner sellers need special roles to work on Partner Center?</span></span>
 
<span data-ttu-id="e1da6-118">パートナー販売者には、"紹介管理者" ロールが割り当てられている必要があります。</span><span class="sxs-lookup"><span data-stu-id="e1da6-118">Partner sellers must be assigned the “Referrals admin” role.</span></span> <span data-ttu-id="e1da6-119">詳細については、「アクセス許可の概要 [」を参照してください](create-user-accounts-and-set-permissions.md)。</span><span class="sxs-lookup"><span data-stu-id="e1da6-119">For more information, see [Permissions overview](create-user-accounts-and-set-permissions.md).</span></span>

4. <span data-ttu-id="e1da6-120">CRM 環境で最初に設定する必要があるフィールドは何ですか?</span><span class="sxs-lookup"><span data-stu-id="e1da6-120">What fields need to be set up first in your CRM environment?</span></span> 

<span data-ttu-id="e1da6-121">• 通貨が自分の場所に適し、CRM 環境に正確に含けられているか確認します。</span><span class="sxs-lookup"><span data-stu-id="e1da6-121">• Make sure your currency is appropriate to your location and is in your CRM environment accurately.</span></span> <span data-ttu-id="e1da6-122">• 販売チームは CRM ユーザーとして CRM 環境に表示される必要があります。</span><span class="sxs-lookup"><span data-stu-id="e1da6-122">• Your sales team should be listed in your CRM environment as CRM users.</span></span>

5. <span data-ttu-id="e1da6-123">環境の作成を自動化するために必要な前提条件は何ですか。</span><span class="sxs-lookup"><span data-stu-id="e1da6-123">What pre-requisites are required for Power Automate environment creation?</span></span>

<span data-ttu-id="e1da6-124">電力自動化環境を使用するには、次のものが必要です。</span><span class="sxs-lookup"><span data-stu-id="e1da6-124">To use the Power Automate environment, you need:</span></span>

- <span data-ttu-id="e1da6-125">Power 自動ライセンス認証が必要です。</span><span class="sxs-lookup"><span data-stu-id="e1da6-125">A Power Automate license is required.</span></span>
- <span data-ttu-id="e1da6-126">少なくとも 1 GB のストレージが必要です。</span><span class="sxs-lookup"><span data-stu-id="e1da6-126">A minimum of 1-GB storage is required.</span></span>

6.  <span data-ttu-id="e1da6-127">Salesforce コネクタソリューションを使用するには、Dynamics 365 サブスクリプションが必要ですか?</span><span class="sxs-lookup"><span data-stu-id="e1da6-127">Do you need a Dynamics 365 subscription to use Salesforce Connectors solution?</span></span>

<span data-ttu-id="e1da6-128">Salesforce コネクタソリューションの種類は "Dynamics Flow" で、他の CRM システムとの同期をサポートしています。</span><span class="sxs-lookup"><span data-stu-id="e1da6-128">The Salesforce Connector solution is of type “Dynamics Flow” that supports synchronizing with other CRM systems.</span></span> <span data-ttu-id="e1da6-129">このソリューションでは、Dynamics 365 インスタンスまたはサブスクリプションが必要ではありません。</span><span class="sxs-lookup"><span data-stu-id="e1da6-129">The solution doesn’t require you to have a Dynamics 365 instance or a subscription.</span></span> <span data-ttu-id="e1da6-130">Salesforce ソリューションをインストールするときに、会社内の既存の CD 環境を含むドロップダウンが表示されることがあります。</span><span class="sxs-lookup"><span data-stu-id="e1da6-130">While installing the Salesforce solution, a drop-down with existing CDS environment in your company may appear.</span></span> <span data-ttu-id="e1da6-131">その環境を選択する必要があります。</span><span class="sxs-lookup"><span data-stu-id="e1da6-131">You need to select that environment.</span></span> <span data-ttu-id="e1da6-132">さらに、"サインインしたユーザーに接続された Dynamics 365 組織が見つかりませんでした" というエラーが表示された場合は、コネクタ用に新しい環境を作成する必要があります。</span><span class="sxs-lookup"><span data-stu-id="e1da6-132">In addition, if you get the error "We couldn't find a Dynamics 365 organization connected to signed-in user", then you will need to create new environment for connector.</span></span>

## <a name="questions-and-answers-about-configuration"></a><span data-ttu-id="e1da6-133">構成に関する質問と回答</span><span class="sxs-lookup"><span data-stu-id="e1da6-133">Questions and answers about configuration</span></span>

1. <span data-ttu-id="e1da6-134">パワー自動化プラットフォームでフローをアクティブ化しているときに、次のエラーが発生した場合はどうすればよいですか?</span><span class="sxs-lookup"><span data-stu-id="e1da6-134">What should you do if you face the following error while activating flows in Power Automate Platform?</span></span>

<span data-ttu-id="e1da6-135">エラー: Azure Resource Manager への要求が失敗しました。エラー: ' {"エラー": {"code": "WorkflowTriggerNotFound"、"message": "ワークフロー ' e14d00f1-1fdf-4b1b-aaac-54a5064093d3 ' トリガー ' manual ' が見つかりませんでした。"}} '。</span><span class="sxs-lookup"><span data-stu-id="e1da6-135">Error: Request to Azure Resource Manager failed with error: '{"error":{"code":"WorkflowTriggerNotFound","message":"The workflow 'e14d00f1-1fdf-4b1b-aaac-54a5064093d3' trigger 'manual' could not be found."}}'.</span></span> 

<span data-ttu-id="e1da6-136">次のトラブルシューティング手順に従います。</span><span class="sxs-lookup"><span data-stu-id="e1da6-136">Follow these troubleshooting steps:</span></span>

- <span data-ttu-id="e1da6-137">CD 接続を削除してから、CD 接続を再作成してください。</span><span class="sxs-lookup"><span data-stu-id="e1da6-137">Delete the CDS connection and then recreate the CDS connections.</span></span>
- <span data-ttu-id="e1da6-138">子フローをオフまたはオンにする</span><span class="sxs-lookup"><span data-stu-id="e1da6-138">Turn the child flow off and on</span></span> 
- <span data-ttu-id="e1da6-139">ソリューションを削除してから、ソリューションを再インストールしてください。</span><span class="sxs-lookup"><span data-stu-id="e1da6-139">Delete solution and then reinstall the solution.</span></span> 

2.  <span data-ttu-id="e1da6-140">Power オートメーションプラットフォームでパートナーセンターコネクタを追加するときに "サインイン" エラーが発生した場合はどうすればよいですか?</span><span class="sxs-lookup"><span data-stu-id="e1da6-140">What should you do if you face the "Sign in" error while adding a Partner Center connector in Power Automate Platform?</span></span>

:::image type="content" source="images/cosellconnectors/failure.png" alt-text="サインインが必要なエラーメッセージ":::

<span data-ttu-id="e1da6-142">このトラブルシューティングの手順に従います。</span><span class="sxs-lookup"><span data-stu-id="e1da6-142">Follow this troubleshooting step:</span></span>

- <span data-ttu-id="e1da6-143">資格情報をパートナー センター使用して、フロー環境に 1 回サインインします (flow.microsoft.com)。</span><span class="sxs-lookup"><span data-stu-id="e1da6-143">Use your Partner Center credentials to sign into the flow environment once (flow.microsoft.com).</span></span>


3. <span data-ttu-id="e1da6-144">パートナー センター Platform で CRM へのアクセス フローをアクティブ化中に次のエラーが発生した場合Power Automateしてください。</span><span class="sxs-lookup"><span data-stu-id="e1da6-144">What should you do if you receive the following error while activating the Partner Center to CRM flow in Power Automate Platform?</span></span>
 
:::image type="content" source="images/cosellconnectors/powererror.png" alt-text="更新が必要なエラー メッセージ":::

<span data-ttu-id="e1da6-146">次のトラブルシューティング手順に従います。</span><span class="sxs-lookup"><span data-stu-id="e1da6-146">Follow these troubleshooting steps:</span></span>

- <span data-ttu-id="e1da6-147">CRM フローへの接続をアクティブ化する前に、最初に次の 2 パートナー センターをアクティブ化します。</span><span class="sxs-lookup"><span data-stu-id="e1da6-147">Activate the following two child flows first before you activate the Partner Center to CRM flow.</span></span>
      - <span data-ttu-id="e1da6-148">パートナー センター CRM へのアクセス - ヘルパー (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="e1da6-148">Partner Center to CRM - Helper (Insider Preview)</span></span>
      - <span data-ttu-id="e1da6-149">パートナー センター Crm への Microsoft 共同販売紹介の更新プログラムの作成 (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="e1da6-149">Partner Center Microsoft Co-sell Referral Updates to CRM (Insider Preview)</span></span>

4. <span data-ttu-id="e1da6-150">フローを編集しようとするときにフローに接続を追加できない場合は、何をする必要がありますか?</span><span class="sxs-lookup"><span data-stu-id="e1da6-150">What should you do when you aren't able to add connections to the flow when you try to edit the flow?</span></span>

<span data-ttu-id="e1da6-151">フローの実行中にフローへの接続を追加し、各フローに個別に追加します。</span><span class="sxs-lookup"><span data-stu-id="e1da6-151">You add connections to the flow while the flow is running, and you add to each flow separately.</span></span>  <span data-ttu-id="e1da6-152">フローの編集中に接続を追加するダイアログが自動的に開かない場合は、フローの各ステップとサブステップを個別に編集できます。</span><span class="sxs-lookup"><span data-stu-id="e1da6-152">If the dialog to add connections doesn't open up automatically while editing the flow, then you can edit each of the steps and sub steps of the flows individually.</span></span>

- <span data-ttu-id="e1da6-153">各フローを選択し、個別に編集します。</span><span class="sxs-lookup"><span data-stu-id="e1da6-153">Select each flow and edit them individually.</span></span>
- <span data-ttu-id="e1da6-154">フロー内のすべてのステップを展開する</span><span class="sxs-lookup"><span data-stu-id="e1da6-154">Expand all the steps in the flow</span></span> 

:::image type="content" source="images/cosellconnectors/flowsteps.png" alt-text="接続が必要な手順":::

- <span data-ttu-id="e1da6-156">接続の関連付けを求める警告アイコンが表示される手順を選択し、接続を追加します。</span><span class="sxs-lookup"><span data-stu-id="e1da6-156">Select the steps where you see a warning icon asking to associate connections, and add connections.</span></span> 

:::image type="content" source="images/cosellconnectors/editflow.png" alt-text="フローをステップ バイ ステップで編集する":::


5. <span data-ttu-id="e1da6-158">共同販売紹介コネクタ ソリューションのフローが有効にならない場合は、どうする必要がありますか?</span><span class="sxs-lookup"><span data-stu-id="e1da6-158">What should you do if the flows of the Co-sell Referrals Connectors solution don’t turn on?</span></span>

<span data-ttu-id="e1da6-159">A.</span><span class="sxs-lookup"><span data-stu-id="e1da6-159">A.</span></span> <span data-ttu-id="e1da6-160">このPower Automate、次の順序でフローを編集し、正しい接続を使用するために更新する必要があります。</span><span class="sxs-lookup"><span data-stu-id="e1da6-160">In Power Automate, you'll need to edit flows in the following order and update them to use the correct connections:</span></span>

- <span data-ttu-id="e1da6-161">パートナー センター Webhook 登録 (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="e1da6-161">Partner Center Webhook Registration (Insider Preview)</span></span>
- <span data-ttu-id="e1da6-162">共同販売の紹介を作成する - Salesforce パートナー センター (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="e1da6-162">Create Co-sell Referral - Salesforce to Partner Center (Insider Preview)</span></span>
- <span data-ttu-id="e1da6-163">パートナー センターに Microsoft 共同販売紹介の更新プログラムを追加する (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="e1da6-163">Partner Center Microsoft Co-sell Referral Updates to Salesforce (Insider Preview)</span></span>
- <span data-ttu-id="e1da6-164">パートナーセンターから Salesforce へ (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="e1da6-164">Partner Center to Salesforce (Insider Preview)</span></span>
- <span data-ttu-id="e1da6-165">Salesforce からパートナーセンターへ (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="e1da6-165">Salesforce to Partner Center (Insider Preview)</span></span>
- <span data-ttu-id="e1da6-166">パートナーセンターへの Salesforce の営業案件 (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="e1da6-166">Salesforce Opportunity to Partner Center (Insider Preview)</span></span>
- <span data-ttu-id="e1da6-167">パートナーセンターへの Salesforce Microsoft ソリューション (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="e1da6-167">Salesforce Microsoft Solutions to Partner Center (Insider Preview)</span></span>

 <span data-ttu-id="e1da6-168">B.</span><span class="sxs-lookup"><span data-stu-id="e1da6-168">B.</span></span> <span data-ttu-id="e1da6-169">各フローに対して、[ **ユーザーのみ実行** ] オプションを選択します。</span><span class="sxs-lookup"><span data-stu-id="e1da6-169">For each of flow, select **Run only users** option.</span></span> <span data-ttu-id="e1da6-170">[**実行専用ユーザーによって提供される** のではなく、**接続を使用する**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="e1da6-170">Select **Use connection** instead of **Provided by run-only user**.</span></span>  

:::image type="content" source="images/cosellconnectors/runonly.png" alt-text="フローをアクティブ化するには":::


<span data-ttu-id="e1da6-172">C.</span><span class="sxs-lookup"><span data-stu-id="e1da6-172">C.</span></span> <span data-ttu-id="e1da6-173">以下のフローフローをアクティブにします。</span><span class="sxs-lookup"><span data-stu-id="e1da6-173">Activate these below mentioned flows:</span></span>

 - <span data-ttu-id="e1da6-174">パートナーセンター: Microsoft 共同での Salesforce の参照の更新 (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="e1da6-174">Partner Center Microsoft Co-sell Referral Updates to Salesforce (Insider Preview)</span></span>

- <span data-ttu-id="e1da6-175">Salesforce からパートナーセンターへ (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="e1da6-175">Salesforce to Partner Center (Insider Preview)</span></span>

    
<span data-ttu-id="e1da6-176">D.</span><span class="sxs-lookup"><span data-stu-id="e1da6-176">D.</span></span> <span data-ttu-id="e1da6-177">残りのすべてのフローをアクティブ化します。</span><span class="sxs-lookup"><span data-stu-id="e1da6-177">Activate all the remaining flows.</span></span>

<span data-ttu-id="e1da6-178">E.</span><span class="sxs-lookup"><span data-stu-id="e1da6-178">E.</span></span> <span data-ttu-id="e1da6-179">Flow パートナーセンターの Webhook 登録で、[ **実行**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="e1da6-179">At flow Partner Center Webhook Registration, select **Run**.</span></span> <span data-ttu-id="e1da6-180">**パートナーセンター** の最初のアクションから Salesforce flow に **http url** を指定します。</span><span class="sxs-lookup"><span data-stu-id="e1da6-180">Provide the **http url** from the first action in **Partner Center to Salesforce** flow.</span></span> <span data-ttu-id="e1da6-181">[ **登録するイベント** ] の下にある4つのオプションをすべて選択し、[上書き] で [ **はい]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="e1da6-181">Select all four options under **Events to register** and select **yes** for Overwrite.</span></span>

## <a name="questions-and-answers-about-runmaintenance"></a><span data-ttu-id="e1da6-182">実行/メンテナンスに関する質問と回答</span><span class="sxs-lookup"><span data-stu-id="e1da6-182">Questions and answers about Run/Maintenance</span></span>

1. <span data-ttu-id="e1da6-183">省電力のフロー実行中に発生したエラーをトラブルシューティングするにはどうすればよいですか。</span><span class="sxs-lookup"><span data-stu-id="e1da6-183">How do you troubleshoot failures during Power Automate flow execution?</span></span>

<span data-ttu-id="e1da6-184">フローが期待どおりに実行されるようにし、実行中のエラーをトラブルシューティングするには、 [フローエラーの修正](/power-automate/fix-flow-failures)に関する記述を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e1da6-184">To ensure that your Power Automate flows run as you expect and to troubleshoot failures during execution, refer to [Fix flow failures](/power-automate/fix-flow-failures).</span></span>

2. <span data-ttu-id="e1da6-185">パートナーセンターまたは CRM 環境で適切に同期されていない参照が表示される場合は、どうすればよいですか。</span><span class="sxs-lookup"><span data-stu-id="e1da6-185">What should you do if you see referrals that aren't synchronized properly in Partner Center or CRM environment?</span></span>
 
<span data-ttu-id="e1da6-186">参照同期の状態を確認するには、[ **監査**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="e1da6-186">To determine the status of referral synchronization, select **Audit**.</span></span> 

:::image type="content" source="images/cosellconnectors/synch.png" alt-text="参照を同期する方法":::

<span data-ttu-id="e1da6-188">次の条件が満たされている必要があります。</span><span class="sxs-lookup"><span data-stu-id="e1da6-188">Ensure that the following conditions are met:</span></span>

- <span data-ttu-id="e1da6-189">ソリューション ID は、営業案件の一部として提供されます。</span><span class="sxs-lookup"><span data-stu-id="e1da6-189">Solution ID is provided as part of the opportunity.</span></span>

- <span data-ttu-id="e1da6-190">2 文字の国コードが必要です。</span><span class="sxs-lookup"><span data-stu-id="e1da6-190">Two letter country code is required.</span></span>

- <span data-ttu-id="e1da6-191">営業案件に対して Microsoft のヘルプが選択されている場合は、顧客の連絡先情報が必要です。</span><span class="sxs-lookup"><span data-stu-id="e1da6-191">When help from Microsoft is selected for the opportunity, customer contact information is required.</span></span>

3. <span data-ttu-id="e1da6-192">紹介が双方向に同期されるのを確認する方法</span><span class="sxs-lookup"><span data-stu-id="e1da6-192">How to ensure that a referral will synchronize bi-directionally?</span></span>

<span data-ttu-id="e1da6-193">手順は次のとおりです。</span><span class="sxs-lookup"><span data-stu-id="e1da6-193">Do the following steps:</span></span>

- <span data-ttu-id="e1da6-194">パートナー販売者は、CRM セクションで [同期と同期] **パートナー センター有効に** している必要があります。</span><span class="sxs-lookup"><span data-stu-id="e1da6-194">Partner sellers need to ensure that they have enabled **Sync with Partner Center** option in the CRM section.</span></span>

:::image type="content" source="images/cosellconnectors/enablesynch.png" alt-text="Synch を有効にした":::

- <span data-ttu-id="e1da6-196">販売者は、リードを修飾するときに収益と終了日を提供する必要があります。</span><span class="sxs-lookup"><span data-stu-id="e1da6-196">Sellers need to provide revenue and closing date when qualifying a lead.</span></span>

- <span data-ttu-id="e1da6-197">CRM ID が共同販売機会の作成または更新ステージで提供されているが、その ID を持つリード 営業案件が CRM に見つからない場合、更新または作成は無視されます。</span><span class="sxs-lookup"><span data-stu-id="e1da6-197">If CRM ID is provided in the **create** or **update** stage of co-sell opportunity, but a lead opportunity with that ID is not found in CRM, then update or create will be ignored.</span></span>

- <span data-ttu-id="e1da6-198">Salesforce 環境で紹介通貨フィールドが構成されていることを確認します。</span><span class="sxs-lookup"><span data-stu-id="e1da6-198">Ensure that referral currency field is configured on Salesforce environment.</span></span> 

4. <span data-ttu-id="e1da6-199">コネクタが切断され、紹介の同期が失敗した場合は、どうする必要がありますか?</span><span class="sxs-lookup"><span data-stu-id="e1da6-199">What should you do if the connector gets disconnected and you miss a referral synchronization.?</span></span>

<span data-ttu-id="e1da6-200">試しに使用できるオプションの一部を次に示します。</span><span class="sxs-lookup"><span data-stu-id="e1da6-200">Following are few of the options that you can try out:</span></span>

- <span data-ttu-id="e1da6-201">紹介管理者ロールを持つユーザーに対して、ユーザー名またはパスワードパートナー センター有効期限が切れているかどうかを確認します。</span><span class="sxs-lookup"><span data-stu-id="e1da6-201">Check whether username or password has expired for the Partner Center user with referral admin roles.</span></span>

- <span data-ttu-id="e1da6-202">同期されていない営業案件に移動し、軽微な更新を行い、紹介が同期されているかどうかを確認できます。</span><span class="sxs-lookup"><span data-stu-id="e1da6-202">You can go to the un-synchronized opportunity, make a minor update, and observe whether the referral has synchronized.</span></span>

- <span data-ttu-id="e1da6-203">フローが実行され、失敗した場合は、フローを選択し、失敗した実行を再送信します。</span><span class="sxs-lookup"><span data-stu-id="e1da6-203">If the flows have run and failed, then select the flow and re-submit the run that has failed.</span></span>

5. <span data-ttu-id="e1da6-204">アクセス拒否エラーが発生した場合は、何をする必要がありますか?</span><span class="sxs-lookup"><span data-stu-id="e1da6-204">What should you do when you get access denied errors?</span></span>

<span data-ttu-id="e1da6-205">適切なロールが存在する</span><span class="sxs-lookup"><span data-stu-id="e1da6-205">Make sure the appropriate roles exist</span></span>

- <span data-ttu-id="e1da6-206">販売者の紹介管理者パートナー センターロール</span><span class="sxs-lookup"><span data-stu-id="e1da6-206">Referral Administrator role for Partner Center seller</span></span> 
 
- <span data-ttu-id="e1da6-207">CRM インスタンスのシステム管理者またはシステム カスタマイザー ロール</span><span class="sxs-lookup"><span data-stu-id="e1da6-207">System Administrator or System Customizer role on your CRM instance</span></span>

- <span data-ttu-id="e1da6-208">フロー アカウントのユーザー Power Automate少なくとも 1 回事前 https://flow.microsoft.com にログインしてください</span><span class="sxs-lookup"><span data-stu-id="e1da6-208">Ensure that the Power Automate flow account user logs into https://flow.microsoft.com at least once beforehand</span></span>

6. <span data-ttu-id="e1da6-209">共同販売の機会の作成中に **顧客アカウントの国コード** が不足していることがわかった場合は、どうすればよいでしょうか。</span><span class="sxs-lookup"><span data-stu-id="e1da6-209">If you see that **Customer account country code** is missing while creating a Co-sell opportunity, what should you do?</span></span>

<span data-ttu-id="e1da6-210">ISO の2文字の国コードを CRM の顧客アカウントに追加する必要があります。</span><span class="sxs-lookup"><span data-stu-id="e1da6-210">You will need to add the ISO two-letter country code to the Customer account in CRM.</span></span>

7. <span data-ttu-id="e1da6-211">共同販売の機会を作成するときに **ソリューション ID が必要** であるというエラーが表示された場合はどうすればよいですか。</span><span class="sxs-lookup"><span data-stu-id="e1da6-211">What should you do if you see the error that **Solution ID is required** while creating a Co-sell opportunity?</span></span>

<span data-ttu-id="e1da6-212">共同販売の紹介を作成するには、Microsoft 共同販売の準備ができているソリューションが必要です。</span><span class="sxs-lookup"><span data-stu-id="e1da6-212">In order to create a co-sell referral, you need a Microsoft co-sell ready solution.</span></span> 

8. <span data-ttu-id="e1da6-213">フローエラーが発生していなくても CRM に同期されていない共同販売機会がパートナーセンターで作成されている場合はどうすればよいですか。</span><span class="sxs-lookup"><span data-stu-id="e1da6-213">What should you do when you see Co-sell opportunities created in Partner Center that aren't synchronized to CRM even though there are no flow errors?</span></span>

<span data-ttu-id="e1da6-214">次の手順で行います。</span><span class="sxs-lookup"><span data-stu-id="e1da6-214">Do the following:</span></span>

- <span data-ttu-id="e1da6-215">パートナーセンターで新しい共同販売取引を作成した後、パートナーセンターから Dynamics 365 へのフローが呼び出されるかどうかを確認します (複数回呼び出される可能性があります)。</span><span class="sxs-lookup"><span data-stu-id="e1da6-215">After you have created a new co-sell deal in Partner Center, check if Partner Center to Dynamics 365 flow gets invoked (it might get invoked multiple times).</span></span>

- <span data-ttu-id="e1da6-216">フローが呼び出された場合は、呼び出されたすべてのフローを確認し、CRM を更新するフロー実行を特定します。</span><span class="sxs-lookup"><span data-stu-id="e1da6-216">If the flow gets invoked, check all invoked flows, and identify the flow run which that would update the CRM.</span></span> <span data-ttu-id="e1da6-217">アクションに従って操作を実行し、CRM が更新されたか、または問題が発生したかどうかを確認できます。</span><span class="sxs-lookup"><span data-stu-id="e1da6-217">You can follow the actions and verify if it did update the CRM or encountered a problem.</span></span>

- <span data-ttu-id="e1da6-218">パートナーセンターで **新しい取引** を確認し、CRM ID が設定されているかどうかを確認します。</span><span class="sxs-lookup"><span data-stu-id="e1da6-218">Check **New deal** in Partner Center to see if it gets populated with CRM ID.</span></span>

- <span data-ttu-id="e1da6-219">パートナー **センターで取引** が誤って閉じられていないことを **確認します**。</span><span class="sxs-lookup"><span data-stu-id="e1da6-219">Make sure that the deal is not accidentally closed as **Won** or **Lost** in Partner Center.</span></span>

## <a name="next-steps"></a><span data-ttu-id="e1da6-220">次のステップ</span><span class="sxs-lookup"><span data-stu-id="e1da6-220">Next steps</span></span>

- [<span data-ttu-id="e1da6-221">見込み客を管理する</span><span class="sxs-lookup"><span data-stu-id="e1da6-221">Manage leads</span></span>](manage-leads.md)
 
- [<span data-ttu-id="e1da6-222">共同販売の機会を管理する</span><span class="sxs-lookup"><span data-stu-id="e1da6-222">Manage co-sell opportunities</span></span>](manage-co-sell-opportunities.md)
