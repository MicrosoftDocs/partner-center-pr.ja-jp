---
title: 共同販売紹介コネクタのトラブルシューティング
ms.topic: how-to
ms.date: 09/21/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 共同販売コネクタのトラブルシューティング方法に関する FAQ。
author: sroy
ms.author: sroy
ms.localizationpriority: medium
ms.openlocfilehash: ad09d7c805ce5a1138d7546fd041ae1eda77b00c
ms.sourcegitcommit: 51e3c912eba8cfa72733206c0fee22386fbc34aa
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/22/2020
ms.locfileid: "91002971"
---
# <a name="troubleshoot-co-sell-referrals-connectors"></a><span data-ttu-id="6aadc-103">共同販売紹介コネクタのトラブルシューティング</span><span class="sxs-lookup"><span data-stu-id="6aadc-103">Troubleshoot co-sell referrals connectors</span></span>

<span data-ttu-id="6aadc-104">**適用対象:**</span><span class="sxs-lookup"><span data-stu-id="6aadc-104">**Applies to:**</span></span>

- <span data-ttu-id="6aadc-105">パートナー センター</span><span class="sxs-lookup"><span data-stu-id="6aadc-105">Partner Center</span></span>
- <span data-ttu-id="6aadc-106">Dynamics 365 CRM</span><span class="sxs-lookup"><span data-stu-id="6aadc-106">Dynamics 365 CRM</span></span>
- <span data-ttu-id="6aadc-107">Salesforce CRM</span><span class="sxs-lookup"><span data-stu-id="6aadc-107">Salesforce CRM</span></span>

<span data-ttu-id="6aadc-108">**適切なロール**</span><span class="sxs-lookup"><span data-stu-id="6aadc-108">**Appropriate roles**</span></span>

- <span data-ttu-id="6aadc-109">紹介管理者</span><span class="sxs-lookup"><span data-stu-id="6aadc-109">Referrals admin</span></span>
- <span data-ttu-id="6aadc-110">CRM のシステム管理者またはシステムカスタマイザー</span><span class="sxs-lookup"><span data-stu-id="6aadc-110">System admin or system customizer on the CRM</span></span>

 ## <a name="questions-and-answers-about-pre-requisites"></a><span data-ttu-id="6aadc-111">前提条件に関する質問と回答</span><span class="sxs-lookup"><span data-stu-id="6aadc-111">Questions and answers about pre-requisites</span></span>

1. <span data-ttu-id="6aadc-112">お使いの環境に対して試用版の共同販売紹介コネクタソリューションを使用できますか。</span><span class="sxs-lookup"><span data-stu-id="6aadc-112">Can you use a trial co-sell referrals connectors solution for your environment?</span></span>

<span data-ttu-id="6aadc-113">テスト/ステージング環境を使用している場合は、試用版ソリューションを選択できます。</span><span class="sxs-lookup"><span data-stu-id="6aadc-113">If you are on the test/staging environment, you can opt for trial solution.</span></span> <span data-ttu-id="6aadc-114">このコネクタの有料バージョンは、AppSource で米国ドルの 15/月でご利用いただけます。</span><span class="sxs-lookup"><span data-stu-id="6aadc-114">The paid version of the Connectors is available in AppSource at US$ 15/month.</span></span> <span data-ttu-id="6aadc-115">有料接続では、1日あたり10K の API 呼び出しを取得します。</span><span class="sxs-lookup"><span data-stu-id="6aadc-115">With the paid connection, you will be getting 10K API calls per day.</span></span> <span data-ttu-id="6aadc-116">コネクタは、パートナーセンターの参照 Api の上にあるラッパーです。</span><span class="sxs-lookup"><span data-stu-id="6aadc-116">The Connectors are wrappers on top of Partner Center referral APIs.</span></span> <span data-ttu-id="6aadc-117">パートナーセンターまたは CRM 側の営業案件で、コネクタソリューションが **作成** または **更新** イベントに対して実行されるたびに、API 呼び出しが行われます。</span><span class="sxs-lookup"><span data-stu-id="6aadc-117">Whenever the connector solutions run for a **Create** or **Update** event on the opportunities on either Partner Center or the CRM side, an API call is made.</span></span>

