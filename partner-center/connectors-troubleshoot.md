---
title: 共同販売紹介コネクタのトラブルシューティング
ms.topic: how-to
ms.date: 09/21/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 共同販売コネクタの使用に関してよく寄せられる質問への回答について説明します。 共同販売コネクタのトラブルシューティング方法については、こちらの FAQ を参照してください。
author: sroy
ms.author: sroy
ms.localizationpriority: medium
ms.openlocfilehash: b8977f7c602b8587a619236b37a760a55bf87e53
ms.sourcegitcommit: 22d79fb31cce852ae809078ea2310ebc80030739
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/12/2020
ms.locfileid: "97354544"
---
# <a name="troubleshoot-co-sell-referrals-connectors"></a><span data-ttu-id="1acd7-104">共同販売紹介コネクタのトラブルシューティング</span><span class="sxs-lookup"><span data-stu-id="1acd7-104">Troubleshoot co-sell referrals connectors</span></span>

<span data-ttu-id="1acd7-105">**適用対象:**</span><span class="sxs-lookup"><span data-stu-id="1acd7-105">**Applies to:**</span></span>

- <span data-ttu-id="1acd7-106">Dynamics 365 CRM</span><span class="sxs-lookup"><span data-stu-id="1acd7-106">Dynamics 365 CRM</span></span>
- <span data-ttu-id="1acd7-107">Salesforce CRM</span><span class="sxs-lookup"><span data-stu-id="1acd7-107">Salesforce CRM</span></span>

<span data-ttu-id="1acd7-108">**適切なロール**</span><span class="sxs-lookup"><span data-stu-id="1acd7-108">**Appropriate roles**</span></span>

- <span data-ttu-id="1acd7-109">紹介管理者</span><span class="sxs-lookup"><span data-stu-id="1acd7-109">Referrals admin</span></span>
- <span data-ttu-id="1acd7-110">CRM のシステム管理者またはシステムカスタマイザー</span><span class="sxs-lookup"><span data-stu-id="1acd7-110">System admin or system customizer on the CRM</span></span>

 ## <a name="questions-and-answers-about-pre-requisites"></a><span data-ttu-id="1acd7-111">前提条件に関する質問と回答</span><span class="sxs-lookup"><span data-stu-id="1acd7-111">Questions and answers about pre-requisites</span></span>

1. <span data-ttu-id="1acd7-112">お使いの環境に対して試用版の共同販売紹介コネクタソリューションを使用できますか。</span><span class="sxs-lookup"><span data-stu-id="1acd7-112">Can you use a trial co-sell referrals connectors solution for your environment?</span></span>

<span data-ttu-id="1acd7-113">テスト/ステージング環境を使用している場合は、試用版ソリューションを選択できます。</span><span class="sxs-lookup"><span data-stu-id="1acd7-113">If you are on the test/staging environment, you can opt for trial solution.</span></span> <span data-ttu-id="1acd7-114">このコネクタの有料バージョンは、AppSource で米国ドルの 15/月でご利用いただけます。</span><span class="sxs-lookup"><span data-stu-id="1acd7-114">The paid version of the Connectors is available in AppSource at US$ 15/month.</span></span> <span data-ttu-id="1acd7-115">有料接続では、1日あたり10K の API 呼び出しを取得します。</span><span class="sxs-lookup"><span data-stu-id="1acd7-115">With the paid connection, you will be getting 10K API calls per day.</span></span> <span data-ttu-id="1acd7-116">コネクタは、パートナーセンターの参照 Api の上にあるラッパーです。</span><span class="sxs-lookup"><span data-stu-id="1acd7-116">The Connectors are wrappers on top of Partner Center referral APIs.</span></span> <span data-ttu-id="1acd7-117">パートナーセンターまたは CRM 側の営業案件で、コネクタソリューションが **作成** または **更新** イベントに対して実行されるたびに、API 呼び出しが行われます。</span><span class="sxs-lookup"><span data-stu-id="1acd7-117">Whenever the connector solutions run for a **Create** or **Update** event on the opportunities on either Partner Center or the CRM side, an API call is made.</span></span>

