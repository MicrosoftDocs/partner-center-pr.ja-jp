---
title: ダイレクト請求パートナーを間接リセラーに切り替える
ms.topic: article
ms.date: 06/05/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: CSP プログラムパートナーがパートナーセンターを使用して、直接請求パートナーから間接リセラーに移行する方法について説明します。
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
keywords: 直接請求, 移行, 間接リセラー
ms.custom: SEOMAY.20
ms.openlocfilehash: f3f87014e76ea32bf15d3e0147d5e40c3a5ebefc
ms.sourcegitcommit: 775a13540d6576201a900e517a0696a6ff4897d8
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/05/2020
ms.locfileid: "84458408"
---
# <a name="transition-from-cloud-solution-provider-csp-direct-bill-partner-to-csp-indirect-reseller"></a><span data-ttu-id="83679-104">クラウド ソリューション プロバイダー (CSP) 直接請求パートナーから CSP 間接リセラーへの移行</span><span class="sxs-lookup"><span data-stu-id="83679-104">Transition from Cloud Solution Provider (CSP) direct bill partner to CSP indirect reseller</span></span>

<span data-ttu-id="83679-105">**適用対象:**</span><span class="sxs-lookup"><span data-stu-id="83679-105">**Applies to:**</span></span>

- <span data-ttu-id="83679-106">CSP パートナー</span><span class="sxs-lookup"><span data-stu-id="83679-106">CSP partners</span></span>

>[!Note]
><span data-ttu-id="83679-107">この記事は、間接リセラーに移行することに決めた直接請求パートナーのためのものです。</span><span class="sxs-lookup"><span data-stu-id="83679-107">This article is intended for direct bill partners who have decided to transition to indirect resellers.</span></span> <span data-ttu-id="83679-108">ただし、間接リセラーとして登録するための明示的な決定をまだ行っていない場合でも、CSP direct bill partner プログラムの新しい[要件](direct-partner-new-requirements.md)を満たしていない直接請求先のパートナーは、[直接請求書の機能が制限さ](restricted-direct-bill-capabilities.md)れるときに Microsoft によって通知されます。</span><span class="sxs-lookup"><span data-stu-id="83679-108">However, even if you have not made an explicit decision yet to enroll as an indirect reseller, direct bill partners who do not meet the new [requirements](direct-partner-new-requirements.md) for the CSP direct bill partner program will be informed by Microsoft when their [direct bill capabilities will be restricted](restricted-direct-bill-capabilities.md).</span></span>

<span data-ttu-id="83679-109">パートナーは、既存の直接請求テナントを使用して間接リセラー プログラムに登録できます。</span><span class="sxs-lookup"><span data-stu-id="83679-109">You will be able to enroll in the indirect reseller program using your existing direct bill tenant.</span></span>

## <a name="get-started"></a><span data-ttu-id="83679-110">作業開始</span><span class="sxs-lookup"><span data-stu-id="83679-110">Get started</span></span>

1. <span data-ttu-id="83679-111">パートナー センターのパートナー プロファイルと MPN ID が最新の状態であることを確認します。</span><span class="sxs-lookup"><span data-stu-id="83679-111">Make sure your partner profile in Partner Center and MPN ID are current.</span></span>

2. <span data-ttu-id="83679-112">間接リセラーに移行する直接請求テナントのグローバル管理者としてパートナー センターにサインインします。</span><span class="sxs-lookup"><span data-stu-id="83679-112">Sign in to Partner Center as the global admin for the direct bill tenant you are transitioning to indirect reseller.</span></span>

   :::image type="content" source="images/direct/direct1.png" alt-text="概要":::

3. <span data-ttu-id="83679-114">登録フォームでパートナーの詳細を確認します。</span><span class="sxs-lookup"><span data-stu-id="83679-114">Review your partner details on the enrollment form.</span></span>

   :::image type="content" source="images/direct/direct2a.png" alt-text="今すぐ登録":::

4. <span data-ttu-id="83679-116">[Enroll now]\(今すぐ登録\) を選択します。</span><span class="sxs-lookup"><span data-stu-id="83679-116">Select Enroll now.</span></span> <span data-ttu-id="83679-117">間接リセラー ビジネスでは、直接ビジネスに使用しているものと同じ AAD テナントを使います。</span><span class="sxs-lookup"><span data-stu-id="83679-117">Your indirect reseller business will use the same AAD tenant you use for your direct business.</span></span>

    > [!NOTE]
    > <span data-ttu-id="83679-118">最初は、この新しい移行機能は、契約応当日が 9 月から 12 月までのパートナーが利用できます。</span><span class="sxs-lookup"><span data-stu-id="83679-118">Initially, this new transition capability will be available for partners with September to December anniversary dates.</span></span> <span data-ttu-id="83679-119">契約応当日が 9 月から 12 月の間にない場合、現時点では機能が表示されません。</span><span class="sxs-lookup"><span data-stu-id="83679-119">If you don"t have an anniversary date between September and December, you won't see the capability at this time.</span></span> <span data-ttu-id="83679-120">契約応当日が 2018 年 12 月以降のパートナーは、今後パートナー向けに機能が有効になった時点で通知されます。</span><span class="sxs-lookup"><span data-stu-id="83679-120">Partners with anniversary dates after December 2018 will be notified later once the feature is enabled for the partners.</span></span>

5. <span data-ttu-id="83679-121">登録が承認されたら、パートナー センターにもう一度サインインします。</span><span class="sxs-lookup"><span data-stu-id="83679-121">When your enrollment is approved, sign in to Partner Center again.</span></span>

    > [!NOTE]
    > <span data-ttu-id="83679-122">通常であればすぐに承認されますが、最大で 5 営業日かかることがあります。</span><span class="sxs-lookup"><span data-stu-id="83679-122">While approval is usually immediate, it can take up to five business days.</span></span> <span data-ttu-id="83679-123">承認が済むと、登録フォームで主要連絡先に指定したメール アドレスに通知が届きます。</span><span class="sxs-lookup"><span data-stu-id="83679-123">Once approved, you will receive a notification to the email address you have specified under primary contact in the enrollment form.</span></span> <span data-ttu-id="83679-124">また、[**設定**] [  >  **パートナー設定**] [  >  **パートナープロファイル**] > [プログラム情報] で、登録の状態を確認することもできます。</span><span class="sxs-lookup"><span data-stu-id="83679-124">You can also check your enrollment status under **Settings** > **Partner Settings** > **Partner Profile** > Program info.</span></span>

6. <span data-ttu-id="83679-125">**[概要]** ページに、間接リセラー契約が表示されます。</span><span class="sxs-lookup"><span data-stu-id="83679-125">On your **Overview** page, you will see the indirect reseller agreement.</span></span> <span data-ttu-id="83679-126">**[Accept and continue] (同意して続ける)** を選びます。</span><span class="sxs-lookup"><span data-stu-id="83679-126">Select **Accept and continue**.</span></span> <span data-ttu-id="83679-127">この操作により、間接リセラーの機能が有効になります。</span><span class="sxs-lookup"><span data-stu-id="83679-127">This action enables the indirect reseller capabilities.</span></span>

<span data-ttu-id="83679-128">間接リセラー契約を受け入れるときは、パートナー プロファイルでは直接請求パートナーと間接リセラーの**両方**として示されていることに注意してください。</span><span class="sxs-lookup"><span data-stu-id="83679-128">When you have accepted the indirect reseller agreement, notice that your Partner profile identifies you as **both** a direct bill and indirect reseller.</span></span>

:::image type="content" source="images/direct/direct3.png" alt-text="間接リセラー契約":::

> [!IMPORTANT]
> <span data-ttu-id="83679-130">新しい機能を使用して間接リセラーとして登録した後は、直接請求のみのテナントにロールバックするオプションはありません。</span><span class="sxs-lookup"><span data-stu-id="83679-130">Once you enroll as an indirect reseller using the new capability, there is no option to roll back to a direct bill- only tenant.</span></span> <span data-ttu-id="83679-131">間接リセラーとして登録する前に、ビジネス ニーズを完全に評価していることを確認してください。</span><span class="sxs-lookup"><span data-stu-id="83679-131">Please make sure that you fully evaluate your business needs before enrolling as an indirect reseller.</span></span>

