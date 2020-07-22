---
title: Webhook を使用してリソース変更イベントを取得する
ms.topic: article
ms.date: 06/05/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: パートナーセンターの Webhook Api を使用して、Dynamics 365 CRM または Salesforce CRM で参照のリソースがどのように変更されるかを学習します。
author: sroy
ms.author: sroy
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: bc640e27bf3827e6a1cdbcf5b4913db62488402b
ms.sourcegitcommit: 54f823f0e02e0e7add737d78de74d8eba8d9f381
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/22/2020
ms.locfileid: "86875208"
---
# <a name="use-webhook-apis-to-register-for-resource-change-events-for-dynamics-365-crm-and-salesforce-crm"></a><span data-ttu-id="148a1-103">Webhook Api を使用して Dynamics 365 CRM と Salesforce CRM のリソース変更イベントに登録する</span><span class="sxs-lookup"><span data-stu-id="148a1-103">Use Webhook APIs to register for resource change events for Dynamics 365 CRM and Salesforce CRM</span></span>

### <a name="appropriate-roles"></a><span data-ttu-id="148a1-104">適切なロール</span><span class="sxs-lookup"><span data-stu-id="148a1-104">Appropriate roles</span></span>

- <span data-ttu-id="148a1-105">紹介管理者</span><span class="sxs-lookup"><span data-stu-id="148a1-105">Referrals admin</span></span>
- <span data-ttu-id="148a1-106">Dynamics 365 CRM または Salesforce CRM のシステム管理者またはシステムカスタマイザー</span><span class="sxs-lookup"><span data-stu-id="148a1-106">System admin or System customizer for Dynamics 365 CRM or Salesforce CRM</span></span>

<span data-ttu-id="148a1-107">パートナーセンターの Webhook Api を使用すると、リソース変更イベントに登録できます。</span><span class="sxs-lookup"><span data-stu-id="148a1-107">The Partner Center Webhook APIs allow you to register for resource change events.</span></span> <span data-ttu-id="148a1-108">これらの変更イベントは、HTTP 投稿として url に送信されます。</span><span class="sxs-lookup"><span data-stu-id="148a1-108">These change events are sent to your url as HTTP posts.</span></span>

>[!NOTE]
><span data-ttu-id="148a1-109">このトピックでは、Dynamics 365 CRM と Salesforce CRM の両方の Webhook Api について説明します。</span><span class="sxs-lookup"><span data-stu-id="148a1-109">This topic explains Webhook APIs for both Dynamics 365 CRM and Salesforce CRM.</span></span>

## <a name="configure-the-webhook"></a><span data-ttu-id="148a1-110">webhook を構成する</span><span class="sxs-lookup"><span data-stu-id="148a1-110">Configure the webhook</span></span>

1. <span data-ttu-id="148a1-111">Url を登録するには、**パートナーセンターの Webhook 登録 (Insider Preview)** パワー自動化フローを選択します。</span><span class="sxs-lookup"><span data-stu-id="148a1-111">To register your url, select **Partner Center Webhook Registration (Insider Preview)** Power Automate flow.</span></span>

2. <span data-ttu-id="148a1-112">接続の追加 (a.)参照管理者の資格情報を持つパートナーセンターのユーザー (b)次の強調表示されているパートナーセンターのイベント</span><span class="sxs-lookup"><span data-stu-id="148a1-112">Add connections for (a.) Partner Center user with referrals admin credentials (b.) Partner Center Events as highlighted below</span></span>

   :::image type="content" source="images/cosellconnectors/triggerflow.png" alt-text="トリガー":::

3. <span data-ttu-id="148a1-114">これらの更新を行うと、次のように表示されます。</span><span class="sxs-lookup"><span data-stu-id="148a1-114">When you make these updates, you will see</span></span>

   :::image type="content" source="images/cosellconnectors/webhook1.png" alt-text="Webhook":::