2. <span data-ttu-id="1acd7-118">CRM 環境でセクションを作成するにはどのような役割が必要ですか。</span><span class="sxs-lookup"><span data-stu-id="1acd7-118">What role do you need to create sections in CRM environment?</span></span>

<span data-ttu-id="1acd7-119">システム管理者またはシステムカスタマイザーのユーザーは、すべてのユーザーに変更を適用できます。</span><span class="sxs-lookup"><span data-stu-id="1acd7-119">Users who are system admins or system customizers can apply changes for everyone.</span></span> <span data-ttu-id="1acd7-120">ただし、すべてのアプリユーザーがシステムをカスタマイズしたり、カスタマイズの一部を他のユーザーと共有したりすることもできます。</span><span class="sxs-lookup"><span data-stu-id="1acd7-120">All app users, however,  can personalize the system and even share some of their customizations with others.</span></span> 

3. <span data-ttu-id="1acd7-121">パートナー販売者は、パートナーセンターで作業するために特別な役割を必要としていますか。</span><span class="sxs-lookup"><span data-stu-id="1acd7-121">Do partner sellers need special roles to work on Partner Center?</span></span>
 
<span data-ttu-id="1acd7-122">パートナーの販売元には、"紹介管理者" ロールが割り当てられている必要があります。</span><span class="sxs-lookup"><span data-stu-id="1acd7-122">Partner sellers must be assigned the “Referrals admin” role.</span></span> <span data-ttu-id="1acd7-123">詳細については、次の「アクセス許可の概要」を参照してください (作成-ユーザーアカウントと-設定-アクセス許可)。</span><span class="sxs-lookup"><span data-stu-id="1acd7-123">For more information, refer to the following [Permissions overview)(create-user-accounts-and-set-permissions).</span></span>

4. <span data-ttu-id="1acd7-124">CRM 環境で最初にどのようなフィールドを設定する必要がありますか。</span><span class="sxs-lookup"><span data-stu-id="1acd7-124">What fields need to be set up first in your CRM environment?</span></span> 

<span data-ttu-id="1acd7-125">•お客様の地域に合った通貨を使用していること、および CRM 環境に正確に対応していることを確認してください。</span><span class="sxs-lookup"><span data-stu-id="1acd7-125">• Make sure your currency is appropriate to your location and is in your CRM environment accurately.</span></span> <span data-ttu-id="1acd7-126">• Crm ユーザーとして CRM 環境に販売チームが一覧表示されている必要があります。</span><span class="sxs-lookup"><span data-stu-id="1acd7-126">• Your sales team should be listed in your CRM environment as CRM users.</span></span>

5. <span data-ttu-id="1acd7-127">環境の作成を自動化するために必要な前提条件は何ですか。</span><span class="sxs-lookup"><span data-stu-id="1acd7-127">What pre-requisites are required for Power Automate environment creation?</span></span>

<span data-ttu-id="1acd7-128">電力自動化環境を使用するには、次のものが必要です。</span><span class="sxs-lookup"><span data-stu-id="1acd7-128">To use the Power Automate environment, you need:</span></span>

- <span data-ttu-id="1acd7-129">Power 自動ライセンス認証が必要です。</span><span class="sxs-lookup"><span data-stu-id="1acd7-129">A Power Automate license is required.</span></span>
- <span data-ttu-id="1acd7-130">少なくとも 1 GB のストレージが必要です。</span><span class="sxs-lookup"><span data-stu-id="1acd7-130">A minimum of 1-GB storage is required.</span></span>

6.  <span data-ttu-id="1acd7-131">Salesforce コネクタソリューションを使用するには、Dynamics 365 サブスクリプションが必要ですか?</span><span class="sxs-lookup"><span data-stu-id="1acd7-131">Do you need a Dynamics 365 subscription to use Salesforce Connectors solution?</span></span>