2. <span data-ttu-id="6aadc-118">CRM 環境でセクションを作成するにはどのような役割が必要ですか。</span><span class="sxs-lookup"><span data-stu-id="6aadc-118">What role do you need to create sections in CRM environment?</span></span>

<span data-ttu-id="6aadc-119">システム管理者またはシステムカスタマイザーのユーザーは、すべてのユーザーに変更を適用できます。</span><span class="sxs-lookup"><span data-stu-id="6aadc-119">Users who are system admins or system customizers can apply changes for everyone.</span></span> <span data-ttu-id="6aadc-120">ただし、すべてのアプリユーザーがシステムをカスタマイズしたり、カスタマイズの一部を他のユーザーと共有したりすることもできます。</span><span class="sxs-lookup"><span data-stu-id="6aadc-120">All app users, however,  can personalize the system and even share some of their customizations with others.</span></span> 

3. <span data-ttu-id="6aadc-121">パートナー販売者は、パートナーセンターで作業するために特別な役割を必要としていますか。</span><span class="sxs-lookup"><span data-stu-id="6aadc-121">Do partner sellers need special roles to work on Partner Center?</span></span>
 
<span data-ttu-id="6aadc-122">パートナーの販売元には、"紹介管理者" ロールが割り当てられている必要があります。</span><span class="sxs-lookup"><span data-stu-id="6aadc-122">Partner sellers must be assigned the “Referrals admin” role.</span></span> <span data-ttu-id="6aadc-123">詳細については、次の「アクセス許可の概要」を参照してください (作成-ユーザーアカウントと-設定-アクセス許可)。</span><span class="sxs-lookup"><span data-stu-id="6aadc-123">For more information, refer to the following [Permissions overview)(create-user-accounts-and-set-permissions).</span></span>

4. <span data-ttu-id="6aadc-124">CRM 環境で最初に設定する必要があるフィールドは何ですか。</span><span class="sxs-lookup"><span data-stu-id="6aadc-124">What are the fields that need to be set-up first in your CRM environment?</span></span> 

<span data-ttu-id="6aadc-125">•お客様の地域に合った通貨を使用していること、および CRM 環境に正確に対応していることを確認してください。</span><span class="sxs-lookup"><span data-stu-id="6aadc-125">• Make sure your currency is appropriate to your location and is in your CRM environment accurately.</span></span> <span data-ttu-id="6aadc-126">• Crm ユーザーとして CRM 環境に販売チームが一覧表示されている必要があります。</span><span class="sxs-lookup"><span data-stu-id="6aadc-126">• Your sales team should be listed in your CRM environment as CRM users.</span></span>

5.  <span data-ttu-id="6aadc-127">環境の作成を自動化するために必要な前提条件は何ですか。</span><span class="sxs-lookup"><span data-stu-id="6aadc-127">What pre-requisites are required for Power Automate environment creation?</span></span>

<span data-ttu-id="6aadc-128">電力自動化環境を使用するには、次のものが必要です。</span><span class="sxs-lookup"><span data-stu-id="6aadc-128">To use the Power Automate environment, you need:</span></span>

- <span data-ttu-id="6aadc-129">Power 自動ライセンス認証が必要です。</span><span class="sxs-lookup"><span data-stu-id="6aadc-129">A Power Automate license is required.</span></span>
- <span data-ttu-id="6aadc-130">少なくとも 1 GB のストレージが必要です。</span><span class="sxs-lookup"><span data-stu-id="6aadc-130">A minimum of 1-GB storage is required.</span></span>

6.  <span data-ttu-id="6aadc-131">Salesforce コネクタソリューションを使用するには、Dynamics 365 サブスクリプションが必要ですか?</span><span class="sxs-lookup"><span data-stu-id="6aadc-131">Do you need a Dynamics 365 subscription to use Salesforce Connectors solution?</span></span>