4. <span data-ttu-id="148a1-116">変更内容を保存し、[**有効にする**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="148a1-116">Save your changes and select **Turn on**.</span></span>

   <span data-ttu-id="148a1-117">パートナーセンターの webhook がパートナーセンターと CRM システムの IP 共同販売/独立した参照オブジェクトでイベントの変更をリッスンできるようにするには、次の手順を実行します。</span><span class="sxs-lookup"><span data-stu-id="148a1-117">To enable Partner Center webhooks to listen to event changes in the IP Co-sell/independent referral objects in Partner Center and CRM systems perform the following steps:</span></span>

5. <span data-ttu-id="148a1-118">[**パートナーセンター] を選択して Dynamics 365 (Insider preview)** または**パートナーセンターから Salesforce へ (insider preview)** を選択します。</span><span class="sxs-lookup"><span data-stu-id="148a1-118">Select **Partner Center to Dynamics 365 (Insider Preview)** or **Partner Center to Salesforce (Insider Preview)**.</span></span>

6. <span data-ttu-id="148a1-119">[**編集**] アイコンを選択し、[ **HTTP 要求の受信時**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="148a1-119">Select the **Edit** icon and select **When a HTTP request is received**.</span></span>

7. <span data-ttu-id="148a1-120">**コピー**アイコンを選択して、指定された HTTP POST URL をコピーします。</span><span class="sxs-lookup"><span data-stu-id="148a1-120">Select the **Copy** icon to copy the provided HTTP POST URL.</span></span>

   :::image type="content" source="images/cosellconnectors/copyurl.png" alt-text="URL のコピー":::

8. <span data-ttu-id="148a1-122">次に、"パートナーセンターの Webhook の登録 (Insider Preview)" パワー自動化フローを選択し、[**実行**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="148a1-122">Now select the “Partner Center Webhook Registration (Insider Preview)” Power Automate flow and select **Run**.</span></span>

9. <span data-ttu-id="148a1-123">右側のウィンドウで [実行フロー] ウィンドウが開いていることを確認し、[**続行**] をクリックします。</span><span class="sxs-lookup"><span data-stu-id="148a1-123">Ensure that the “Run Flow” window opens on the right-hand pane and click **Continue**.</span></span>

10. <span data-ttu-id="148a1-124">次の詳細を入力します。</span><span class="sxs-lookup"><span data-stu-id="148a1-124">Enter the following details:</span></span>

    1. <span data-ttu-id="148a1-125">**Http トリガーエンドポイント**: 前の手順からコピーされた URL</span><span class="sxs-lookup"><span data-stu-id="148a1-125">**Http Trigger Endpoint**: URL copied from earlier step</span></span>

    2. <span data-ttu-id="148a1-126">**登録するイベント**: "紹介-作成" と "参照-更新"</span><span class="sxs-lookup"><span data-stu-id="148a1-126">**Events to Register**: “referral-created” and “referral-updated”</span></span>

    3. <span data-ttu-id="148a1-127">**既存のトリガーエンドポイントがある場合は上書き**します (存在する場合は既存のエンドポイントを上書きします)。</span><span class="sxs-lookup"><span data-stu-id="148a1-127">**Overwrite existing trigger endpoints if present**: Yes (This overwrites any existing endpoints.)</span></span>

    <span data-ttu-id="148a1-128">Webhook は、変更 (イベントの作成と更新) をリッスンできるようになりました。</span><span class="sxs-lookup"><span data-stu-id="148a1-128">The webhook can now listen to changes (create and update events).</span></span>

11. <span data-ttu-id="148a1-129">[**実行**] を選択し、[完了] を選択し**ます。**</span><span class="sxs-lookup"><span data-stu-id="148a1-129">Select **Run** and then select **Done.**</span></span>

## <a name="customize-synchronization-steps"></a><span data-ttu-id="148a1-130">同期手順のカスタマイズ</span><span class="sxs-lookup"><span data-stu-id="148a1-130">Customize synchronization steps</span></span>

<span data-ttu-id="148a1-131">パートナーセンターと CRM システムの間で共同販売参照が同期されると、パートナーセンター PC で同期されるフィールドがここに表示されます。</span><span class="sxs-lookup"><span data-stu-id="148a1-131">When Co-sell referrals are synced between Partner Center and your CRM system, the fields that are synced on Partner Center PC are listed here.</span></span>

<span data-ttu-id="148a1-132">多くの場合、CRM システムは高度にカスタマイズされています。</span><span class="sxs-lookup"><span data-stu-id="148a1-132">Often CRM systems are highly customized.</span></span> <span data-ttu-id="148a1-133">パワー自動化フローをカスタマイズできます。</span><span class="sxs-lookup"><span data-stu-id="148a1-133">You can customize the Power Automate flows.</span></span> <span data-ttu-id="148a1-134">フィールドマッピングガイドに従って、必要に応じて、パワー自動化フローの手順に適切な変更を加えます。</span><span class="sxs-lookup"><span data-stu-id="148a1-134">Follow the field mapping guide, and if necessary, make appropriate changes in the steps of the Power Automate flows.</span></span>  <span data-ttu-id="148a1-135">Microsoft パートナーセンターから CRM へのマッピングが提供されますが、CRM 環境に基づいて、フィールドをさらにカスタマイズすることもできます。</span><span class="sxs-lookup"><span data-stu-id="148a1-135">Microsoft Partner Center to CRM mappings are provided, but based on your CRM environment, you can choose to further customize the fields.</span></span>

<span data-ttu-id="148a1-136">各パワー自動化フローの複数の手順は、ニーズに応じてカスタマイズできます。</span><span class="sxs-lookup"><span data-stu-id="148a1-136">Multiple steps of each of the Power Automate flows can be customized based on your needs.</span></span> <span data-ttu-id="148a1-137">使用可能なカスタマイズの例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="148a1-137">The following are examples of available customizations:</span></span>

1. <span data-ttu-id="148a1-138">パートナーセンターで作成または更新イベントのフィールドを CRM の参照同期にカスタマイズするには、次のようにします。</span><span class="sxs-lookup"><span data-stu-id="148a1-138">To customize the fields for the create or update events in the Partner Center to CRM referral synchronization:</span></span>

   1. <span data-ttu-id="148a1-139">[パートナーセンター] を選択して Dynamics 365 (Insider Preview) またはパートナーセンターから Salesforce へ (Insider Preview) を選択します。</span><span class="sxs-lookup"><span data-stu-id="148a1-139">Select Partner Center to Dynamics 365 (Insider Preview) or Partner Center to Salesforce (Insider Preview).</span></span>

   2. <span data-ttu-id="148a1-140">[**編集**] を選択して、パワー自動化フローを編集またはカスタマイズします。</span><span class="sxs-lookup"><span data-stu-id="148a1-140">Select **Edit** to edit/customize the Power Automate flow.</span></span>

   3. <span data-ttu-id="148a1-141">選択 **(スコープ) 潜在顧客または営業案件を同期**します。</span><span class="sxs-lookup"><span data-stu-id="148a1-141">Select **(Scope) Synchronize the lead or opportunity**.</span></span>

2. <span data-ttu-id="148a1-142">イベントの作成用に (フィールドマッピングガイドに基づいて) CRM フィールドマッピングをカスタマイズするには、[**新しい共有の営業案件]、[] の順**に選択します。</span><span class="sxs-lookup"><span data-stu-id="148a1-142">To customize CRM field mappings (based on field mappings guide) for create events, select **If it’s new Shared opportunity, then**.</span></span> <span data-ttu-id="148a1-143">[サブステップ**if]** を選択し、 **CRM で [新しい営業案件の作成**] を展開します。</span><span class="sxs-lookup"><span data-stu-id="148a1-143">Select the substep **if yes** and then expand **Creating a new opportunity in the CRM**.</span></span> <span data-ttu-id="148a1-144">このセクションでマッピングを編集するには、[フィールドマッピングガイド] を使用します。</span><span class="sxs-lookup"><span data-stu-id="148a1-144">You can edit the mappings in this section using the Field Mapping Guide.</span></span>

   1. <span data-ttu-id="148a1-145">更新イベントの CRM フィールドマッピングをカスタマイズする (フィールドマップガイドに基づく) 場合は、"(スコープ) 潜在顧客または営業案件の同期" ステップをクリックします。</span><span class="sxs-lookup"><span data-stu-id="148a1-145">For customizing CRM field mappings (based on field mappings guide) for update events, click on the step “(Scope) Synchronize the lead or opportunity”.</span></span>

   2. <span data-ttu-id="148a1-146">**営業案件の更新である場合は、** を選択します。</span><span class="sxs-lookup"><span data-stu-id="148a1-146">Select **If it’s an update to an opportunity, then**.</span></span> <span data-ttu-id="148a1-147">[サブステップ**if yes]** を選択し、次に**パートナーセンターと CRM の営業案件オブジェクト間の差異がある場合**は、を展開します。</span><span class="sxs-lookup"><span data-stu-id="148a1-147">Select the substep **if yes** and then expand **If difference between the opportunity objects in Partner Center and CRM, then**.</span></span>  

   3. <span data-ttu-id="148a1-148">**既存の営業案件を更新**する場合は、[**はい]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="148a1-148">Select **If yes** followed with **Update existing opportunity**</span></span>

3. <span data-ttu-id="148a1-149">更新イベントの CRM から PC への参照同期のフィールドをカスタマイズするには、次のようにします。</span><span class="sxs-lookup"><span data-stu-id="148a1-149">To customize the fields for CRM to PC referral synchronization for update events:</span></span>

   1. <span data-ttu-id="148a1-150">[**編集**] を選択して、パワー自動化フローを編集またはカスタマイズします。</span><span class="sxs-lookup"><span data-stu-id="148a1-150">Select **Edit**  to edit/customize the Power Automate flow.</span></span>

   2. <span data-ttu-id="148a1-151">[ **(スコープ)] を選択して、営業案件を同期**します。</span><span class="sxs-lookup"><span data-stu-id="148a1-151">Select **(Scope) Synchronize the opportunity**.</span></span>

   3. <span data-ttu-id="148a1-152">更新イベントの CRM フィールドマッピング (フィールドマッピングガイドに基づく) をカスタマイズする場合は、**パートナーセンターと CRM の潜在顧客オブジェクトが異なるかどうか**を選択してから、を選択します。</span><span class="sxs-lookup"><span data-stu-id="148a1-152">For customizing CRM field mappings (based on field mappings guide) for update events, select **If there is difference between the lead objects in Partner Center and CRM, then**.</span></span>

   4. <span data-ttu-id="148a1-153">[サブステップ**if yes]** を選択し、[**営業案件データを使用して紹介を更新する**] ステップを展開します。</span><span class="sxs-lookup"><span data-stu-id="148a1-153">Select the substep **if yes** and then expand the step **Update a referral with opportunity data**.</span></span>

   <span data-ttu-id="148a1-154">このセクションのマッピングは、フィールドマッピングガイドに基づいて編集できます。</span><span class="sxs-lookup"><span data-stu-id="148a1-154">You can edit the mappings in this section based on the Field Mapping Guide.</span></span>

4. <span data-ttu-id="148a1-155">Create events の CRM to PC 参照同期のフィールドをカスタマイズするには</span><span class="sxs-lookup"><span data-stu-id="148a1-155">To customize the fields for CRM to PC referral synchronization for create events?</span></span>

   1. <span data-ttu-id="148a1-156">[**編集**] を選択して、パワー自動化フローを編集またはカスタマイズします。</span><span class="sxs-lookup"><span data-stu-id="148a1-156">Select **Edit**  to edit/customize the Power Automate flow.</span></span>

   2. <span data-ttu-id="148a1-157">**参照の同期を選択 (スコープ) します。**</span><span class="sxs-lookup"><span data-stu-id="148a1-157">Select **(Scope) Synchronizing Referrals.**</span></span>

   3. <span data-ttu-id="148a1-158">[イベントの作成] で (フィールドマッピングガイドに基づいて) CRM フィールドマッピングをカスタマイズする場合は、[ **Microsoft の紹介を作成する**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="148a1-158">For customizing CRM field mappings (based on field mappings guide) for create events, select **Create Microsoft Referral**.</span></span>

<span data-ttu-id="148a1-159">このセクションのマッピングは、フィールドマッピングガイドに基づいて編集できます。</span><span class="sxs-lookup"><span data-stu-id="148a1-159">You can edit the mappings in this section based on the Field Mapping Guide.</span></span>

## <a name="end-to-end-bi-directional-co-sell-referral-synchronization"></a><span data-ttu-id="148a1-160">エンドツーエンドの双方向の共同販売参照の同期</span><span class="sxs-lookup"><span data-stu-id="148a1-160">End-to-End Bi-directional Co-sell Referral Synchronization</span></span>

<span data-ttu-id="148a1-161">パワー自動化ソリューションのインストール、構成、およびカスタマイズが完了したら、Dynamics 365 または Salesforce とパートナーセンター間の共同販売参照の同期をテストできます。</span><span class="sxs-lookup"><span data-stu-id="148a1-161">Once you have installed, configured, and customized the Power Automate solution, you can test for Co-sell referrals synchronization between Dynamics 365 or Salesforce and Partner Center.</span></span>

### <a name="pre-requisites"></a><span data-ttu-id="148a1-162">前提条件</span><span class="sxs-lookup"><span data-stu-id="148a1-162">Pre-requisites</span></span>

<span data-ttu-id="148a1-163">パートナーセンターと Dynamics 365 CRM 間、またはパートナーセンターと Salesforce CRM 間で紹介を同期するには、Power 区別のソリューションで、Microsoft 固有の紹介フィールドを明確にする必要があります。</span><span class="sxs-lookup"><span data-stu-id="148a1-163">To synchronize the referrals across Partner Center and Dynamics 365 CRM or across Partner Center and Salesforce CRM, the Power Automate solution needs to clearly demarcate Microsoft-specific referral fields.</span></span> <span data-ttu-id="148a1-164">これにより、販売者チームは、共同販売のために Microsoft と共有する参照を決定することができます。</span><span class="sxs-lookup"><span data-stu-id="148a1-164">This provides your seller teams with the ability to decide which referrals they want to share with Microsoft for co-selling.</span></span>

<span data-ttu-id="148a1-165">Dynamics 365 ソリューションの**営業案件**エンティティのパートナーセンターの紹介同期の一部として、一連のカスタムフィールドを使用できます。</span><span class="sxs-lookup"><span data-stu-id="148a1-165">A set of custom fields is available as part of Partner Center Referrals Synchronization for Dynamics 365 solution **Opportunity** entity.</span></span> <span data-ttu-id="148a1-166">CRM 管理者ユーザーは、**営業案件**のカスタムフィールドを使用して、別の crm セクションを作成する必要があります。</span><span class="sxs-lookup"><span data-stu-id="148a1-166">A CRM admin user will need to create a separate CRM section with the **Opportunity** custom fields.</span></span>

<span data-ttu-id="148a1-167">次のカスタムフィールドは、CRM セクションの一部にする必要があります。</span><span class="sxs-lookup"><span data-stu-id="148a1-167">The following custom fields should be part of the CRM section:</span></span>

- <span data-ttu-id="148a1-168">**パートナーセンターとの同期**: 営業案件を Microsoft パートナーセンターと同期するかどうか</span><span class="sxs-lookup"><span data-stu-id="148a1-168">**Sync with Partner Center**: Whether to sync the opportunity with Microsoft Partner Center</span></span>

- <span data-ttu-id="148a1-169">**参照識別子**: Microsoft パートナーセンターの紹介の読み取り専用識別子フィールド</span><span class="sxs-lookup"><span data-stu-id="148a1-169">**Referral Identifier**: A read-only identifier field for Microsoft Partner Center referral</span></span>

- <span data-ttu-id="148a1-170">**紹介リンク**: Microsoft パートナーセンターでの紹介への読み取り専用リンク</span><span class="sxs-lookup"><span data-stu-id="148a1-170">**Referral Link**: A read-only link to the referral in Microsoft Partner Center</span></span>

- <span data-ttu-id="148a1-171">Microsoft の**ヘルプ**を参照してください。</span><span class="sxs-lookup"><span data-stu-id="148a1-171">**How can Microsoft help?**: Help required from Microsoft for the referral</span></span>

- <span data-ttu-id="148a1-172">**製品**: この営業案件に関連付けられている製品の一覧</span><span class="sxs-lookup"><span data-stu-id="148a1-172">**Products**: List of products associated with this opportunity</span></span>

- <span data-ttu-id="148a1-173">**監査**: パートナーセンターの紹介と同期するための読み取り専用の監査証跡</span><span class="sxs-lookup"><span data-stu-id="148a1-173">**Audit**: A read-only audit trail for syncing with Partner Center referrals</span></span>

### <a name="scenarios"></a><span data-ttu-id="148a1-174">モデル</span><span class="sxs-lookup"><span data-stu-id="148a1-174">SCENARIOS:</span></span>

1. <span data-ttu-id="148a1-175">CRM で参照が作成または更新され、パートナーセンターで同期される場合の参照の同期:</span><span class="sxs-lookup"><span data-stu-id="148a1-175">Referral synchronization when referral is created or updated in CRM and synced in Partner Center:</span></span>

   1. <span data-ttu-id="148a1-176">CRM の**営業案件**セクションで可視性を持つユーザーを使用して、DYNAMICS 365 CRM 環境にサインインします。</span><span class="sxs-lookup"><span data-stu-id="148a1-176">Sign into your Dynamics 365 CRM environment with user who has visibility in the **Opportunity** section of the CRM.</span></span>

   2. <span data-ttu-id="148a1-177">Dynamics 365 環境で "新しい営業案件" を作成するときに、次のセクションが存在することを確認します。</span><span class="sxs-lookup"><span data-stu-id="148a1-177">Ensure that the following section is present when you create a “New Opportunity” in Dynamics 365 environment</span></span>

      :::image type="content" source="images/cosellconnectors/opportunity.png" alt-text="営業の機会":::

   3. <span data-ttu-id="148a1-179">この機会を Microsoft パートナーセンターと同期するには、カードビューで次のフィールドを設定していることを確認します。</span><span class="sxs-lookup"><span data-stu-id="148a1-179">To synchronize this opportunity with Microsoft Partner Center, ensure that you set the following fields in the card view:</span></span>

      - <span data-ttu-id="148a1-180">**パートナーセンターとの同期**: はい</span><span class="sxs-lookup"><span data-stu-id="148a1-180">**Sync with Partner Center**: Yes</span></span>

      - <span data-ttu-id="148a1-181">**Microsoft のヘルプを使用する方法**: 次から選択してください。</span><span class="sxs-lookup"><span data-stu-id="148a1-181">**How can Microsoft help?**: Select from the following:</span></span>

         :::image type="content" source="images/cosellconnectors/help.png" alt-text="ヘルプの選択":::

      - <span data-ttu-id="148a1-183">**製品**: 製品のソリューション id</span><span class="sxs-lookup"><span data-stu-id="148a1-183">**Products**: Solution IDs of the product</span></span>

   4. <span data-ttu-id="148a1-184">営業案件が Dynamics 365 で作成され、[**パートナーセンターとの同期**] オプションを **[はい]** に設定した場合は、10分間待機して、パートナーセンターアカウントにサインインします。</span><span class="sxs-lookup"><span data-stu-id="148a1-184">Once the opportunity is created in Dynamics 365 with **Sync with Partner Center** option set to **Yes**, wait 10 minutes, sign into your Partner Center account.</span></span> <span data-ttu-id="148a1-185">参照は Dynamics 365 と同期されます。</span><span class="sxs-lookup"><span data-stu-id="148a1-185">Your referrals will be synchronized with Dynamics 365.</span></span>

   5. <span data-ttu-id="148a1-186">そのため、[パートナーセンターとの同期] オプションを [はい] に設定した場合、Dynamics 365 CRM で営業案件を更新すると、パートナーセンターアカウントで変更が同期されます。</span><span class="sxs-lookup"><span data-stu-id="148a1-186">Consequently, for an opportunity that had “Sync with Partner Center” option set to “Yes”, if you update the opportunity in Dynamics 365 CRM, the changes will be synchronized in your Partner Center account.</span></span>

   6. <span data-ttu-id="148a1-187">パートナーセンターで正常に同期された営業案件は、Dynamics 365 の✔アイコンで識別されます。</span><span class="sxs-lookup"><span data-stu-id="148a1-187">Opportunities that are synchronized successfully with Partner Center will be identified with ✔icon in Dynamics 365.</span></span>

2. <span data-ttu-id="148a1-188">Microsoft パートナーセンターで参照が作成または更新され、Dynamics 365 環境で同期される場合の参照同期:</span><span class="sxs-lookup"><span data-stu-id="148a1-188">Referral Synchronization when referral is created or updated in Microsoft Partner Center and synchronized in Dynamics 365 environment:</span></span>

   1. <span data-ttu-id="148a1-189">パートナーセンターの[ダッシュボード](https://partner.microsoft.com/dashboard/home)にサインインします。</span><span class="sxs-lookup"><span data-stu-id="148a1-189">Sign into your Partner Center [dashboard](https://partner.microsoft.com/dashboard/home).</span></span>

   2. <span data-ttu-id="148a1-190">左側のメニューから [**紹介**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="148a1-190">Select **Referrals** from the left-hand menu.</span></span>

   3. <span data-ttu-id="148a1-191">[新しい取引] オプションをクリックして、パートナーセンターから新しい共同販売紹介を作成します。</span><span class="sxs-lookup"><span data-stu-id="148a1-191">Create a new Co-sell referral from Partner Center by clicking “New deal” option.</span></span>

   4. <span data-ttu-id="148a1-192">Dynamics 365 CRM 環境にサインインします。</span><span class="sxs-lookup"><span data-stu-id="148a1-192">Sign into your Dynamics 365 CRM environment.</span></span>

   5. <span data-ttu-id="148a1-193">**[Open opportunity**] に移動します。</span><span class="sxs-lookup"><span data-stu-id="148a1-193">Navigate to **Open Opportunities**.</span></span> <span data-ttu-id="148a1-194">Microsoft パートナーセンターで作成された紹介が Dynamics 365 CRM で同期されるようになりました。</span><span class="sxs-lookup"><span data-stu-id="148a1-194">The referral created in Microsoft Partner Center is now synchronized in Dynamics 365 CRM.</span></span>

   6. <span data-ttu-id="148a1-195">同期された参照を選択すると、カードビューの詳細が設定されます。</span><span class="sxs-lookup"><span data-stu-id="148a1-195">When you select a synchronized referral, the card view details are populated.</span></span>

## <a name="next-steps"></a><span data-ttu-id="148a1-196">次のステップ</span><span class="sxs-lookup"><span data-stu-id="148a1-196">Next steps</span></span>

- [<span data-ttu-id="148a1-197">Microsoft Power の自動化プラットフォームの詳細</span><span class="sxs-lookup"><span data-stu-id="148a1-197">More about Microsoft Power Automate platform?</span></span>](https://docs.microsoft.com/power-automate/)

- [<span data-ttu-id="148a1-198">パートナーセンターの webhook イベント</span><span class="sxs-lookup"><span data-stu-id="148a1-198">Partner Center webhook events</span></span>](https://docs.microsoft.com/partner-center/develop/partner-center-webhook-events)

- [<span data-ttu-id="148a1-199">見込み客を管理する</span><span class="sxs-lookup"><span data-stu-id="148a1-199">Manage leads</span></span>](manage-leads.md)

- [<span data-ttu-id="148a1-200">共同販売の機会を管理する</span><span class="sxs-lookup"><span data-stu-id="148a1-200">Manage co-sell opportunities</span></span>](manage-co-sell-opportunities.md)