<span data-ttu-id="1acd7-132">Salesforce コネクタソリューションの種類は "Dynamics Flow" で、他の CRM システムとの同期をサポートしています。</span><span class="sxs-lookup"><span data-stu-id="1acd7-132">The Salesforce Connector solution is of type “Dynamics Flow” that supports synchronizing with other CRM systems.</span></span> <span data-ttu-id="1acd7-133">このソリューションでは、Dynamics 365 インスタンスまたはサブスクリプションが必要ではありません。</span><span class="sxs-lookup"><span data-stu-id="1acd7-133">The solution doesn’t require you to have a Dynamics 365 instance or a subscription.</span></span> <span data-ttu-id="1acd7-134">Salesforce ソリューションをインストールするときに、会社内の既存の CD 環境を含むドロップダウンが表示されることがあります。</span><span class="sxs-lookup"><span data-stu-id="1acd7-134">While installing the Salesforce solution, a drop-down with existing CDS environment in your company may appear.</span></span> <span data-ttu-id="1acd7-135">その環境を選択する必要があります。</span><span class="sxs-lookup"><span data-stu-id="1acd7-135">You need to select that environment.</span></span> <span data-ttu-id="1acd7-136">さらに、"サインインしたユーザーに接続された Dynamics 365 組織が見つかりませんでした" というエラーが表示された場合は、コネクタ用に新しい環境を作成する必要があります。</span><span class="sxs-lookup"><span data-stu-id="1acd7-136">In addition, if you get the error "We couldn't find a Dynamics 365 organization connected to signed-in user", then you will need to create new environment for connector.</span></span>

## <a name="questions-and-answers-about-configuration"></a><span data-ttu-id="1acd7-137">構成に関する質問と回答</span><span class="sxs-lookup"><span data-stu-id="1acd7-137">Questions and answers about configuration</span></span>

1. <span data-ttu-id="1acd7-138">パワー自動化プラットフォームでフローをアクティブ化しているときに、次のエラーが発生した場合はどうすればよいですか?</span><span class="sxs-lookup"><span data-stu-id="1acd7-138">What should you do if you face the following error while activating flows in Power Automate Platform?</span></span>

<span data-ttu-id="1acd7-139">エラー: Azure Resource Manager への要求が失敗しました。エラー: ' {"エラー": {"code": "WorkflowTriggerNotFound"、"message": "ワークフロー ' e14d00f1-1fdf-4b1b-aaac-54a5064093d3 ' トリガー ' manual ' が見つかりませんでした。"}} '。</span><span class="sxs-lookup"><span data-stu-id="1acd7-139">Error: Request to Azure Resource Manager failed with error: '{"error":{"code":"WorkflowTriggerNotFound","message":"The workflow 'e14d00f1-1fdf-4b1b-aaac-54a5064093d3' trigger 'manual' could not be found."}}'.</span></span> 

<span data-ttu-id="1acd7-140">次のトラブルシューティング手順に従います。</span><span class="sxs-lookup"><span data-stu-id="1acd7-140">Follow these troubleshooting steps:</span></span>

- <span data-ttu-id="1acd7-141">CD 接続を削除してから、CD 接続を再作成してください。</span><span class="sxs-lookup"><span data-stu-id="1acd7-141">Delete the CDS connection and then recreate the CDS connections.</span></span>
- <span data-ttu-id="1acd7-142">子フローをオフまたはオンにする</span><span class="sxs-lookup"><span data-stu-id="1acd7-142">Turn the child flow off and on</span></span> 
- <span data-ttu-id="1acd7-143">ソリューションを削除してから、ソリューションを再インストールしてください。</span><span class="sxs-lookup"><span data-stu-id="1acd7-143">Delete solution and then reinstall the solution.</span></span> 

2.  <span data-ttu-id="1acd7-144">Power オートメーションプラットフォームでパートナーセンターコネクタを追加するときに "サインイン" エラーが発生した場合はどうすればよいですか?</span><span class="sxs-lookup"><span data-stu-id="1acd7-144">What should you do if you face the "Sign in" error while adding a Partner Center connector in Power Automate Platform?</span></span>