<span data-ttu-id="6aadc-132">Salesforce コネクタソリューションの種類は "Dynamics Flow" で、他の CRM システムとの同期をサポートしています。</span><span class="sxs-lookup"><span data-stu-id="6aadc-132">The Salesforce Connector solution is of type “Dynamics Flow” that supports synchronizing with other CRM systems.</span></span> <span data-ttu-id="6aadc-133">このソリューションでは、Dynamics 365 インスタンスまたはサブスクリプションが必要ではありません。</span><span class="sxs-lookup"><span data-stu-id="6aadc-133">The solution doesn’t require you to have a Dynamics 365 instance or a subscription.</span></span> <span data-ttu-id="6aadc-134">Salesforce ソリューションをインストールするときに、会社内の既存の CD 環境を含むドロップダウンが表示されることがあります。</span><span class="sxs-lookup"><span data-stu-id="6aadc-134">While installing the Salesforce solution, a drop-down with existing CDS environment in your company may appear.</span></span> <span data-ttu-id="6aadc-135">その環境を選択する必要があります。</span><span class="sxs-lookup"><span data-stu-id="6aadc-135">You need to select that environment.</span></span> <span data-ttu-id="6aadc-136">さらに、"サインインしたユーザーに接続された Dynamics 365 組織が見つかりませんでした" というエラーが表示された場合は、コネクタ用に新しい環境を作成する必要があります。</span><span class="sxs-lookup"><span data-stu-id="6aadc-136">In addition, if you get the error we couldn't find a Dynamics 365 organization connected to signed-in user", then you will need to create new environment for connector.</span></span>

## <a name="questions-and-answers-about-configuration"></a><span data-ttu-id="6aadc-137">構成に関する質問と回答</span><span class="sxs-lookup"><span data-stu-id="6aadc-137">Questions and answers about configuration</span></span>

1. <span data-ttu-id="6aadc-138">パワー自動化プラットフォームでフローをアクティブ化しているときに、次のエラーが発生した場合はどうすればよいですか?</span><span class="sxs-lookup"><span data-stu-id="6aadc-138">What should you do if you face the following error while activating flows in Power Automate Platform?</span></span>

<span data-ttu-id="6aadc-139">エラー: Azure Resource Manager への要求が失敗しました。エラー: ' {"エラー": {"code": "WorkflowTriggerNotFound"、"message": "ワークフロー ' e14d00f1-1fdf-4b1b-aaac-54a5064093d3 ' トリガー ' manual ' が見つかりませんでした。"}} '。</span><span class="sxs-lookup"><span data-stu-id="6aadc-139">Error: Request to Azure Resource Manager failed with error: '{"error":{"code":"WorkflowTriggerNotFound","message":"The workflow 'e14d00f1-1fdf-4b1b-aaac-54a5064093d3' trigger 'manual' could not be found."}}'.</span></span> 

<span data-ttu-id="6aadc-140">次のトラブルシューティング手順に従います。</span><span class="sxs-lookup"><span data-stu-id="6aadc-140">Follow these troubleshooting steps:</span></span>

- <span data-ttu-id="6aadc-141">CD 接続を削除してから、CD 接続を再作成してください。</span><span class="sxs-lookup"><span data-stu-id="6aadc-141">Delete the CDS connection and then recreate the CDS connections.</span></span>
- <span data-ttu-id="6aadc-142">子フローをオフまたはオンにする</span><span class="sxs-lookup"><span data-stu-id="6aadc-142">Turn the child flow off and on</span></span> 
- <span data-ttu-id="6aadc-143">ソリューションを削除してから、ソリューションを再インストールしてください。</span><span class="sxs-lookup"><span data-stu-id="6aadc-143">Delete solution and then reinstall the solution.</span></span> 

2.  <span data-ttu-id="6aadc-144">Power オートメーションプラットフォームでパートナーセンターコネクタを追加するときに、次のエラーが発生した場合はどうすればよいですか。</span><span class="sxs-lookup"><span data-stu-id="6aadc-144">What should you do if you face the following error while adding a Partner Center connector in Power Automate Platform?</span></span>