## <a name="while-you-transition-from-direct-to-indirect-reseller"></a><span data-ttu-id="83679-132">直接パートナーから間接リセラーへの移行中</span><span class="sxs-lookup"><span data-stu-id="83679-132">While you transition from direct to indirect reseller</span></span>

<span data-ttu-id="83679-133">このフェーズでは、課金プロセスを含め、お客様の直接のサブスクリプションのニーズを引き続き管理します。</span><span class="sxs-lookup"><span data-stu-id="83679-133">During this phase, you will continue to manage your direct customers' subscription needs including the billing process.</span></span> <span data-ttu-id="83679-134">同時に、間接プロバイダーからの顧客の受け入れを開始し、間接リセラーとして活動することもできます。</span><span class="sxs-lookup"><span data-stu-id="83679-134">You can also begin accepting customers from your Indirect provider and operating as an indirect reseller.</span></span>

:::image type="content" source="images/direct/direct4.png" alt-text="パートナーは、直接請求パートナーと間接リセラーの両方である":::

## <a name="find-an-indirect-provider"></a><span data-ttu-id="83679-136">間接プロバイダーの検索</span><span class="sxs-lookup"><span data-stu-id="83679-136">Find an indirect provider</span></span>

<span data-ttu-id="83679-137">登録が済むと、左側のナビゲーションに間接プロバイダーへのリンクが表示されます。</span><span class="sxs-lookup"><span data-stu-id="83679-137">After enrolling, a link to Indirect providers will appear in your left nav.</span></span> <span data-ttu-id="83679-138">間接リセラーとしてパートナーは、間接プロバイダーとの関係を確立し、その後は間接プロバイダーが、請求を処理し、顧客の製品を購入し、インフラストラクチャをサポートすることができます。</span><span class="sxs-lookup"><span data-stu-id="83679-138">As an indirect reseller you will establish a relationship with an indirect provider who then can handle your billing, purchase products for your customers, and support infrastructure.</span></span>

<span data-ttu-id="83679-139">提供されるサポートやサービスは間接プロバイダーによって異なるため、リセラーは対象地域の複数のプロバイダーを評価して、自社のニーズに最も適したプロバイダーを判断する必要があります。</span><span class="sxs-lookup"><span data-stu-id="83679-139">Different indirect providers offer different support and services, so you should evaluate the providers in your area to determine which ones best meet your needs.</span></span> <span data-ttu-id="83679-140">一般に、ほとんどのプロバイダーが提供している機能は次のとおりです。</span><span class="sxs-lookup"><span data-stu-id="83679-140">Generally, most providers will:</span></span>

- <span data-ttu-id="83679-141">リセラーへのテクニカル サポートの提供</span><span class="sxs-lookup"><span data-stu-id="83679-141">Provide you with technical training and assistance</span></span>
- <span data-ttu-id="83679-142">リセラーの製品やサービスのマーケティング支援</span><span class="sxs-lookup"><span data-stu-id="83679-142">Help you market your products and services</span></span>
- <span data-ttu-id="83679-143">財務および与信条件を管理する</span><span class="sxs-lookup"><span data-stu-id="83679-143">Manage your financing and credit terms</span></span>