:::image type="content" source="images/cosellconnectors/failure.png" alt-text="サインインが必要なエラーメッセージ":::

<span data-ttu-id="1acd7-146">このトラブルシューティングの手順に従います。</span><span class="sxs-lookup"><span data-stu-id="1acd7-146">Follow this troubleshooting step:</span></span>

- <span data-ttu-id="1acd7-147">パートナーセンターの資格情報を使用して、flow 環境に1回サインインします (flow.microsoft.com)。</span><span class="sxs-lookup"><span data-stu-id="1acd7-147">Use your Partner Center credentials to sign into the flow environment once (flow.microsoft.com).</span></span>


3. <span data-ttu-id="1acd7-148">Power オートメーションプラットフォームでパートナーセンターから CRM へのフローをアクティブにするときに、次のエラーが発生した場合はどうすればよいですか?</span><span class="sxs-lookup"><span data-stu-id="1acd7-148">What should you do if you receive the following error while activating the Partner Center to CRM flow in Power Automate Platform?</span></span>
 
:::image type="content" source="images/cosellconnectors/powererror.png" alt-text="更新が必要なエラーメッセージ":::

<span data-ttu-id="1acd7-150">次のトラブルシューティング手順に従います。</span><span class="sxs-lookup"><span data-stu-id="1acd7-150">Follow these troubleshooting steps:</span></span>