:::image type="content" source="images/cosellconnectors/failure.png" alt-text="サインインが必要なエラーメッセージ":::

<span data-ttu-id="6aadc-146">このトラブルシューティングの手順に従います。</span><span class="sxs-lookup"><span data-stu-id="6aadc-146">Follow this troubleshooting step:</span></span>

- <span data-ttu-id="6aadc-147">パートナーセンターのサインインを使用して、フロー環境に1回サインインします (flow.microsoft.com)。</span><span class="sxs-lookup"><span data-stu-id="6aadc-147">Use the Partner Center sign-in to sign into the flow environment once (flow.microsoft.com).</span></span>


3. <span data-ttu-id="6aadc-148">Power オートメーションプラットフォームでパートナーセンターから CRM へのフローをアクティブにするときに、次のエラーが発生した場合はどうすればよいですか?</span><span class="sxs-lookup"><span data-stu-id="6aadc-148">What should you do if you receive the following error while activating the Partner Center to CRM flow in Power Automate Platform?</span></span>
 
:::image type="content" source="images/cosellconnectors/powererror.png" alt-text="更新が必要なエラーメッセージ":::

<span data-ttu-id="6aadc-150">次のトラブルシューティング手順に従います。</span><span class="sxs-lookup"><span data-stu-id="6aadc-150">Follow these troubleshooting steps:</span></span>