<span data-ttu-id="83679-144">公式な [Microsoft 間接プロバイダー](https://partnercenter.microsoft.com/partner/find-a-provider)の一覧を検索してください。</span><span class="sxs-lookup"><span data-stu-id="83679-144">Search the list of official [Microsoft indirect providers](https://partnercenter.microsoft.com/partner/find-a-provider).</span></span>

<span data-ttu-id="83679-145">詳しくは、[間接プロバイダーとの提携](indirect-reseller-tasks-in-partner-center.md)に関する記事をご覧ください</span><span class="sxs-lookup"><span data-stu-id="83679-145">Learn more, read  [Partner with indirect providers](indirect-reseller-tasks-in-partner-center.md)</span></span>

## <a name="accept-a-partnership-invitation-from-your-indirect-provider"></a><span data-ttu-id="83679-146">間接プロバイダーからのパートナーシップへの招待を受け入れる</span><span class="sxs-lookup"><span data-stu-id="83679-146">Accept a partnership invitation from your indirect provider</span></span>

<span data-ttu-id="83679-147">提携する間接プロバイダーが見つかったら、パートナー センターで間接プロバイダーとのパートナーシップを確立します。</span><span class="sxs-lookup"><span data-stu-id="83679-147">When you find an indirect provider to partner with, establish a partnership with the indirect provider in Partner Center.</span></span>

<span data-ttu-id="83679-148">選択した間接プロバイダーから、パートナー センターで招待に移動するパートナーシップ招待リンクがメールで送られてきます。</span><span class="sxs-lookup"><span data-stu-id="83679-148">The indirect provider you select will send you in email a partnership invitation link that will take you to their invitation in Partner Center.</span></span> <span data-ttu-id="83679-149">必ず、グローバル管理者がパートナー センターにサインインして、招待リンクに従います。</span><span class="sxs-lookup"><span data-stu-id="83679-149">Be sure your global admin signs in to Partner Center and follows the invitation link.</span></span> <span data-ttu-id="83679-150">招待を受け入れると、プロバイダーの名前が間接プロバイダーの一覧に表示されます。</span><span class="sxs-lookup"><span data-stu-id="83679-150">When you accept the invitation, the provider's name will appear in your indirect provider list.</span></span>

## <a name="acquire-new-customers-as-indirect-reseller"></a><span data-ttu-id="83679-151">間接リセラーとして新しい顧客を獲得する</span><span class="sxs-lookup"><span data-stu-id="83679-151">Acquire new customers as indirect reseller</span></span>

<span data-ttu-id="83679-152">間接リセラーと間接プロバイダーの両方が、顧客との間にリセラーの関係を持つ必要があります。</span><span class="sxs-lookup"><span data-stu-id="83679-152">Both you and your indirect provider need to have reseller relationships with customers.</span></span> <span data-ttu-id="83679-153">これらの再販業者の関係により、顧客のサブスクリプションとサービスをユーザーの代理として管理することができます。</span><span class="sxs-lookup"><span data-stu-id="83679-153">These reseller relationships enable you to manage a customer's subscriptions and services on their behalf.</span></span> <span data-ttu-id="83679-154">既存の Azure AD テナントを持つ新しい顧客を獲得するには、貴社と貴社のプロバイダーの両方と同時にリセラーの関係を確立するよう、顧客を招待できます。</span><span class="sxs-lookup"><span data-stu-id="83679-154">To acquire a new customer who has an existing Azure AD tenant, you can invite the customer to establish a reseller relationship with both you and your provider at the same time.</span></span>

<span data-ttu-id="83679-155">間接リセラーの招待を作成するには:</span><span class="sxs-lookup"><span data-stu-id="83679-155">To create an indirect reseller invitation:</span></span>

1. <span data-ttu-id="83679-156">パートナー センターの左側のナビゲーションから **[間接プロバイダー]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="83679-156">Select **Indirect providers** from your Partner Center left nav.</span></span>

2. <span data-ttu-id="83679-157">貴社と間接プロバイダーの両方について再販業者関係を確立するために新しい顧客を招待するには、 **[新しい顧客を招待する]** を選びます。</span><span class="sxs-lookup"><span data-stu-id="83679-157">Select **Invite new customers** to invite a customer to establish a reseller relationship with both you and the indirect provider at the same time.</span></span> <span data-ttu-id="83679-158">プロバイダーは顧客との再販業者関係を持っている必要があるため、顧客が新しいサブスクリプションを購入したり、既存のサブスクリプションに新しいライセンスを追加したりするときに、顧客に代わって注文を送信することができます。</span><span class="sxs-lookup"><span data-stu-id="83679-158">The provider needs to have a reseller relationship with your customer, so they can submit orders on your customer's behalf when the customer wants to buy new subscriptions or add new licenses to existing subscriptions.</span></span>

3. <span data-ttu-id="83679-159">次のページで、メール メッセージの下書きを確認します。</span><span class="sxs-lookup"><span data-stu-id="83679-159">On the next page, review the draft email message.</span></span> <span data-ttu-id="83679-160">メールで下書きメッセージを開くか、メッセージをクリップボードにコピーし、メールに貼り付けます。</span><span class="sxs-lookup"><span data-stu-id="83679-160">You can open the draft message in email, or you can copy the message to your clipboard and paste it into an email.</span></span>

4. <span data-ttu-id="83679-161">電子メールのテキストを編集して必要なものを指定しますが、自分のアカウントとプロバイダーのアカウントの両方に顧客を直接接続できるように、パーソナライズされたリンクを含めてください。</span><span class="sxs-lookup"><span data-stu-id="83679-161">Edit the text in the email to say what you need but be sure to include the link as it is personalized to connect the customer directly to both your account and your provider's account.</span></span> <span data-ttu-id="83679-162">**[完了]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="83679-162">Then select **Done**.</span></span>

5. <span data-ttu-id="83679-163">顧客が貴社とプロバイダーを指名リセラーとして承認すると、貴社には顧客のサブスクリプション、ライセンス、ユーザーを管理するための管理者のアクセス許可が付与され、間接プロバイダーは、顧客に代わって注文を送信できるようになります。</span><span class="sxs-lookup"><span data-stu-id="83679-163">After the customer authorizes you and your provider to be their resellers of record, you'll have administrator permissions to manage their subscriptions, licenses, and users on their behalf, and your indirect provider will be able to submit orders on their behalf.</span></span>
6. <span data-ttu-id="83679-164">顧客のアカウント、サービス、ユーザー、ライセンスを管理するには、顧客の名前の下矢印を選んで、顧客のレコードを展開します。</span><span class="sxs-lookup"><span data-stu-id="83679-164">To manage the customer's account, services, users, and licenses, expand the customer's record by selecting the down arrow near their name.</span></span>

<span data-ttu-id="83679-165">ダイレクト請求パートナーとは異なり、間接リセラーは、パートナーセンターで新しい顧客用に Azure AD テナントを作成することはできません。</span><span class="sxs-lookup"><span data-stu-id="83679-165">Unlike direct bill partners, indirect resellers can't create Azure AD tenants for their new customers in Partner Center.</span></span> <span data-ttu-id="83679-166">プロバイダーがテナントを作成し、この顧客に対する間接リセラーとして貴社を指定します。</span><span class="sxs-lookup"><span data-stu-id="83679-166">Your provider will create the tenant and will specify you as the indirect reseller for this customer.</span></span> <span data-ttu-id="83679-167">これにより、顧客がパートナー センターの顧客リストに表示されます。</span><span class="sxs-lookup"><span data-stu-id="83679-167">This ensures that the customer will appear in your customer list in Partner Center.</span></span>

>[!Note]
><span data-ttu-id="83679-168">貴社は、直接請求機能を使用して、間接リセラーとして獲得した顧客の購入を作成することはできません。</span><span class="sxs-lookup"><span data-stu-id="83679-168">You will not be able to use your direct bill capability to create purchases for customers you acquire as an indirect reseller.</span></span>

## <a name="managing-your-direct-bill-customers-and-your-indirect-reseller-customers"></a><span data-ttu-id="83679-169">直接請求の顧客と間接リセラーの顧客を管理する</span><span class="sxs-lookup"><span data-stu-id="83679-169">Managing your direct bill customers and your indirect reseller customers</span></span>

<span data-ttu-id="83679-170">直接請求の顧客の管理と、間接リセラーの顧客の管理は異なります。</span><span class="sxs-lookup"><span data-stu-id="83679-170">You manage your direct bill customers and your indirect reseller customers differently.</span></span>

### <a name="direct-bill-customers-things-you-wont-do-as-an-indirect-reseller"></a><span data-ttu-id="83679-171">ダイレクト請求顧客 (間接リセラーとしては実行されません)</span><span class="sxs-lookup"><span data-stu-id="83679-171">Direct bill customers (things you won't do as an indirect reseller)</span></span>

- <span data-ttu-id="83679-172">製品の注文を作成します</span><span class="sxs-lookup"><span data-stu-id="83679-172">Create orders for products</span></span>
- <span data-ttu-id="83679-173">Azure の予約の管理</span><span class="sxs-lookup"><span data-stu-id="83679-173">Manage Azure reservations</span></span>
- <span data-ttu-id="83679-174">注文履歴を管理します</span><span class="sxs-lookup"><span data-stu-id="83679-174">Manage their order history</span></span>
- <span data-ttu-id="83679-175">ソフトウェアを購入します</span><span class="sxs-lookup"><span data-stu-id="83679-175">Purchase software</span></span>
- <span data-ttu-id="83679-176">顧客に直接請求します</span><span class="sxs-lookup"><span data-stu-id="83679-176">Bill customers directly</span></span>

### <a name="indirect-reseller-customers"></a><span data-ttu-id="83679-177">間接リセラーの顧客</span><span class="sxs-lookup"><span data-stu-id="83679-177">Indirect reseller customers</span></span>

- <span data-ttu-id="83679-178">間接プロバイダーが顧客の製品を注文します</span><span class="sxs-lookup"><span data-stu-id="83679-178">Your indirect provider orders products for your customers</span></span>
- <span data-ttu-id="83679-179">顧客のライセンスとユーザーを管理する</span><span class="sxs-lookup"><span data-stu-id="83679-179">Manage customers' licenses and users</span></span>
- <span data-ttu-id="83679-180">サブスクリプションの更新を処理します</span><span class="sxs-lookup"><span data-stu-id="83679-180">Handle subscription renewals</span></span>

### <a name="to-identify-customers-that-you-acquired-as-a-direct-bill-partner"></a><span data-ttu-id="83679-181">直接請求パートナーとして獲得した顧客を識別するには</span><span class="sxs-lookup"><span data-stu-id="83679-181">To identify customers that you acquired as a direct bill partner</span></span>

1. <span data-ttu-id="83679-182">**顧客**の選択</span><span class="sxs-lookup"><span data-stu-id="83679-182">Select **Customers**</span></span>

2. <span data-ttu-id="83679-183">その詳細を表示する顧客を選択します</span><span class="sxs-lookup"><span data-stu-id="83679-183">Select a customer to view their details</span></span>

3. <span data-ttu-id="83679-184">この顧客が直接請求パートナーとして獲得した顧客である場合は、**製品を追加**または**表示**するためのオプションが表示され、そのサブスクリプションが表示されます。</span><span class="sxs-lookup"><span data-stu-id="83679-184">If this customer is one you acquired as a direct bill partner, you will see options to **add** or **view products** and you will see their subscriptions.</span></span>

4. <span data-ttu-id="83679-185">その顧客と貴社の間に間接リセラーの関係がある場合、これらのオプションは利用できません。</span><span class="sxs-lookup"><span data-stu-id="83679-185">If the customer has an indirect reseller relationship with you, those options will not be available.</span></span>

## <a name="move-your-direct-bill-customers-to-your-indirect-provider"></a><span data-ttu-id="83679-186">直接請求の顧客を間接プロバイダーに移動する</span><span class="sxs-lookup"><span data-stu-id="83679-186">Move your direct bill customers to your indirect provider</span></span>

<span data-ttu-id="83679-187">間接プロバイダーは、販売店との関係がなければ、既存の直接請求先の顧客に対して注文や既存のサブスクリプション転送を送信することはできません。</span><span class="sxs-lookup"><span data-stu-id="83679-187">Your indirect provider cannot submit orders or existing subscription transfers for your existing direct bill customers until they have a reseller relationship with them.</span></span> <span data-ttu-id="83679-188">間接プロバイダーと既存の直接請求顧客の間の再販業者の関係を確立するには、次のいずれかの方法を使用できます。</span><span class="sxs-lookup"><span data-stu-id="83679-188">To establish the reseller relationship between your indirect provider and your existing direct bill customer, you can use one of the following methods:</span></span>

- [<span data-ttu-id="83679-189">再販業者の関係拡張機能</span><span class="sxs-lookup"><span data-stu-id="83679-189">Reseller relationship extension</span></span>](#reseller-relationship-extension)

- [<span data-ttu-id="83679-190">間接リセラー招待を顧客に送信する</span><span class="sxs-lookup"><span data-stu-id="83679-190">Send an indirect reseller invitation to the customer</span></span>](#send-an-indirect-reseller-invitation-to-the-customer)

<span data-ttu-id="83679-191">詳細な手順の概要については、「[間接的な移行に関するドキュメント](https://partner.microsoft.com/resources/collection/Direct-Bill-transition-to-Indirect-reseller#/)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="83679-191">You can find a detailed overview of the step-by-step process in the [Direct to indirect transition document](https://partner.microsoft.com/resources/collection/Direct-Bill-transition-to-Indirect-reseller#/)</span></span>

### <a name="reseller-relationship-extension"></a><span data-ttu-id="83679-192">再販業者の関係拡張機能</span><span class="sxs-lookup"><span data-stu-id="83679-192">Reseller relationship extension</span></span>

<span data-ttu-id="83679-193">パートナーセンターダッシュボードを使用して、既存の直接請求顧客と間接プロバイダーの間の再販業者関係を確立することができます。</span><span class="sxs-lookup"><span data-stu-id="83679-193">You can use the reseller relationship extension feature to establish reseller relationship between your existing direct bill customers and your indirect provider using Partner Center Dashboard.</span></span> <span data-ttu-id="83679-194">この機能を使用する前に、次の点に注意してください。</span><span class="sxs-lookup"><span data-stu-id="83679-194">Before using the feature, note the following:</span></span>

- <span data-ttu-id="83679-195">この機能を利用できるのは、間接リセラーが間接[リセラーの登録](#get-started)を完了するために移行しているダイレクト請求パートナーだけです。</span><span class="sxs-lookup"><span data-stu-id="83679-195">This feature is only available to direct bill partners who are transitioning to become an indirect reseller have completed the [indirect reseller enrollment](#get-started).</span></span>

- <span data-ttu-id="83679-196">この機能は、既存の直接請求顧客にのみ適用できます。</span><span class="sxs-lookup"><span data-stu-id="83679-196">You can only apply this feature to existing direct bill customers.</span></span> <span data-ttu-id="83679-197">[間接リセラーのお客様](#acquire-new-customers-as-indirect-reseller)には適用されません。</span><span class="sxs-lookup"><span data-stu-id="83679-197">It is not applicable to [indirect reseller customers](#acquire-new-customers-as-indirect-reseller).</span></span>

- <span data-ttu-id="83679-198">間接プロバイダー[からパートナーの招待を承諾](#accept-a-partnership-invitation-from-your-indirect-provider)した間接プロバイダーのみを選択できます。</span><span class="sxs-lookup"><span data-stu-id="83679-198">You can only select an indirect provider for which you have [accepted a partner invitation from your indirect provider](#accept-a-partnership-invitation-from-your-indirect-provider).</span></span>

- <span data-ttu-id="83679-199">この顧客に対して使用している請求先情報のコピーが間接プロバイダーに提供されます。</span><span class="sxs-lookup"><span data-stu-id="83679-199">A copy of the bill-to info you have for this customer will be made available to the indirect provider.</span></span> <span data-ttu-id="83679-200">パートナーセンターダッシュボードでこの顧客のアカウントページにアクセスすることにより、請求先情報にアクセスできます。</span><span class="sxs-lookup"><span data-stu-id="83679-200">You can access the bill-to info by accessing the Account page for this customer in Partner Center Dashboard.</span></span>

    > [!NOTE]
    > <span data-ttu-id="83679-201">リセラーとの関係拡張機能を使用することにより、このお客様に対して間接プロバイダーとの請求書の情報を共有することに同意したことになります。</span><span class="sxs-lookup"><span data-stu-id="83679-201">By using the reseller relationship extension feature, you consent to sharing the bill-to info you have for this customer with the indirect provider.</span></span>

- <span data-ttu-id="83679-202">間接プロバイダーは、お客様のテナントに[代理管理特権](customers-revoke-admin-privileges.md)を付与されることはありません。</span><span class="sxs-lookup"><span data-stu-id="83679-202">Your indirect provider will not be provided with [delegated administration privileges](customers-revoke-admin-privileges.md) to the customer tenant.</span></span> <span data-ttu-id="83679-203">間接プロバイダーが代理管理特権を必要とする場合は、代わりに間接リセラーの招待を顧客に送信する必要があります。</span><span class="sxs-lookup"><span data-stu-id="83679-203">If your indirect provider requires delegated administration privileges, you must send an indirect reseller invitation to the customer instead.</span></span>

- <span data-ttu-id="83679-204">リセラーとの関係が確立されると、 [M365 管理センター](https://admin.microsoft.com/AdminPortal/Home#/partners)の [パートナー関係] ページで、間接プロバイダーが顧客に対して CSP パートナーとして表示され、[ビジネス Microsoft Store](https://docs.microsoft.com/microsoft-store/work-with-partner-microsoft-store-business)ます。</span><span class="sxs-lookup"><span data-stu-id="83679-204">Once the reseller relationship is established, the indirect provider will appear as a CSP partner to the customer under the Partner Relationships page in [M365 Admin Center](https://admin.microsoft.com/AdminPortal/Home#/partners) and [Microsoft Store for Business](https://docs.microsoft.com/microsoft-store/work-with-partner-microsoft-store-business).</span></span>

    > [!IMPORTANT]
    > <span data-ttu-id="83679-205">混乱や誤解を避けるために、パートナー契約によって契約必要は、取引先との関係拡張機能を使用して、既存の直接請求顧客と間接プロバイダーの間に再販業者の関係を確立する前に、お客様に直接請求を通知し、同意を得ることができます。</span><span class="sxs-lookup"><span data-stu-id="83679-205">To avoid confusion and misunderstanding, you are contractually obliged by your partner agreement to inform and obtain consent from the direct bill customer before you use the relationship extension feature to establish reseller relationship between an existing direct bill customer and an indirect provider.</span></span>

<span data-ttu-id="83679-206">既存の顧客テナントでこの機能を使用するには、次のようにします。</span><span class="sxs-lookup"><span data-stu-id="83679-206">To use this feature on an existing customer tenant:</span></span>

1. <span data-ttu-id="83679-207">**管理エージェント**としてパートナーセンターにログインします。</span><span class="sxs-lookup"><span data-stu-id="83679-207">Log in to Partner Center as an **Admin Agent**.</span></span>

2. <span data-ttu-id="83679-208">[ **Customers] ページ**で、既存の顧客を選択し、その**クイックリンク**アイコンをクリックして、顧客の概要ビューを展開します。</span><span class="sxs-lookup"><span data-stu-id="83679-208">In the **Customers page**, select an existing customer and click on its **Quick links** icon to expand the summary view of the customer.</span></span>

3. <span data-ttu-id="83679-209">[**間接プロバイダー**] で、[**間接プロバイダーの顧客の転送**] をクリックします。</span><span class="sxs-lookup"><span data-stu-id="83679-209">Under **Indirect provider(s)**, click **Transfer customer on an indirect provider**.</span></span>

    :::image type="content" source="images/direct/direct5-1.png" alt-text="顧客を間接プロバイダーに転送する":::

4. <span data-ttu-id="83679-211">ポップアップダイアログで、リセラーと顧客との関係を設定する**間接プロバイダー**を選択します。</span><span class="sxs-lookup"><span data-stu-id="83679-211">In the pop-up dialog, select the **Indirect Provider** you would like to have reseller relationship with the customer.</span></span>

5. <span data-ttu-id="83679-212">[**保存して続行] を**クリックします。</span><span class="sxs-lookup"><span data-stu-id="83679-212">Click **Save and continue**.</span></span>

6. <span data-ttu-id="83679-213">選択した間接プロバイダーが**間接プロバイダー**の下に表示されることを確認します。</span><span class="sxs-lookup"><span data-stu-id="83679-213">Verify the selected indirect provider shows up under **Indirect provider(s)**.</span></span>

    :::image type="content" source="images/direct/direct5-2.png" alt-text="間接プロバイダーの一覧":::

### <a name="send-an-indirect-reseller-invitation-to-the-customer"></a><span data-ttu-id="83679-215">間接リセラー招待を顧客に送信する</span><span class="sxs-lookup"><span data-stu-id="83679-215">Send an indirect reseller invitation to the customer</span></span>

<span data-ttu-id="83679-216">間接プロバイダーは、再販業者とパートナー関係がある場合に、既存の直接請求先の顧客の注文を送信することはできません。</span><span class="sxs-lookup"><span data-stu-id="83679-216">Your indirect provider cannot submit orders for your existing direct bill customers until they have a reseller relationship with them.</span></span> <span data-ttu-id="83679-217">既存の顧客と間接プロバイダーの間にリセラーの関係を確立するには、間接リセラーの招待を使用して顧客を招待します。</span><span class="sxs-lookup"><span data-stu-id="83679-217">To establish the reseller relationship between your existing customers and your indirect provider, invite the customer using an indirect reseller invitation.</span></span>

1. <span data-ttu-id="83679-218">パートナー センターの左側のナビゲーションから **[間接プロバイダー]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="83679-218">Select **Indirect providers** from your Partner Center left nav.</span></span>

2. <span data-ttu-id="83679-219">貴社と間接プロバイダーの両方について再販業者関係を確立するために新しい顧客を招待するには、 **[新しい顧客を招待する]** を選びます。</span><span class="sxs-lookup"><span data-stu-id="83679-219">Select **Invite new customers** to invite a customer to establish a reseller relationship with both you and the indirect provider at the same time.</span></span> <span data-ttu-id="83679-220">プロバイダーは顧客との再販業者関係を持っている必要があるため、顧客が新しいサブスクリプションを購入したり、既存のサブスクリプションに新しいライセンスを追加したりするときに、顧客に代わって注文を送信することができます。</span><span class="sxs-lookup"><span data-stu-id="83679-220">The provider needs to have a reseller relationship with your customer, so they can submit orders on your customer's behalf when the customer wants to buy new subscriptions or add new licenses to existing subscriptions.</span></span>

    :::image type="content" source="images/direct/direct6.png" alt-text="新しい顧客を招待する":::

3. <span data-ttu-id="83679-222">次のページで、メール メッセージの下書きを確認します。</span><span class="sxs-lookup"><span data-stu-id="83679-222">On the next page, review the draft email message.</span></span> <span data-ttu-id="83679-223">メールで下書きメッセージを開くか、メッセージをクリップボードにコピーし、メールに貼り付けます。</span><span class="sxs-lookup"><span data-stu-id="83679-223">You can open the draft message in email, or you can copy the message to your clipboard and paste it into an email.</span></span>

4. <span data-ttu-id="83679-224">電子メールのテキストを編集して必要なものを指定しますが、自分のアカウントとプロバイダーのアカウントの両方に顧客を直接接続できるように、パーソナライズされたリンクを含めてください。</span><span class="sxs-lookup"><span data-stu-id="83679-224">Edit the text in the email to say what you need but be sure to include the link as it is personalized to connect the customer directly to both your account and your provider's account.</span></span> <span data-ttu-id="83679-225">**[完了]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="83679-225">Then select **Done**.</span></span>

5. <span data-ttu-id="83679-226">顧客が貴社とプロバイダーを指名リセラーとして承認すると、貴社には顧客のサブスクリプション、ライセンス、ユーザーを管理するための管理者のアクセス許可が付与され、間接プロバイダーは、顧客に代わって注文を送信できるようになります。</span><span class="sxs-lookup"><span data-stu-id="83679-226">After the customer authorizes you and your provider to be their resellers of record, you'll have administrator permissions to manage their subscriptions, licenses, and users on their behalf, and your indirect provider will be able to submit orders on their behalf.</span></span>

6. <span data-ttu-id="83679-227">顧客のアカウント、サービス、ユーザー、ライセンスを管理するには、顧客の名前の下矢印を選んで、顧客のレコードを展開します。</span><span class="sxs-lookup"><span data-stu-id="83679-227">To manage the customer's account, services, users, and licenses, expand the customer's record by selecting the down arrow near their name.</span></span>

### <a name="microsoft-customer-agreement-acceptance"></a><span data-ttu-id="83679-228">Microsoft カスタマーアグリーメントへの同意</span><span class="sxs-lookup"><span data-stu-id="83679-228">Microsoft Customer Agreement acceptance</span></span>

<span data-ttu-id="83679-229">Microsoft Cloud Agreement は、2020年1月31日まで有効です。</span><span class="sxs-lookup"><span data-stu-id="83679-229">Microsoft Cloud Agreement is valid until January 31, 2020.</span></span> <span data-ttu-id="83679-230">その後、すべてのお客様 (既存および新規) は、新しい[Microsoft カスタマー契約](https://docs.microsoft.com/partner-center/confirm-customer-agreement)に署名する必要があります。</span><span class="sxs-lookup"><span data-stu-id="83679-230">After that date, all customers, existing and new, must sign the new [Microsoft Customer Agreement](https://docs.microsoft.com/partner-center/confirm-customer-agreement).</span></span> <span data-ttu-id="83679-231">お客様の移行の場合:</span><span class="sxs-lookup"><span data-stu-id="83679-231">For transitioning customers, if:</span></span>

- <span data-ttu-id="83679-232">**お客様はまだ Microsoft カスタマーアグリーメントに同意していません**</span><span class="sxs-lookup"><span data-stu-id="83679-232">**Customer has not accepted Microsoft Customer Agreement yet**</span></span>

   <span data-ttu-id="83679-233">間接プロバイダーと協力して、お客様が[Microsoft カスタマーアグリーメントに同意](confirm-customer-agreement.md)するようにしてください。</span><span class="sxs-lookup"><span data-stu-id="83679-233">Please work with Indirect Provider to have customer [accept the Microsoft Customer Agreement](confirm-customer-agreement.md).</span></span>

- <span data-ttu-id="83679-234">**お客様は、Microsoft 365 管理センターを通じて Microsoft カスタマーアグリーメントに同意しました**</span><span class="sxs-lookup"><span data-stu-id="83679-234">**Customer has accepted Microsoft Customer Agreement with you through the Microsoft 365 Admin Center**</span></span>

   <span data-ttu-id="83679-235">間接プロバイダーとの再販業者の関係が確立されると、受け入れが維持されます。</span><span class="sxs-lookup"><span data-stu-id="83679-235">The acceptance will be retained once the reseller relationship is established with the Indirect Provider.</span></span> <span data-ttu-id="83679-236">何もする必要はありません。</span><span class="sxs-lookup"><span data-stu-id="83679-236">There is nothing you need to do.</span></span>

- <span data-ttu-id="83679-237">**お客様がパートナーの構成証明を通じて Microsoft カスタマーアグリーメントに同意しました**</span><span class="sxs-lookup"><span data-stu-id="83679-237">**Customer has accepted Microsoft Customer Agreement with you through partner attestation**</span></span>

   <span data-ttu-id="83679-238">受け入れは保持されません。</span><span class="sxs-lookup"><span data-stu-id="83679-238">The acceptance will not be retained.</span></span> <span data-ttu-id="83679-239">[パートナーセンターでお客様の同意を更新するには、](confirm-customer-agreement.md#confirm-customer-acceptance-for-existing-customers)間接プロバイダーと協力してください。</span><span class="sxs-lookup"><span data-stu-id="83679-239">Please work with Indirect Provider to [update the customer's acceptance in Partner Center](confirm-customer-agreement.md#confirm-customer-acceptance-for-existing-customers).</span></span>

## <a name="transfer-existing-direct-bill-subscriptions-to-indirect-provider"></a><span data-ttu-id="83679-240">既存の直接請求書のサブスクリプションを間接プロバイダーに転送する</span><span class="sxs-lookup"><span data-stu-id="83679-240">Transfer existing direct bill subscriptions to indirect provider</span></span>

<span data-ttu-id="83679-241">CSP 間接モデルでは、間接リセラーには Microsoft との請求関係がありません。</span><span class="sxs-lookup"><span data-stu-id="83679-241">Under CSP indirect model, indirect resellers do not have billing relationships with Microsoft.</span></span> <span data-ttu-id="83679-242">間接リセラーは、間接プロバイダーを通じて顧客のサブスクリプションを取得します。</span><span class="sxs-lookup"><span data-stu-id="83679-242">Instead, indirect resellers obtain subscriptions for their customers through their indirect providers.</span></span> <span data-ttu-id="83679-243">ダイレクト請求パートナーから間接リセラーに移行している間は、直接請求パートナーとして所有している既存のサブスクリプションを間接プロバイダーに譲渡する必要があります。</span><span class="sxs-lookup"><span data-stu-id="83679-243">While transitioning from direct bill partner to indirect reseller, you need to transfer the existing subscriptions you have as the direct bill partner to your indirect provider.</span></span> <span data-ttu-id="83679-244">パートナーセンターダッシュボードのセルフサービスサブスクリプション転送機能を使用して、これを行うことができます。</span><span class="sxs-lookup"><span data-stu-id="83679-244">You can use the self-served subscription transfer feature in Partner Center Dashboard to do so.</span></span>

### <a name="pre-requisites"></a><span data-ttu-id="83679-245">前提条件</span><span class="sxs-lookup"><span data-stu-id="83679-245">Pre-requisites</span></span>

<span data-ttu-id="83679-246">この機能を使用する前に、次の点に注意してください。</span><span class="sxs-lookup"><span data-stu-id="83679-246">Before using the feature, note the following:</span></span>

- <span data-ttu-id="83679-247">この機能は、既存の直接請求パートナーテナントを使用して間接リセラーの登録を完了したパートナーを移行する場合にのみ使用できます。</span><span class="sxs-lookup"><span data-stu-id="83679-247">This feature is only available to transitioning partners who have completed the indirect reseller enrollment using their existing direct bill partner tenants</span></span>

- <span data-ttu-id="83679-248">特定の顧客に関連付けられているサブスクリプションを転送する前に、移行パートナーは顧客を間接プロバイダーに移動する必要があります。</span><span class="sxs-lookup"><span data-stu-id="83679-248">Before transferring subscriptions associated with a given customer, the transitioning partner must move the customer to an indirect provider.</span></span>

- <span data-ttu-id="83679-249">お客様は[間接プロバイダーを通じて Microsoft カスタマーアグリーメントに同意](#microsoft-customer-agreement-acceptance)しました。</span><span class="sxs-lookup"><span data-stu-id="83679-249">Customer has [accepted Microsoft Customer Agreement through the Indirect Provider](#microsoft-customer-agreement-acceptance).</span></span>

### <a name="how-to-transition-to-indirect-reseller-status"></a><span data-ttu-id="83679-250">間接リセラーの状態に移行する方法</span><span class="sxs-lookup"><span data-stu-id="83679-250">How-to transition to indirect reseller status</span></span>

<span data-ttu-id="83679-251">この機能は、4つの手順からなるプロセスです。</span><span class="sxs-lookup"><span data-stu-id="83679-251">The feature is a 4-step process, where:</span></span>

- <span data-ttu-id="83679-252">遷移中のパートナーは、サブスクリプションの譲渡要求を作成します。</span><span class="sxs-lookup"><span data-stu-id="83679-252">The transitioning partner creates a subscription transfer request.</span></span> <span data-ttu-id="83679-253">要求には、同じ顧客に関連付けられた1つ以上の既存のサブスクリプションが含まれており、間接プロバイダーによってアドレス指定されています。</span><span class="sxs-lookup"><span data-stu-id="83679-253">The request contains one or more existing subscriptions associated with the same customer and is addressed to an indirect provider.</span></span>

- <span data-ttu-id="83679-254">間接プロバイダーは、転送要求のレビューと受け入れ (または拒否) を行います。</span><span class="sxs-lookup"><span data-stu-id="83679-254">The indirect provider reviews and accepts (or reject) the transfer request.</span></span>

- <span data-ttu-id="83679-255">間接プロバイダーは、転送要求が完了したことを確認します。</span><span class="sxs-lookup"><span data-stu-id="83679-255">The indirect provider verifies that the transfer request is complete.</span></span>

- <span data-ttu-id="83679-256">移行パートナーは、転送要求が完了したことを確認します。</span><span class="sxs-lookup"><span data-stu-id="83679-256">The transitioning partner verifies that the transfer request is complete.</span></span>

### <a name="transitioning-partner"></a><span data-ttu-id="83679-257">パートナーの移行中</span><span class="sxs-lookup"><span data-stu-id="83679-257">Transitioning partner</span></span>

> [!NOTE]
> <span data-ttu-id="83679-258">また、[パートナーセンター API/SDK](https://docs.microsoft.com/partner-center/develop/manage-customers)を使用して、既存のサブスクリプションを間接プロバイダーに転送することもできます。</span><span class="sxs-lookup"><span data-stu-id="83679-258">You can also use [Partner Center API/SDK](https://docs.microsoft.com/partner-center/develop/manage-customers) to transfer the existing subscriptions to your indirect provider.</span></span>
>
> - [<span data-ttu-id="83679-259">顧客のサブスクリプション譲渡の資格を取得する</span><span class="sxs-lookup"><span data-stu-id="83679-259">Get a customer's subscriptions transfer eligibility</span></span>](https://docs.microsoft.com/partner-center/develop/get-customer-s-subscriptions-transfer-eligibility)
> - [<span data-ttu-id="83679-260">顧客からの譲渡を作成する</span><span class="sxs-lookup"><span data-stu-id="83679-260">Create a customer's transfer</span></span>](https://docs.microsoft.com/partner-center/develop/create-a-transfer)
> - [<span data-ttu-id="83679-261">顧客の譲渡を撤回する</span><span class="sxs-lookup"><span data-stu-id="83679-261">Withdraw a customer's transfer</span></span>](https://docs.microsoft.com/partner-center/develop/withdraw-a-transfer)
> - [<span data-ttu-id="83679-262">顧客の譲渡を承諾する</span><span class="sxs-lookup"><span data-stu-id="83679-262">Accept a customer's transfer</span></span>](https://docs.microsoft.com/partner-center/develop/accept-a-transfer)
> - [<span data-ttu-id="83679-263">顧客の譲渡を拒否する</span><span class="sxs-lookup"><span data-stu-id="83679-263">Reject a Customer's transfer</span></span>](https://docs.microsoft.com/partner-center/develop/reject-a-transfer)
> - [<span data-ttu-id="83679-264">顧客の譲渡を取得する</span><span class="sxs-lookup"><span data-stu-id="83679-264">Get a customer's transfers</span></span>](https://docs.microsoft.com/partner-center/develop/get-all-of-a-customer-s-transfers)
> - [<span data-ttu-id="83679-265">Id で転送の詳細を取得する</span><span class="sxs-lookup"><span data-stu-id="83679-265">Get transfer details by id</span></span>](https://docs.microsoft.com/partner-center/develop/get-transfer-by-id)

### <a name="transitioning-partner---create-transfer-request"></a><span data-ttu-id="83679-266">パートナー-転送の作成要求を移行しています</span><span class="sxs-lookup"><span data-stu-id="83679-266">Transitioning partner - create transfer request</span></span>

<span data-ttu-id="83679-267">移行パートナーとして転送要求を作成するには、次のようにします。</span><span class="sxs-lookup"><span data-stu-id="83679-267">To create a transfer request as the transitioning partner:</span></span>

1. <span data-ttu-id="83679-268">**管理エージェント**としてパートナーセンターにログインします。</span><span class="sxs-lookup"><span data-stu-id="83679-268">Log in to Partner Center as an **Admin Agent**.</span></span>

2. <span data-ttu-id="83679-269">[ **Customers** ] ページで目的の顧客を選択し、[クイックリンク] アイコンをクリックして顧客の概要ビューを展開します。</span><span class="sxs-lookup"><span data-stu-id="83679-269">In the **Customers** page, select the intended customer and click on the Quick links icon to expand the summary view of the customer.</span></span>

3. <span data-ttu-id="83679-270">[**間接プロバイダー**] で、目的の間接プロバイダーが一覧に表示されていることを確認します。</span><span class="sxs-lookup"><span data-stu-id="83679-270">Under **Indirect provider(s)**, confirm that the intended indirect provider is listed.</span></span>

4. <span data-ttu-id="83679-271">[**サブスクリプションの表示**] をクリックします。</span><span class="sxs-lookup"><span data-stu-id="83679-271">Click **View Subscriptions**.</span></span>

5. <span data-ttu-id="83679-272">[**サブスクリプション**] ページで、[**サブスクリプションの譲渡**] を探します。</span><span class="sxs-lookup"><span data-stu-id="83679-272">In the **Subscriptions** page, look for **Subscription Transfer**.</span></span>

6. <span data-ttu-id="83679-273">[**サブスクリプションの譲渡**] で、[**サブスクリプションの譲渡の要求**] をクリックします。</span><span class="sxs-lookup"><span data-stu-id="83679-273">Under **Subscription Transfer**, click **Request subscription transfer**.</span></span>

    :::image type="content" source="images/direct/direct8.png" alt-text="サブスクリプションの譲渡を要求する":::

7. <span data-ttu-id="83679-275">[転送要求] ダイアログボックスで、転送する1つ以上のサブスクリプションを選択します。</span><span class="sxs-lookup"><span data-stu-id="83679-275">In the transfer request dialog, select one or more subscriptions to be transferred.</span></span>

    :::image type="content" source="images/direct/direct9.png" alt-text="転送要求の作成":::

8. <span data-ttu-id="83679-277">**Create** をクリックしてください。</span><span class="sxs-lookup"><span data-stu-id="83679-277">Click **Create**.</span></span>

9. <span data-ttu-id="83679-278">アクティブなサブスクリプションの譲渡要求が [**サブスクリプションの譲渡**] に表示されます。</span><span class="sxs-lookup"><span data-stu-id="83679-278">An active subscription transfer request will appear under **Subscription Transfer**.</span></span>

    :::image type="content" source="images/direct/direct10.png" alt-text="要求一覧の転送":::

10. <span data-ttu-id="83679-280">サブスクリプションへの譲渡要求が作成されたことを間接プロバイダーに通知します。</span><span class="sxs-lookup"><span data-stu-id="83679-280">Inform your indirect provider that you have created a subscription transfer request to them.</span></span>

### <a name="indirect-provider---accept-transfer-request"></a><span data-ttu-id="83679-281">間接プロバイダー-転送要求の受け入れ</span><span class="sxs-lookup"><span data-stu-id="83679-281">Indirect provider - accept transfer request</span></span>

<span data-ttu-id="83679-282">間接プロバイダーとして転送要求を確認して受け入れるには、次のようにします。</span><span class="sxs-lookup"><span data-stu-id="83679-282">To review and accept a transfer request as the indirect provider:</span></span>

1. <span data-ttu-id="83679-283">管理エージェントまたは**営業担当\*\*\*\*者**としてパートナーセンターにログインします。</span><span class="sxs-lookup"><span data-stu-id="83679-283">Log in to Partner Center as an **Admin** Agent or **Sales Agent**.</span></span>

2. <span data-ttu-id="83679-284">[ **Customers** ] ページで、目的の顧客を選択し、そのクイックリンクアイコンをクリックして、顧客の概要ビューを展開します。</span><span class="sxs-lookup"><span data-stu-id="83679-284">In the **Customers** page, select the intended customer and click on its Quick links icon to expand the summary view of the customer.</span></span>

3. <span data-ttu-id="83679-285">[**間接リセラー**] の下に、[移行パートナー] が表示されていることを確認します。</span><span class="sxs-lookup"><span data-stu-id="83679-285">Under **Indirect reseller(s)**, confirm the transitioning partner is listed.</span></span>

4. <span data-ttu-id="83679-286">[**サブスクリプションの表示**] をクリックします。</span><span class="sxs-lookup"><span data-stu-id="83679-286">Click **View Subscriptions**.</span></span>

5. <span data-ttu-id="83679-287">[**サブスクリプション**] ページで、[**サブスクリプションの譲渡**] を探します。</span><span class="sxs-lookup"><span data-stu-id="83679-287">In the **Subscriptions** page, look for **Subscription Transfer**.</span></span>

    :::image type="content" source="images/direct/direct11.png" alt-text="転送要求の表示":::

6. <span data-ttu-id="83679-289">[**サブスクリプションの譲渡**] で、[転送要求] をクリックして確認します。</span><span class="sxs-lookup"><span data-stu-id="83679-289">Under **Subscription Transfer**, click on the transfer request to review.</span></span>

7. <span data-ttu-id="83679-290">必要に応じて、[**承諾**] (または [**拒否**]) をクリックします。</span><span class="sxs-lookup"><span data-stu-id="83679-290">Click **Accept** (or **Reject**) as appropriate.</span></span>

    :::image type="content" source="images/direct/direct12.png" alt-text="譲渡要求の受け入れ":::

8. <span data-ttu-id="83679-292">転送要求が完了するまで待ちます。</span><span class="sxs-lookup"><span data-stu-id="83679-292">Wait for the transfer request to complete.</span></span>

### <a name="indirect-provider---verify-transfer-request-is-complete"></a><span data-ttu-id="83679-293">間接プロバイダー-転送要求の確認が完了しました</span><span class="sxs-lookup"><span data-stu-id="83679-293">Indirect provider - verify transfer request is complete</span></span>

1. <span data-ttu-id="83679-294">転送要求が正常に完了したら、サブスクリプションが [**サブスクリプション**] の下に表示されることを確認します。</span><span class="sxs-lookup"><span data-stu-id="83679-294">After the transfer request is completed successfully, verify that you can see the subscriptions appear under **Subscriptions**.</span></span>

2. <span data-ttu-id="83679-295">移行パートナーに通知します。</span><span class="sxs-lookup"><span data-stu-id="83679-295">Inform the transitioning partner.</span></span>

### <a name="transitioning-partner---verify-transfer-request-is-complete"></a><span data-ttu-id="83679-296">パートナーの移行-転送要求の確認が完了しました</span><span class="sxs-lookup"><span data-stu-id="83679-296">Transitioning partner - verify transfer request is complete</span></span>

<span data-ttu-id="83679-297">移行中のパートナーは、次の操作を行う必要があります。</span><span class="sxs-lookup"><span data-stu-id="83679-297">The transitioning partner should do the following:</span></span>

1. <span data-ttu-id="83679-298">**管理エージェント**または**営業担当**者としてパートナーセンターにログインします。</span><span class="sxs-lookup"><span data-stu-id="83679-298">Log in to Partner Center as an **Admin Agent** or **Sales Agent**.</span></span>

2. <span data-ttu-id="83679-299">[ **Customers** ] ページで目的の顧客を選択し、[**クイックリンク**] アイコンをクリックして顧客の概要ビューを展開します。</span><span class="sxs-lookup"><span data-stu-id="83679-299">In the **Customers** page, select the intended customer and click on the **Quick links** icon to expand the summary view of the customer.</span></span>

3. <span data-ttu-id="83679-300">[**サブスクリプションの表示**] をクリックします。</span><span class="sxs-lookup"><span data-stu-id="83679-300">Click **View Subscriptions**.</span></span>

4. <span data-ttu-id="83679-301">[**サブスクリプション**] ページで、[**サブスクリプションの譲渡**] を探します。</span><span class="sxs-lookup"><span data-stu-id="83679-301">In the **Subscriptions** page, look for **Subscription Transfer**.</span></span>

5. <span data-ttu-id="83679-302">転送要求が**完了**とマークされていることを確認します。</span><span class="sxs-lookup"><span data-stu-id="83679-302">Verify that the transfer request is marked as **Complete**.</span></span>

6. <span data-ttu-id="83679-303">サブスクリプションが [**サブスクリプション**] ページに [アクティブ] と表示されないことを確認します。</span><span class="sxs-lookup"><span data-stu-id="83679-303">Verify that the subscription(s) no longer appear as active in the **Subscriptions** page:</span></span>

   1. <span data-ttu-id="83679-304">これが Azure サブスクリプション (0145P) の場合は、表示されなくなります。</span><span class="sxs-lookup"><span data-stu-id="83679-304">If this is an Azure subscription (MS-AZR-0145P), it will no longer be listed.</span></span>

   2. <span data-ttu-id="83679-305">これが接続クライアントベースのサブスクリプション (Office 365、Dynamics、Intune) である場合は、状態が "**中断**" として一覧表示されます。</span><span class="sxs-lookup"><span data-stu-id="83679-305">If this is a seat-based subscription (Office 365, Dynamics, Intune), it will be listed with state as **Suspended**.</span></span>

   :::image type="content" source="images/direct/direct13.png" alt-text="サブスクリプションが中断されました":::

### <a name="considerations"></a><span data-ttu-id="83679-307">考慮事項</span><span class="sxs-lookup"><span data-stu-id="83679-307">Considerations</span></span>

- <span data-ttu-id="83679-308">**サブスクリプション ID は、転送後に異なります。**</span><span class="sxs-lookup"><span data-stu-id="83679-308">**Subscription ID will be different after transfer.**</span></span> <span data-ttu-id="83679-309">Azure サブスクリプション (0145P) の場合、さらに、azure サブスクリプション ID が付与されます。これは以前の所有者から保持され、Azure 管理ポータルに表示されます。</span><span class="sxs-lookup"><span data-stu-id="83679-309">If it is an Azure subscription (MS-AZR-0145P), additionally, it will have an Azure Subscription ID, which is retained from the previous owner, and will appear in the Azure management portal.</span></span>

- <span data-ttu-id="83679-310">**複数の転送要求で同じサブスクリプションを参照することはできません。**</span><span class="sxs-lookup"><span data-stu-id="83679-310">**The same subscription cannot be referenced by multiple transfer requests.**</span></span> <span data-ttu-id="83679-311">既存のサブスクリプションを含む転送要求を作成した後は、最初の転送要求が取り消されるまで、同じサブスクリプションを含む追加の転送要求を作成することはできません。</span><span class="sxs-lookup"><span data-stu-id="83679-311">After you have created a transfer request, which includes an existing subscription, you cannot create additional transfer requests including the same subscription, until the first transfer request is canceled.</span></span>

- <span data-ttu-id="83679-312">**座席ベースのサブスクリプションのアドオンは、基本サブスクリプションと共に転送する必要があります。**</span><span class="sxs-lookup"><span data-stu-id="83679-312">**Add-ons for seat-based subscriptions must be transferred along with their base subscription.**</span></span> <span data-ttu-id="83679-313">転送要求を作成するときに、1つ以上のアドオンを含む既存のサブスクリプションを選択すると、そのアドオンは自動的に転送要求に含まれます。</span><span class="sxs-lookup"><span data-stu-id="83679-313">When creating a transfer request, if you pick an existing subscription with one or more add-ons, the add-ons will automatically be included in the transfer request.</span></span>

- <span data-ttu-id="83679-314">**サブスクリプションに対する接続クライアント数の変更は、既存の転送要求に反映されません。**</span><span class="sxs-lookup"><span data-stu-id="83679-314">**Seat count changes to a subscription will not be reflected in existing transfer request.**</span></span> <span data-ttu-id="83679-315">既存のサブスクリプションを含む譲渡要求を作成した後は、サブスクリプションの接続クライアント数 (または関連するアドオン) を更新しないようにしてください。</span><span class="sxs-lookup"><span data-stu-id="83679-315">After you have created a transfer request which includes an existing subscription, you should avoid updating the seat quantity of the subscription (or associated addons).</span></span> <span data-ttu-id="83679-316">この場合、新しい数量は転送要求に反映されません。</span><span class="sxs-lookup"><span data-stu-id="83679-316">If you do so, the new quantity will not be reflected in the transfer request.</span></span> <span data-ttu-id="83679-317">間接プロバイダーが譲渡要求を受け入れると、結果として得られるサブスクリプションの数量が古いものになります。</span><span class="sxs-lookup"><span data-stu-id="83679-317">After the indirect provider accepts the transfer request, the resultant subscription will have the old quantity.</span></span> <span data-ttu-id="83679-318">新しい数量を間接プロバイダーに転送する場合は、既存の転送要求を取り消して新しい数量を再作成する必要があります。</span><span class="sxs-lookup"><span data-stu-id="83679-318">If you wish for the new quantity to be transferred to the indirect provider, you must cancel the existing transfer request and recreate a new one.</span></span>

- <span data-ttu-id="83679-319">**セルフサービスサブスクリプション転送を使用して、すべての購入を転送できるわけではありません。**</span><span class="sxs-lookup"><span data-stu-id="83679-319">**Not all purchases can be transferred using self-served subscription transfer.**</span></span> <span data-ttu-id="83679-320">現時点では、この機能を使用して、O365 サブスクリプションと Azure PAYG サブスクリプション (0145P) のみを転送できます。</span><span class="sxs-lookup"><span data-stu-id="83679-320">Currently, you can only transfer O365 subscriptions and Azure PAYG subscriptions (MS-AZR-0145P) using this feature.</span></span> <span data-ttu-id="83679-321">Azure プラン、azure 予約インスタンス、用語ベースのサブスクリプション、Azure Marketplace の SaaS サブスクリプションなど、その他の購入はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="83679-321">Other purchases including Azure Plans, Azure Reserved Instances, Term-based Subscriptions and SaaS subscriptions for Azure Marketplace are not supported.</span></span> <span data-ttu-id="83679-322">[転送要求の送信] ページでサブスクリプションを転送できない理由が表示されます。</span><span class="sxs-lookup"><span data-stu-id="83679-322">You will see a reason why a subscription cannot be transferred in the submit transfer request page.</span></span> <span data-ttu-id="83679-323">これらのサブスクリプションを譲渡するには、[既存のサブスクリプションをキャンセル](https://docs.microsoft.com/partner-center/create-a-new-subscription#suspend-or-cancel-a-subscription)し、間接プロバイダーを通じて顧客向けの新しいプランを購入する必要があります。</span><span class="sxs-lookup"><span data-stu-id="83679-323">To transfer these subscriptions, you will need to [cancel the existing subscription](https://docs.microsoft.com/partner-center/create-a-new-subscription#suspend-or-cancel-a-subscription) and purchase new offer for customer through Indirect Provider.</span></span>

- <span data-ttu-id="83679-324">**サンドボックス環境を使用してテストすることはできません。**</span><span class="sxs-lookup"><span data-stu-id="83679-324">**Cannot be tested using sandbox environment.**</span></span>

## <a name="enroll-for-indirect-reseller-incentives"></a><span data-ttu-id="83679-325">間接リセラー インセンティブに登録する</span><span class="sxs-lookup"><span data-stu-id="83679-325">Enroll for indirect reseller incentives</span></span>

<span data-ttu-id="83679-326">既存の直接請求パートナー テナントで間接リセラーとして正常に登録した後、30 日以内に、間接リセラー インセンティブへの登録の招待を受け取ります。</span><span class="sxs-lookup"><span data-stu-id="83679-326">After you have successfully enrolled as an indirect reseller on your existing direct bill partner tenant, you will receive an invitation to enroll for indirect reseller incentive within 30 days.</span></span> <span data-ttu-id="83679-327">招待は、CSP パートナー テナントに現在関連付けられているパートナー MPN アカウントに基づいています。</span><span class="sxs-lookup"><span data-stu-id="83679-327">The invitation is based on the partner MPN account that is currently associated with your CSP partner tenant.</span></span> <span data-ttu-id="83679-328">招待は、パートナー MPN アカウントに関連付けられているメール アドレスに送られます。</span><span class="sxs-lookup"><span data-stu-id="83679-328">The invitation will be sent to the email address associated with the partner MPN account.</span></span>

<span data-ttu-id="83679-329">また、パートナーは、その同じパートナー テナントで直接請求インセンティブ プログラムに登録する資格もあります。</span><span class="sxs-lookup"><span data-stu-id="83679-329">You are also eligible to enroll for direct bill incentive programs with that same partner tenant.</span></span> <span data-ttu-id="83679-330">プログラムは個別に管理する必要があります。</span><span class="sxs-lookup"><span data-stu-id="83679-330">You must manage the programs separately.</span></span>

## <a name="next-steps"></a><span data-ttu-id="83679-331">次の手順</span><span class="sxs-lookup"><span data-stu-id="83679-331">Next steps</span></span>

- [<span data-ttu-id="83679-332">間接リセラーになることについての追加情報</span><span class="sxs-lookup"><span data-stu-id="83679-332">Additional information on becoming an indirect reseller</span></span>](https://assetsprod.microsoft.com/csp-directbill-to-indirect-transition.pdf)
- [<span data-ttu-id="83679-333">CSP の直接パートナーの新しい要件</span><span class="sxs-lookup"><span data-stu-id="83679-333">CSP direct partner new requirements</span></span>](direct-partner-new-requirements.md)
- [<span data-ttu-id="83679-334">制限付きの直接請求機能</span><span class="sxs-lookup"><span data-stu-id="83679-334">Restricted direct bill capabilities</span></span>](restricted-direct-bill-capabilities.md)