- <span data-ttu-id="1acd7-151">パートナーセンターを CRM フローにアクティブ化する前に、まず次の2つの子フローをアクティブ化します。</span><span class="sxs-lookup"><span data-stu-id="1acd7-151">Activate the following two child flows first before you activate the Partner Center to CRM flow.</span></span>
      - <span data-ttu-id="1acd7-152">パートナーセンターから CRM ヘルパーへ (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="1acd7-152">Partner Center to CRM - Helper (Insider Preview)</span></span>
      - <span data-ttu-id="1acd7-153">パートナーセンターの Microsoft 共同販売の CRM の参照の更新 (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="1acd7-153">Partner Center Microsoft Co-sell Referral Updates to CRM (Insider Preview)</span></span>

4. <span data-ttu-id="1acd7-154">フローを編集しようとすると、フローに接続を追加できない場合はどうすればよいですか。</span><span class="sxs-lookup"><span data-stu-id="1acd7-154">What should you do when you aren't able to add connections to the flow when you try to edit the flow?</span></span>

<span data-ttu-id="1acd7-155">フローの実行中にフローへの接続を追加し、各フローに個別に追加します。</span><span class="sxs-lookup"><span data-stu-id="1acd7-155">You add connections to the flow while the flow is running, and you add to each flow separately.</span></span>  <span data-ttu-id="1acd7-156">フローの編集中に接続を追加するダイアログボックスが自動的に開かない場合は、フローの各ステップとサブステップを個別に編集できます。</span><span class="sxs-lookup"><span data-stu-id="1acd7-156">If the dialog to add connections doesn't open up automatically while editing the flow, then you can edit each of the steps and sub steps of the flows individually.</span></span>

- <span data-ttu-id="1acd7-157">各フローを選択し、個別に編集します。</span><span class="sxs-lookup"><span data-stu-id="1acd7-157">Select each flow and edit them individually.</span></span>
- <span data-ttu-id="1acd7-158">フロー内のすべてのステップを展開する</span><span class="sxs-lookup"><span data-stu-id="1acd7-158">Expand all the steps in the flow</span></span> 

:::image type="content" source="images/cosellconnectors/flowsteps.png" alt-text="接続が必要な手順":::

- <span data-ttu-id="1acd7-160">接続の関連付けと接続の追加を求める警告アイコンが表示される手順を選択します。</span><span class="sxs-lookup"><span data-stu-id="1acd7-160">Select the steps where you see a warning icon asking to associate connections, and add connections.</span></span> 

:::image type="content" source="images/cosellconnectors/editflow.png" alt-text="フローステップをステップごとに編集":::


5. <span data-ttu-id="1acd7-162">共同販売参照コネクタソリューションのフローが有効になっていない場合はどうすればよいですか。</span><span class="sxs-lookup"><span data-stu-id="1acd7-162">What should you do if the flows of the Co-sell Referrals Connectors solution don’t turn on?</span></span>

<span data-ttu-id="1acd7-163">A.</span><span class="sxs-lookup"><span data-stu-id="1acd7-163">A.</span></span> <span data-ttu-id="1acd7-164">Power の自動化では、次の順序でフローを編集し、正しい接続を使用するように更新する必要があります。</span><span class="sxs-lookup"><span data-stu-id="1acd7-164">In Power Automate, you'll need to edit flows in the following order and update them to use the correct connections:</span></span>

- <span data-ttu-id="1acd7-165">パートナーセンターの Webhook の登録 (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="1acd7-165">Partner Center Webhook Registration (Insider Preview)</span></span>
- <span data-ttu-id="1acd7-166">パートナーセンターへの共同販売参照の作成-Salesforce (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="1acd7-166">Create Co-sell Referral - Salesforce to Partner Center (Insider Preview)</span></span>
- <span data-ttu-id="1acd7-167">パートナーセンター: Microsoft 共同での Salesforce の参照の更新 (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="1acd7-167">Partner Center Microsoft Co-sell Referral Updates to Salesforce (Insider Preview)</span></span>
- <span data-ttu-id="1acd7-168">パートナーセンターから Salesforce へ (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="1acd7-168">Partner Center to Salesforce (Insider Preview)</span></span>
- <span data-ttu-id="1acd7-169">Salesforce からパートナーセンターへ (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="1acd7-169">Salesforce to Partner Center (Insider Preview)</span></span>
- <span data-ttu-id="1acd7-170">パートナーセンターへの Salesforce の営業案件 (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="1acd7-170">Salesforce Opportunity to Partner Center (Insider Preview)</span></span>
- <span data-ttu-id="1acd7-171">パートナーセンターへの Salesforce Microsoft ソリューション (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="1acd7-171">Salesforce Microsoft Solutions to Partner Center (Insider Preview)</span></span>

 <span data-ttu-id="1acd7-172">B.</span><span class="sxs-lookup"><span data-stu-id="1acd7-172">B.</span></span> <span data-ttu-id="1acd7-173">各フローに対して、[ **ユーザーのみ実行** ] オプションを選択します。</span><span class="sxs-lookup"><span data-stu-id="1acd7-173">For each of flow, select **Run only users** option.</span></span> <span data-ttu-id="1acd7-174">[**実行専用ユーザーによって提供される** のではなく、**接続を使用する**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="1acd7-174">Select **Use connection** instead of **Provided by run-only user**.</span></span>  

:::image type="content" source="images/cosellconnectors/runonly.png" alt-text="フローをアクティブ化するには":::


<span data-ttu-id="1acd7-176">C.</span><span class="sxs-lookup"><span data-stu-id="1acd7-176">C.</span></span> <span data-ttu-id="1acd7-177">以下のフローフローをアクティブにします。</span><span class="sxs-lookup"><span data-stu-id="1acd7-177">Activate these below mentioned flows:</span></span>

 - <span data-ttu-id="1acd7-178">パートナーセンター: Microsoft 共同での Salesforce の参照の更新 (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="1acd7-178">Partner Center Microsoft Co-sell Referral Updates to Salesforce (Insider Preview)</span></span>

- <span data-ttu-id="1acd7-179">Salesforce からパートナーセンターへ (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="1acd7-179">Salesforce to Partner Center (Insider Preview)</span></span>

    
<span data-ttu-id="1acd7-180">D.</span><span class="sxs-lookup"><span data-stu-id="1acd7-180">D.</span></span> <span data-ttu-id="1acd7-181">残りのすべてのフローをアクティブ化します。</span><span class="sxs-lookup"><span data-stu-id="1acd7-181">Activate all the remaining flows.</span></span>

<span data-ttu-id="1acd7-182">E.</span><span class="sxs-lookup"><span data-stu-id="1acd7-182">E.</span></span> <span data-ttu-id="1acd7-183">Flow パートナーセンターの Webhook 登録で、[ **実行**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="1acd7-183">At flow Partner Center Webhook Registration, select **Run**.</span></span> <span data-ttu-id="1acd7-184">**パートナーセンター** の最初のアクションから Salesforce flow に **http url** を指定します。</span><span class="sxs-lookup"><span data-stu-id="1acd7-184">Provide the **http url** from the first action in **Partner Center to Salesforce** flow.</span></span> <span data-ttu-id="1acd7-185">[ **登録するイベント** ] の下にある4つのオプションをすべて選択し、[上書き] で [ **はい]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="1acd7-185">Select all four options under **Events to register** and select **yes** for Overwrite.</span></span>

## <a name="questions-and-answers-about-runmaintenance"></a><span data-ttu-id="1acd7-186">実行/メンテナンスに関する質問と回答</span><span class="sxs-lookup"><span data-stu-id="1acd7-186">Questions and answers about Run/Maintenance</span></span>

1. <span data-ttu-id="1acd7-187">電源自動化フロー実行中にエラーが発生した場合のトラブルシューティング方法</span><span class="sxs-lookup"><span data-stu-id="1acd7-187">How do you troubleshoot in case of failures during Power Automate flow execution?</span></span>

<span data-ttu-id="1acd7-188">フローが期待どおりに実行されるようにし、実行中のエラーをトラブルシューティングするには、 [フローエラーの修正](/power-automate/fix-flow-failures)に関する記述を参照してください。</span><span class="sxs-lookup"><span data-stu-id="1acd7-188">To ensure that your Power Automate flows run as you expect and to troubleshoot failures during execution, refer to [Fix flow failures](/power-automate/fix-flow-failures).</span></span>

2. <span data-ttu-id="1acd7-189">パートナーセンターまたは CRM 環境で適切に同期されていない参照が表示される場合は、どうすればよいですか。</span><span class="sxs-lookup"><span data-stu-id="1acd7-189">What should you do if you see referrals that aren't synchronized properly in Partner Center or CRM environment?</span></span>
 
<span data-ttu-id="1acd7-190">参照同期の状態を確認するには、[ **監査**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="1acd7-190">To determine the status of referral synchronization, select **Audit**.</span></span> 

:::image type="content" source="images/cosellconnectors/synch.png" alt-text="参照を同期する方法":::

<span data-ttu-id="1acd7-192">次の条件が満たされていることを確認します。</span><span class="sxs-lookup"><span data-stu-id="1acd7-192">Ensure that the following conditions are met:</span></span>

- <span data-ttu-id="1acd7-193">ソリューション ID は、営業案件の一部として提供されます。</span><span class="sxs-lookup"><span data-stu-id="1acd7-193">Solution ID is provided as part of the opportunity.</span></span>

- <span data-ttu-id="1acd7-194">2文字の国コードが必要です。</span><span class="sxs-lookup"><span data-stu-id="1acd7-194">Two letter country code is required.</span></span>

- <span data-ttu-id="1acd7-195">営業案件について Microsoft からのヘルプが選択されている場合は、顧客の連絡先情報が必要です。</span><span class="sxs-lookup"><span data-stu-id="1acd7-195">When help from Microsoft is selected for the opportunity, customer contact information is required.</span></span>

3. <span data-ttu-id="1acd7-196">参照を双方向に同期させる方法</span><span class="sxs-lookup"><span data-stu-id="1acd7-196">How to ensure that a referral will synchronize bi-directionally?</span></span>

<span data-ttu-id="1acd7-197">手順は次のとおりです。</span><span class="sxs-lookup"><span data-stu-id="1acd7-197">Do the following steps:</span></span>

- <span data-ttu-id="1acd7-198">パートナーの販売者は、CRM セクションで **パートナーセンターオプションとの同期** を有効にしていることを確認する必要があります。</span><span class="sxs-lookup"><span data-stu-id="1acd7-198">Partner sellers need to ensure that they have enabled **Sync with Partner Center** option in the CRM section.</span></span>

:::image type="content" source="images/cosellconnectors/enablesynch.png" alt-text="同期が有効になっていることを確認する":::

- <span data-ttu-id="1acd7-200">販売元は、潜在顧客を限定するときに収益と終了日を提供する必要があります。</span><span class="sxs-lookup"><span data-stu-id="1acd7-200">Sellers need to provide revenue and closing date when qualifying a lead.</span></span>

- <span data-ttu-id="1acd7-201">CRM ID が共同販売の機会の **作成** または **更新** ステージで提供されていても、その id を持つリードチャンスが crm に見つからない場合、update または create は無視されます。</span><span class="sxs-lookup"><span data-stu-id="1acd7-201">If CRM ID is provided in the **create** or **update** stage of co-sell opportunity, but a lead opportunity with that ID is not found in CRM, then update or create will be ignored.</span></span>

- <span data-ttu-id="1acd7-202">[紹介通貨] フィールドが Salesforce 環境で構成されていることを確認します。</span><span class="sxs-lookup"><span data-stu-id="1acd7-202">Ensure that referral currency field is configured on Salesforce environment.</span></span> 

4. <span data-ttu-id="1acd7-203">コネクタが切断され、参照の同期が失われた場合はどうすればよいですか。</span><span class="sxs-lookup"><span data-stu-id="1acd7-203">What should you do if the connector gets disconnected and you miss a referral synchronization.</span></span> 

<span data-ttu-id="1acd7-204">次に、試してみることのできるオプションをいくつか示します。</span><span class="sxs-lookup"><span data-stu-id="1acd7-204">Following are few of the options that you can try out:</span></span>

- <span data-ttu-id="1acd7-205">パートナーセンターのユーザーに対して、ユーザー名またはパスワードの有効期限が切れているかどうかを確認します。</span><span class="sxs-lookup"><span data-stu-id="1acd7-205">Check whether username or password has expired for the Partner Center user with referral admin roles.</span></span>

- <span data-ttu-id="1acd7-206">同期されていない営業案件にアクセスし、マイナー更新を行い、参照が同期されているかどうかを確認できます。</span><span class="sxs-lookup"><span data-stu-id="1acd7-206">You can go to the un-synchronized opportunity, make a minor update, and observe whether the referral has synchronized.</span></span>

- <span data-ttu-id="1acd7-207">フローが実行されて失敗した場合は、フローを選択し、失敗した実行を再送信します。</span><span class="sxs-lookup"><span data-stu-id="1acd7-207">If the flows have run and failed, then select the flow and re-submit the run which has failed.</span></span>

5. <span data-ttu-id="1acd7-208">アクセス拒否エラーが発生した場合はどうすればよいですか?</span><span class="sxs-lookup"><span data-stu-id="1acd7-208">What should you do when you get access denied errors?</span></span>

<span data-ttu-id="1acd7-209">適切なロールが存在することを確認する</span><span class="sxs-lookup"><span data-stu-id="1acd7-209">Make sure the appropriate roles exist</span></span>

- <span data-ttu-id="1acd7-210">パートナーセンターの販売者の紹介管理者ロール</span><span class="sxs-lookup"><span data-stu-id="1acd7-210">Referral Administrator role for Partner Center seller</span></span> 
 
- <span data-ttu-id="1acd7-211">CRM インスタンスのシステム管理者ロールまたはシステムカスタマイザーロール</span><span class="sxs-lookup"><span data-stu-id="1acd7-211">System Administrator or System Customizer role on your CRM instance</span></span>

- <span data-ttu-id="1acd7-212">フローアカウントのユーザーログが https://flow.microsoft.com 少なくとも事前に1回は自動で実行されていることを確認します。</span><span class="sxs-lookup"><span data-stu-id="1acd7-212">Ensure that the Power Automate flow account user logs into https://flow.microsoft.com at least once beforehand</span></span>

6. <span data-ttu-id="1acd7-213">共同販売の機会の作成中に **顧客アカウントの国コード** が不足していることがわかった場合は、どうすればよいでしょうか。</span><span class="sxs-lookup"><span data-stu-id="1acd7-213">If you see that **Customer account country code** is missing while creating a Co-sell opportunity, what should you do?</span></span>

<span data-ttu-id="1acd7-214">ISO の2文字の国コードを CRM の顧客アカウントに追加する必要があります。</span><span class="sxs-lookup"><span data-stu-id="1acd7-214">You will need to add the ISO two-letter country code to the Customer account in CRM.</span></span>

7. <span data-ttu-id="1acd7-215">共同販売の機会を作成するときに **ソリューション ID が必要** であるというエラーが表示された場合はどうすればよいですか。</span><span class="sxs-lookup"><span data-stu-id="1acd7-215">What should you do if you see the error that **Solution ID is required** while creating a Co-sell opportunity?</span></span>

<span data-ttu-id="1acd7-216">共同販売の紹介を作成するには、Microsoft 共同販売の準備ができているソリューションが必要です。</span><span class="sxs-lookup"><span data-stu-id="1acd7-216">In order to create a co-sell referral, you need a Microsoft co-sell ready solution.</span></span> 

8. <span data-ttu-id="1acd7-217">フローエラーが発生していなくても CRM に同期されていない共同販売機会がパートナーセンターで作成されている場合は、次のことを行う必要があります。</span><span class="sxs-lookup"><span data-stu-id="1acd7-217">What should you do when you see Co-sell opportunities created in Partner Center that aren't synchronized to CRM even though there are no flow errors:</span></span>

<span data-ttu-id="1acd7-218">次の操作を行います。</span><span class="sxs-lookup"><span data-stu-id="1acd7-218">Do the following:</span></span>

- <span data-ttu-id="1acd7-219">パートナーセンターで新しい共同販売取引を作成した後、パートナーセンターから Dynamics 365 へのフローが呼び出されるかどうかを確認します (複数回呼び出される可能性があります)。</span><span class="sxs-lookup"><span data-stu-id="1acd7-219">After you have created a new co-sell deal in Partner Center, check if Partner Center to Dynamics 365 flow gets invoked (it might get invoked multiple times).</span></span>

- <span data-ttu-id="1acd7-220">フローが呼び出された場合は、呼び出されたすべてのフローを確認し、CRM を更新するフロー実行を特定します。</span><span class="sxs-lookup"><span data-stu-id="1acd7-220">If the flow gets invoked, check all invoked flows, and identify the flow run which would update the CRM.</span></span> <span data-ttu-id="1acd7-221">アクションに従って操作を実行し、CRM が更新されたか、または問題が発生したかどうかを確認できます。</span><span class="sxs-lookup"><span data-stu-id="1acd7-221">You can follow the actions and verify if it did update the CRM or encountered a problem.</span></span>

- <span data-ttu-id="1acd7-222">パートナーセンターで *新しい商談*\* を確認し、CRM ID が設定されているかどうかを確認します。</span><span class="sxs-lookup"><span data-stu-id="1acd7-222">Check *New deal*\* in Partner Center to see if it gets populated with CRM ID.</span></span>

- <span data-ttu-id="1acd7-223">パートナーセンターで、取引が誤って "勝ち" または "Lost" として閉じられていないことを確認します。</span><span class="sxs-lookup"><span data-stu-id="1acd7-223">Make sure that the deal is not accidentally closed as “Won” or “Lost” in Partner Center.</span></span>

## <a name="next-steps"></a><span data-ttu-id="1acd7-224">次のステップ</span><span class="sxs-lookup"><span data-stu-id="1acd7-224">Next steps</span></span>

- [<span data-ttu-id="1acd7-225">見込み客を管理する</span><span class="sxs-lookup"><span data-stu-id="1acd7-225">Manage leads</span></span>](manage-leads.md)
 
- [<span data-ttu-id="1acd7-226">共同販売の機会を管理する</span><span class="sxs-lookup"><span data-stu-id="1acd7-226">Manage co-sell opportunities</span></span>](manage-co-sell-opportunities.md)