- <span data-ttu-id="6aadc-151">パートナーセンターを CRM フローにアクティブ化する前に、まず次の2つの子フローをアクティブ化します。</span><span class="sxs-lookup"><span data-stu-id="6aadc-151">Activate the following two child flows first before you activate the Partner Center to CRM flow.</span></span>
      - <span data-ttu-id="6aadc-152">パートナーセンターから CRM ヘルパーへ (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="6aadc-152">Partner Center to CRM - Helper (Insider Preview)</span></span>
      - <span data-ttu-id="6aadc-153">パートナーセンターの Microsoft 共同販売の CRM の参照の更新 (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="6aadc-153">Partner Center Microsoft Co-sell Referral Updates to CRM (Insider Preview)</span></span>

4. <span data-ttu-id="6aadc-154">フローを編集しようとすると、フローに接続を追加できない場合はどうすればよいですか。</span><span class="sxs-lookup"><span data-stu-id="6aadc-154">What should you do when you aren't able to add connections to the flow when you try to edit the flow?</span></span>

<span data-ttu-id="6aadc-155">フローの実行中にフローへの接続を追加し、各フローに個別に追加します。</span><span class="sxs-lookup"><span data-stu-id="6aadc-155">You add connections to the flow while the flow is running and you add to each flow separately.</span></span>  <span data-ttu-id="6aadc-156">フローの編集中に接続を追加するダイアログボックスが自動的に開かない場合は、フローの各ステップとサブステップを編集して、接続を追加できます。</span><span class="sxs-lookup"><span data-stu-id="6aadc-156">If the dialog to add connections doesn't open up automatically while editing the flow, then you can edit each of the steps and substeps of the flows to add the connections.</span></span>

- <span data-ttu-id="6aadc-157">各フローを選択し、個別に編集します。</span><span class="sxs-lookup"><span data-stu-id="6aadc-157">Select each flow and edit them individually.</span></span>
- <span data-ttu-id="6aadc-158">フロー内のすべてのステップを展開する</span><span class="sxs-lookup"><span data-stu-id="6aadc-158">Expand all the steps in the flow</span></span> 

:::image type="content" source="images/cosellconnectors/flowsteps.png" alt-text="接続が必要な手順":::

- <span data-ttu-id="6aadc-160">接続の関連付けと接続の追加を求める警告アイコンが表示される手順を選択します。</span><span class="sxs-lookup"><span data-stu-id="6aadc-160">Select the steps where you see a warning icon asking to associate connections, and add connections.</span></span> 

:::image type="content" source="images/cosellconnectors/editflow.png" alt-text="フローステップをステップごとに編集":::


5. <span data-ttu-id="6aadc-162">共同販売参照コネクタソリューションのフローがアクティブになっていない場合 (有効になっている場合)</span><span class="sxs-lookup"><span data-stu-id="6aadc-162">What should you do if the flows of the Co-sell Referrals Connectors solution don’t activate (turn-on)?</span></span>

    <span data-ttu-id="6aadc-163">A.</span><span class="sxs-lookup"><span data-stu-id="6aadc-163">A.</span></span> <span data-ttu-id="6aadc-164">Power の自動化では、次の順序でフローを編集し、それぞれの接続を使用するように更新する必要があります。</span><span class="sxs-lookup"><span data-stu-id="6aadc-164">In Power Automate, you will need to edit flows in the following order and update them to use respective connections:</span></span>

    - <span data-ttu-id="6aadc-165">パートナーセンターの Webhook の登録 (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="6aadc-165">Partner Center Webhook Registration (Insider Preview)</span></span>
    - <span data-ttu-id="6aadc-166">パートナーセンターへの共同販売参照の作成-Salesforce (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="6aadc-166">Create Co-sell Referral - Salesforce to Partner Center (Insider Preview)</span></span>
    - <span data-ttu-id="6aadc-167">パートナーセンター: Microsoft 共同での Salesforce の参照の更新 (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="6aadc-167">Partner Center Microsoft Co-sell Referral Updates to Salesforce (Insider Preview)</span></span>
    - <span data-ttu-id="6aadc-168">パートナーセンターから Salesforce へ (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="6aadc-168">Partner Center to Salesforce (Insider Preview)</span></span>
    - <span data-ttu-id="6aadc-169">Salesforce からパートナーセンターへ (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="6aadc-169">Salesforce to Partner Center (Insider Preview)</span></span>
    - <span data-ttu-id="6aadc-170">パートナーセンターへの Salesforce の営業案件 (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="6aadc-170">Salesforce Opportunity to Partner Center (Insider Preview)</span></span>
    - <span data-ttu-id="6aadc-171">パートナーセンターへの Salesforce Microsoft ソリューション (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="6aadc-171">Salesforce Microsoft Solutions to Partner Center (Insider Preview)</span></span>

    <span data-ttu-id="6aadc-172">B.</span><span class="sxs-lookup"><span data-stu-id="6aadc-172">B.</span></span> <span data-ttu-id="6aadc-173">各フローに対して、[ **ユーザーのみ実行** ] オプションを選択します。</span><span class="sxs-lookup"><span data-stu-id="6aadc-173">For each of flow, select **Run only users** option.</span></span> <span data-ttu-id="6aadc-174">[**実行専用ユーザーによって提供される**のではなく、**接続を使用する**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="6aadc-174">Select **Use connection** instead of **Provided by run-only user**.</span></span>  

:::image type="content" source="images/cosellconnectors/runonly.png" alt-text="フローをアクティブ化するには":::

<span data-ttu-id="6aadc-176">C.</span><span class="sxs-lookup"><span data-stu-id="6aadc-176">C.</span></span> <span data-ttu-id="6aadc-177">以下のフローフローをアクティブにします。</span><span class="sxs-lookup"><span data-stu-id="6aadc-177">Activate these below mentioned flows:</span></span>

- <span data-ttu-id="6aadc-178">パートナーセンター: Microsoft 共同での Salesforce の参照の更新 (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="6aadc-178">Partner Center Microsoft Co-sell Referral Updates to Salesforce (Insider Preview)</span></span>

- <span data-ttu-id="6aadc-179">Salesforce からパートナーセンターへ (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="6aadc-179">Salesforce to Partner Center (Insider Preview)</span></span>


<span data-ttu-id="6aadc-180">D.</span><span class="sxs-lookup"><span data-stu-id="6aadc-180">D.</span></span> <span data-ttu-id="6aadc-181">残りのすべてのフローをアクティブ化します。</span><span class="sxs-lookup"><span data-stu-id="6aadc-181">Activate all the remaining flows.</span></span>

<span data-ttu-id="6aadc-182">E.</span><span class="sxs-lookup"><span data-stu-id="6aadc-182">E.</span></span> <span data-ttu-id="6aadc-183">Flow パートナーセンターの Webhook 登録で、[ **実行**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="6aadc-183">At flow Partner Center Webhook Registration, select **Run**.</span></span> <span data-ttu-id="6aadc-184">**パートナーセンター**の最初のアクションから Salesforce flow に**http url**を指定します。</span><span class="sxs-lookup"><span data-stu-id="6aadc-184">Provide the **http url** from the first action in **Partner Center to Salesforce** flow.</span></span> <span data-ttu-id="6aadc-185">[ **登録するイベント** ] の下にある4つのオプションをすべて選択し、[上書き] で [ **はい]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="6aadc-185">Select all four options under **Events to register** and select **yes** for Overwrite.</span></span>

## <a name="questions-and-answers-about-runmaintenance"></a><span data-ttu-id="6aadc-186">実行/メンテナンスに関する質問と回答</span><span class="sxs-lookup"><span data-stu-id="6aadc-186">Questions and answers about Run/Maintenance</span></span>

1. <span data-ttu-id="6aadc-187">電源自動化フロー実行中にエラーが発生した場合のトラブルシューティング方法</span><span class="sxs-lookup"><span data-stu-id="6aadc-187">How do you troubleshoot in case of failures during Power Automate flow execution?</span></span>

<span data-ttu-id="6aadc-188">フローが期待どおりに実行されるようにし、実行中のエラーをトラブルシューティングするには、 [フローエラーの修正](/power-automate/fix-flow-failures)に関する記述を参照してください。</span><span class="sxs-lookup"><span data-stu-id="6aadc-188">To ensure that your Power Automate flows run as you expect and to troubleshoot failures during execution, refer to [Fix flow failures](/power-automate/fix-flow-failures).</span></span>

2. <span data-ttu-id="6aadc-189">パートナーセンターまたは CRM 環境で適切に同期されていない参照が表示される場合は、どうすればよいですか。</span><span class="sxs-lookup"><span data-stu-id="6aadc-189">What should you do if you see referrals that aren't synchronized properly in Partner Center or CRM environment?</span></span>
 
<span data-ttu-id="6aadc-190">参照同期の状態を確認するには、[ **監査**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="6aadc-190">To determine the status of referral synchronization, select **Audit**.</span></span> 

:::image type="content" source="images/cosellconnectors/synch.png" alt-text="参照を同期する方法":::

<span data-ttu-id="6aadc-192">次の条件が満たされていることを確認します。</span><span class="sxs-lookup"><span data-stu-id="6aadc-192">Ensure that the following conditions are met:</span></span>

- <span data-ttu-id="6aadc-193">ソリューション id は、営業案件の一部として提供されます。</span><span class="sxs-lookup"><span data-stu-id="6aadc-193">Solution id is provided as part of the opportunity.</span></span>

- <span data-ttu-id="6aadc-194">2文字の国コードが必要です。</span><span class="sxs-lookup"><span data-stu-id="6aadc-194">Two letter country code is required.</span></span>

- <span data-ttu-id="6aadc-195">営業案件について Microsoft からのヘルプが選択されている場合は、顧客の連絡先情報が必要です。</span><span class="sxs-lookup"><span data-stu-id="6aadc-195">When help from Microsoft is selected for the opportunity, customer contact information is required.</span></span>

3. <span data-ttu-id="6aadc-196">参照を双方向に同期させない条件の下</span><span class="sxs-lookup"><span data-stu-id="6aadc-196">Under what conditions a referral won’t synchronize bi-directionally</span></span>

<span data-ttu-id="6aadc-197">以下のことを確認してください。</span><span class="sxs-lookup"><span data-stu-id="6aadc-197">Ensure the following:</span></span>

- <span data-ttu-id="6aadc-198">パートナーの販売者は、CRM セクションで **パートナーセンターオプションとの同期** を有効にしていることを確認する必要があります。</span><span class="sxs-lookup"><span data-stu-id="6aadc-198">Partner sellers need to ensure that they have enabled **Sync with Partner Center** option in the CRM section.</span></span>

:::image type="content" source="images/cosellconnectors/enablesynch.png" alt-text="同期が有効になっていることを確認する":::

- <span data-ttu-id="6aadc-200">販売元は、潜在顧客を限定するときに収益と終了日を提供する必要があります。</span><span class="sxs-lookup"><span data-stu-id="6aadc-200">Sellers need to provide revenue and closing date when qualifying a lead.</span></span>

- <span data-ttu-id="6aadc-201">CRM id が共同販売の機会の作成または更新に指定されていて、その id を持つ潜在顧客が CRM で見つからない場合は、その営業案件の update または create は無視されます。</span><span class="sxs-lookup"><span data-stu-id="6aadc-201">If CRM id is provided in create or update of co-sell opportunity and if a lead/opportunity with that id is not found in CRM, then update or create will be ignored for that opportunity.</span></span>

- <span data-ttu-id="6aadc-202">[紹介通貨] フィールドが Salesforce 環境で構成されていることを確認します。</span><span class="sxs-lookup"><span data-stu-id="6aadc-202">Ensure that referral currency field is configured on Salesforce environment.</span></span> 

4. <span data-ttu-id="6aadc-203">コネクタが切断され、参照の同期が失われた場合はどうすればよいですか。</span><span class="sxs-lookup"><span data-stu-id="6aadc-203">What should you do if the connector gets disconnected and you miss a referral synchronization.</span></span> 

<span data-ttu-id="6aadc-204">次に、試してみることのできるオプションをいくつか示します。</span><span class="sxs-lookup"><span data-stu-id="6aadc-204">Following are few of the options that you can try out:</span></span>

- <span data-ttu-id="6aadc-205">パートナーセンターのユーザーに対して、ユーザー名またはパスワードの有効期限が切れているかどうかを確認します。</span><span class="sxs-lookup"><span data-stu-id="6aadc-205">Check whether username or password has expired for the Partner Center user with referral admin roles.</span></span>

- <span data-ttu-id="6aadc-206">同期されていない営業案件にアクセスし、マイナー更新を行い、参照が同期されているかどうかを確認できます。</span><span class="sxs-lookup"><span data-stu-id="6aadc-206">You can go to the un-synchronized opportunity, make a minor update, and observe whether the referral has synchronized.</span></span>

- <span data-ttu-id="6aadc-207">フローが実行されて失敗した場合は、フローを選択し、失敗した実行を再送信します。</span><span class="sxs-lookup"><span data-stu-id="6aadc-207">If the flows have run and failed, then select the flow and re-submit the run which has failed.</span></span>

5. <span data-ttu-id="6aadc-208">アクセス拒否エラーが発生した場合はどうすればよいですか?</span><span class="sxs-lookup"><span data-stu-id="6aadc-208">What should you do when you get access denied errors?</span></span>

<span data-ttu-id="6aadc-209">適切なロールが存在することを確認する</span><span class="sxs-lookup"><span data-stu-id="6aadc-209">Make sure the appropriate roles exist</span></span>

- <span data-ttu-id="6aadc-210">パートナーセンターの販売者の紹介管理者ロール</span><span class="sxs-lookup"><span data-stu-id="6aadc-210">Referral Administrator role for Partner Center seller</span></span> 
 
- <span data-ttu-id="6aadc-211">CRM インスタンスのシステム管理者ロールまたはシステムカスタマイザーロール</span><span class="sxs-lookup"><span data-stu-id="6aadc-211">System Administrator or System Customizer role on your CRM instance</span></span>

- <span data-ttu-id="6aadc-212">フローアカウントのユーザーログが https://flow.microsoft.com 少なくとも事前に1回は自動で実行されていることを確認します。</span><span class="sxs-lookup"><span data-stu-id="6aadc-212">Ensure that the Power Automate flow account user logs into https://flow.microsoft.com at least once beforehand</span></span>

6. <span data-ttu-id="6aadc-213">共同販売の機会の作成中に **顧客アカウントの国コード** が不足していることがわかった場合は、どうすればよいでしょうか。</span><span class="sxs-lookup"><span data-stu-id="6aadc-213">If you see that **Customer account country code** is missing while creating a Co-sell opportunity, what should you do?</span></span>

<span data-ttu-id="6aadc-214">ISO の2文字の国コードを CRM の顧客アカウントに追加する必要があります。</span><span class="sxs-lookup"><span data-stu-id="6aadc-214">You will need to add the ISO two-letter country code to the Customer account in CRM.</span></span>

7. <span data-ttu-id="6aadc-215">共同販売の機会を作成するときに **ソリューション Id が必要** であるというエラーが表示された場合はどうすればよいですか。</span><span class="sxs-lookup"><span data-stu-id="6aadc-215">What should you do if you see the error that **Solution Id is required** while creating a Co-sell opportunity?</span></span>

<span data-ttu-id="6aadc-216">共同販売の紹介を作成するには、Microsoft 共同販売の準備ができているソリューションが必要です。</span><span class="sxs-lookup"><span data-stu-id="6aadc-216">In order to create a co-sell referral, you need a Microsoft co-sell ready solution.</span></span> 

8. <span data-ttu-id="6aadc-217">フローエラーが発生していなくても CRM に同期されていない共同販売機会がパートナーセンターで作成されている場合は、次のことを行う必要があります。</span><span class="sxs-lookup"><span data-stu-id="6aadc-217">What should you do when you see Co-sell opportunities created in Partner Center that aren't synchronized to CRM even though there are no flow errors:</span></span>

<span data-ttu-id="6aadc-218">次の手順を実行します。</span><span class="sxs-lookup"><span data-stu-id="6aadc-218">Do the following:</span></span>

- <span data-ttu-id="6aadc-219">パートナーセンターで新しい共同販売取引を作成した後、パートナーセンターから Dynamics 365 へのフローが呼び出されるかどうかを確認します (複数回呼び出される可能性があります)。</span><span class="sxs-lookup"><span data-stu-id="6aadc-219">After you have created a new co-sell deal in Partner Center, check if Partner Center to Dynamics 365 flow gets invoked (it might get invoked multiple times).</span></span>

- <span data-ttu-id="6aadc-220">フローが呼び出された場合は、呼び出されたすべてのフローを確認し、CRM を更新するフロー実行を特定します。</span><span class="sxs-lookup"><span data-stu-id="6aadc-220">If the flow gets invoked, check all invoked flows, and identify the flow run which would update the CRM.</span></span> <span data-ttu-id="6aadc-221">アクションに従って操作を実行し、CRM が更新されたか、または問題が発生したかどうかを確認できます。</span><span class="sxs-lookup"><span data-stu-id="6aadc-221">You can follow the actions and verify if it did update the CRM or encountered a problem.</span></span>

- <span data-ttu-id="6aadc-222">パートナーセンターで *新しい商談*\* を確認し、CRM id が設定されているかどうかを確認します。</span><span class="sxs-lookup"><span data-stu-id="6aadc-222">Check *New deal*\* in Partner Center to see if it gets populated with CRM id.</span></span>

- <span data-ttu-id="6aadc-223">パートナーセンターで、取引が誤って "勝ち" または "Lost" として閉じられていないことを確認します。</span><span class="sxs-lookup"><span data-stu-id="6aadc-223">Make sure that the deal is not accidentally closed as “Won” or “Lost” in Partner Center.</span></span>

## <a name="next-steps"></a><span data-ttu-id="6aadc-224">次のステップ</span><span class="sxs-lookup"><span data-stu-id="6aadc-224">Next steps</span></span>

- [<span data-ttu-id="6aadc-225">見込み客を管理する</span><span class="sxs-lookup"><span data-stu-id="6aadc-225">Manage leads</span></span>](manage-leads.md)
 
- [<span data-ttu-id="6aadc-226">共同販売の機会を管理する</span><span class="sxs-lookup"><span data-stu-id="6aadc-226">Manage co-sell opportunities</span></span>](manage-co-sell-opportunities.md)