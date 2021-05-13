---
title: ダイレクト請求パートナーを間接リセラーに切り替える
ms.topic: how-to
ms.date: 06/05/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: CSP プログラムパートナーがパートナーセンターを使用して、直接請求パートナーから間接リセラーに移行する方法について説明します。
author: aarzh-AaronZhang
ms.author: v-aarzh
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: e57ae5a30e3ee4331ae509a0650d09baf4a82590
ms.sourcegitcommit: 7a6836bd962d5b426a8cb34a9132a87cbbbf39f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/13/2021
ms.locfileid: "109854895"
---
# <a name="transition-from-cloud-solution-provider-csp-direct-bill-partner-to-csp-indirect-reseller"></a><span data-ttu-id="a90a7-103">クラウド ソリューション プロバイダー (CSP) 直接請求パートナーから CSP 間接リセラーへの移行</span><span class="sxs-lookup"><span data-stu-id="a90a7-103">Transition from Cloud Solution Provider (CSP) direct bill partner to CSP indirect reseller</span></span>

<span data-ttu-id="a90a7-104">**適切なロール**: 全体管理者</span><span class="sxs-lookup"><span data-stu-id="a90a7-104">**Appropriate roles**: Global admin</span></span>

>[!Note]
><span data-ttu-id="a90a7-105">この記事は、間接リセラーに移行することに決めた直接請求パートナーのためのものです。</span><span class="sxs-lookup"><span data-stu-id="a90a7-105">This article is intended for direct bill partners who have decided to transition to indirect resellers.</span></span> <span data-ttu-id="a90a7-106">ただし、間接リセラーとして登録するための明示的な決定をまだ行っていない場合でも、CSP direct bill partner プログラムの新しい [要件](direct-partner-new-requirements.md) を満たしていない直接請求先のパートナーは、 [直接請求書の機能が制限さ](restricted-direct-bill-capabilities.md)れるときに Microsoft によって通知されます。</span><span class="sxs-lookup"><span data-stu-id="a90a7-106">However, even if you have not made an explicit decision yet to enroll as an indirect reseller, direct bill partners who do not meet the new [requirements](direct-partner-new-requirements.md) for the CSP direct bill partner program will be informed by Microsoft when their [direct bill capabilities will be restricted](restricted-direct-bill-capabilities.md).</span></span>
<br><span data-ttu-id="a90a7-107">2021年1月の時点で、新しい収益要件が追加されます。</span><span class="sxs-lookup"><span data-stu-id="a90a7-107">As of January 2021, a new revenue requirement will be added.</span></span> <span data-ttu-id="a90a7-108">ダイレクト請求パートナーとして登録されているパートナーは、過去12か月間にわたり、パートナーのグローバルアカウントレベルで、クラウドソリューションプロバイダープログラムの収益に対して少なくとも USD $ 300K でトランザクションを実行する必要があります。</span><span class="sxs-lookup"><span data-stu-id="a90a7-108">Partners enrolled as a direct bill partner will need to have transacted at least USD$300K in Cloud Solution Provider program revenue at a Partner Global Account level over the previous 12 months.</span></span>

<span data-ttu-id="a90a7-109">パートナーは、既存の直接請求テナントを使用して間接リセラー プログラムに登録できます。</span><span class="sxs-lookup"><span data-stu-id="a90a7-109">You will be able to enroll in the indirect reseller program using your existing direct bill tenant.</span></span>

## <a name="get-started"></a><span data-ttu-id="a90a7-110">はじめに</span><span class="sxs-lookup"><span data-stu-id="a90a7-110">Get started</span></span>

1. <span data-ttu-id="a90a7-111">パートナー センターのパートナー プロファイルと MPN ID が最新の状態であることを確認します。</span><span class="sxs-lookup"><span data-stu-id="a90a7-111">Make sure your partner profile in Partner Center and MPN ID are current.</span></span>

2. <span data-ttu-id="a90a7-112">間接リセラーに移行する直接請求テナントのグローバル管理者としてパートナー センターにサインインします。</span><span class="sxs-lookup"><span data-stu-id="a90a7-112">Sign in to Partner Center as the global admin for the direct bill tenant you are transitioning to indirect reseller.</span></span>

   :::image type="content" source="images/direct/direct1.png" alt-text="概要":::

3. <span data-ttu-id="a90a7-114">登録フォームでパートナーの詳細を確認します。</span><span class="sxs-lookup"><span data-stu-id="a90a7-114">Review your partner details on the enrollment form.</span></span>

   :::image type="content" source="images/direct/direct2a.png" alt-text="今すぐ登録":::

4. <span data-ttu-id="a90a7-116">[Enroll now]\(今すぐ登録\) を選択します。</span><span class="sxs-lookup"><span data-stu-id="a90a7-116">Select Enroll now.</span></span> <span data-ttu-id="a90a7-117">間接リセラー ビジネスでは、直接ビジネスに使用しているものと同じ AAD テナントを使います。</span><span class="sxs-lookup"><span data-stu-id="a90a7-117">Your indirect reseller business will use the same AAD tenant you use for your direct business.</span></span>

    > [!NOTE]
    > <span data-ttu-id="a90a7-118">最初は、この新しい移行機能は、契約応当日が 9 月から 12 月までのパートナーが利用できます。</span><span class="sxs-lookup"><span data-stu-id="a90a7-118">Initially, this new transition capability will be available for partners with September to December anniversary dates.</span></span> <span data-ttu-id="a90a7-119">契約応当日が 9 月から 12 月の間にない場合、現時点では機能が表示されません。</span><span class="sxs-lookup"><span data-stu-id="a90a7-119">If you don"t have an anniversary date between September and December, you won't see the capability at this time.</span></span> <span data-ttu-id="a90a7-120">契約応当日が 2018 年 12 月以降のパートナーは、今後パートナー向けに機能が有効になった時点で通知されます。</span><span class="sxs-lookup"><span data-stu-id="a90a7-120">Partners with anniversary dates after December 2018 will be notified later once the feature is enabled for the partners.</span></span>

5. <span data-ttu-id="a90a7-121">登録が承認されたら、パートナー センターにもう一度サインインします。</span><span class="sxs-lookup"><span data-stu-id="a90a7-121">When your enrollment is approved, sign in to Partner Center again.</span></span>

    > [!NOTE]
    > <span data-ttu-id="a90a7-122">通常であればすぐに承認されますが、最大で 5 営業日かかることがあります。</span><span class="sxs-lookup"><span data-stu-id="a90a7-122">While approval is usually immediate, it can take up to five business days.</span></span> <span data-ttu-id="a90a7-123">承認が済むと、登録フォームで主要連絡先に指定したメール アドレスに通知が届きます。</span><span class="sxs-lookup"><span data-stu-id="a90a7-123">Once approved, you will receive a notification to the email address you have specified under primary contact in the enrollment form.</span></span> <span data-ttu-id="a90a7-124">また、[**設定**] [  >  **アカウント設定**] [  >  **パートナープロファイル**] > [プログラム情報] で、登録の状態を確認することもできます。</span><span class="sxs-lookup"><span data-stu-id="a90a7-124">You can also check your enrollment status under **Settings** > **Account Settings** > **Partner Profile** > Program info.</span></span>

6. <span data-ttu-id="a90a7-125">**[概要]** ページに、間接リセラー契約が表示されます。</span><span class="sxs-lookup"><span data-stu-id="a90a7-125">On your **Overview** page, you will see the indirect reseller agreement.</span></span> <span data-ttu-id="a90a7-126">**[Accept and continue] (同意して続ける)** を選びます。</span><span class="sxs-lookup"><span data-stu-id="a90a7-126">Select **Accept and continue**.</span></span> <span data-ttu-id="a90a7-127">この操作により、間接リセラーの機能が有効になります。</span><span class="sxs-lookup"><span data-stu-id="a90a7-127">This action enables the indirect reseller capabilities.</span></span>

<span data-ttu-id="a90a7-128">間接リセラー契約を受け入れるときは、パートナー プロファイルでは直接請求パートナーと間接リセラーの **両方** として示されていることに注意してください。</span><span class="sxs-lookup"><span data-stu-id="a90a7-128">When you have accepted the indirect reseller agreement, notice that your Partner profile identifies you as **both** a direct bill and indirect reseller.</span></span>

:::image type="content" source="images/direct/direct3.png" alt-text="間接リセラー契約":::

> [!IMPORTANT]
> <span data-ttu-id="a90a7-130">新しい機能を使用して間接リセラーとして登録した後は、直接請求のみのテナントにロールバックするオプションはありません。</span><span class="sxs-lookup"><span data-stu-id="a90a7-130">Once you enroll as an indirect reseller using the new capability, there is no option to roll back to a direct bill- only tenant.</span></span> <span data-ttu-id="a90a7-131">間接リセラーとして登録する前に、ビジネス ニーズを完全に評価していることを確認してください。</span><span class="sxs-lookup"><span data-stu-id="a90a7-131">Please make sure that you fully evaluate your business needs before enrolling as an indirect reseller.</span></span>

## <a name="while-you-transition-from-direct-to-indirect-reseller"></a><span data-ttu-id="a90a7-132">直接パートナーから間接リセラーへの移行中</span><span class="sxs-lookup"><span data-stu-id="a90a7-132">While you transition from direct to indirect reseller</span></span>

<span data-ttu-id="a90a7-133">このフェーズでは、課金プロセスを含め、お客様の直接のサブスクリプションのニーズを引き続き管理します。</span><span class="sxs-lookup"><span data-stu-id="a90a7-133">During this phase, you will continue to manage your direct customers' subscription needs including the billing process.</span></span> <span data-ttu-id="a90a7-134">同時に、間接プロバイダーからの顧客の受け入れを開始し、間接リセラーとして活動することもできます。</span><span class="sxs-lookup"><span data-stu-id="a90a7-134">You can also begin accepting customers from your Indirect provider and operating as an indirect reseller.</span></span>

:::image type="content" source="images/direct/direct4.png" alt-text="パートナーは、直接請求パートナーと間接リセラーの両方である":::

## <a name="find-an-indirect-provider"></a><span data-ttu-id="a90a7-136">間接プロバイダーの検索</span><span class="sxs-lookup"><span data-stu-id="a90a7-136">Find an indirect provider</span></span>

<span data-ttu-id="a90a7-137">登録が済むと、左側のナビゲーションに間接プロバイダーへのリンクが表示されます。</span><span class="sxs-lookup"><span data-stu-id="a90a7-137">After enrolling, a link to Indirect providers will appear in your left nav.</span></span> <span data-ttu-id="a90a7-138">間接リセラーとしてパートナーは、間接プロバイダーとの関係を確立し、その後は間接プロバイダーが、請求を処理し、顧客の製品を購入し、インフラストラクチャをサポートすることができます。</span><span class="sxs-lookup"><span data-stu-id="a90a7-138">As an indirect reseller you will establish a relationship with an indirect provider who then can handle your billing, purchase products for your customers, and support infrastructure.</span></span>

<span data-ttu-id="a90a7-139">提供されるサポートやサービスは間接プロバイダーによって異なるため、リセラーは対象地域の複数のプロバイダーを評価して、自社のニーズに最も適したプロバイダーを判断する必要があります。</span><span class="sxs-lookup"><span data-stu-id="a90a7-139">Different indirect providers offer different support and services, so you should evaluate the providers in your area to determine which ones best meet your needs.</span></span> <span data-ttu-id="a90a7-140">一般に、ほとんどのプロバイダーが提供している機能は次のとおりです。</span><span class="sxs-lookup"><span data-stu-id="a90a7-140">Generally, most providers will:</span></span>

- <span data-ttu-id="a90a7-141">リセラーへのテクニカル サポートの提供</span><span class="sxs-lookup"><span data-stu-id="a90a7-141">Provide you with technical training and assistance</span></span>
- <span data-ttu-id="a90a7-142">リセラーの製品やサービスのマーケティング支援</span><span class="sxs-lookup"><span data-stu-id="a90a7-142">Help you market your products and services</span></span>
- <span data-ttu-id="a90a7-143">財務および与信条件を管理する</span><span class="sxs-lookup"><span data-stu-id="a90a7-143">Manage your financing and credit terms</span></span>

<span data-ttu-id="a90a7-144">公式な [Microsoft 間接プロバイダー](https://partnercenter.microsoft.com/partner/find-a-provider)の一覧を検索してください。</span><span class="sxs-lookup"><span data-stu-id="a90a7-144">Search the list of official [Microsoft indirect providers](https://partnercenter.microsoft.com/partner/find-a-provider).</span></span>

<span data-ttu-id="a90a7-145">詳しくは、[間接プロバイダーとの提携](indirect-reseller-tasks-in-partner-center.md)に関する記事をご覧ください</span><span class="sxs-lookup"><span data-stu-id="a90a7-145">Learn more, read  [Partner with indirect providers](indirect-reseller-tasks-in-partner-center.md)</span></span>

## <a name="accept-a-partnership-invitation-from-your-indirect-provider"></a><span data-ttu-id="a90a7-146">間接プロバイダーからのパートナーシップへの招待を受け入れる</span><span class="sxs-lookup"><span data-stu-id="a90a7-146">Accept a partnership invitation from your indirect provider</span></span>

<span data-ttu-id="a90a7-147">提携する間接プロバイダーが見つかったら、パートナー センターで間接プロバイダーとのパートナーシップを確立します。</span><span class="sxs-lookup"><span data-stu-id="a90a7-147">When you find an indirect provider to partner with, establish a partnership with the indirect provider in Partner Center.</span></span>

<span data-ttu-id="a90a7-148">選択した間接プロバイダーから、パートナー センターで招待に移動するパートナーシップ招待リンクがメールで送られてきます。</span><span class="sxs-lookup"><span data-stu-id="a90a7-148">The indirect provider you select will send you in email a partnership invitation link that will take you to their invitation in Partner Center.</span></span> <span data-ttu-id="a90a7-149">必ず、グローバル管理者がパートナー センターにサインインして、招待リンクに従います。</span><span class="sxs-lookup"><span data-stu-id="a90a7-149">Be sure your global admin signs in to Partner Center and follows the invitation link.</span></span> <span data-ttu-id="a90a7-150">招待を受け入れると、プロバイダーの名前が間接プロバイダーの一覧に表示されます。</span><span class="sxs-lookup"><span data-stu-id="a90a7-150">When you accept the invitation, the provider's name will appear in your indirect provider list.</span></span>

## <a name="acquire-new-customers-as-indirect-reseller"></a><span data-ttu-id="a90a7-151">間接リセラーとして新しい顧客を獲得する</span><span class="sxs-lookup"><span data-stu-id="a90a7-151">Acquire new customers as indirect reseller</span></span>

<span data-ttu-id="a90a7-152">間接リセラーと間接プロバイダーの両方が、顧客との間にリセラーの関係を持つ必要があります。</span><span class="sxs-lookup"><span data-stu-id="a90a7-152">Both you and your indirect provider need to have reseller relationships with customers.</span></span> <span data-ttu-id="a90a7-153">これらの再販業者の関係により、顧客のサブスクリプションとサービスをユーザーの代理として管理することができます。</span><span class="sxs-lookup"><span data-stu-id="a90a7-153">These reseller relationships enable you to manage a customer's subscriptions and services on their behalf.</span></span> <span data-ttu-id="a90a7-154">既存の Azure AD テナントを持つ新しい顧客を獲得するには、貴社と貴社のプロバイダーの両方と同時にリセラーの関係を確立するよう、顧客を招待できます。</span><span class="sxs-lookup"><span data-stu-id="a90a7-154">To acquire a new customer who has an existing Azure AD tenant, you can invite the customer to establish a reseller relationship with both you and your provider at the same time.</span></span>

<span data-ttu-id="a90a7-155">間接リセラーの招待を作成するには:</span><span class="sxs-lookup"><span data-stu-id="a90a7-155">To create an indirect reseller invitation:</span></span>

1. <span data-ttu-id="a90a7-156">パートナー センターの左側のナビゲーションから **[間接プロバイダー]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="a90a7-156">Select **Indirect providers** from your Partner Center left nav.</span></span>

2. <span data-ttu-id="a90a7-157">貴社と間接プロバイダーの両方について再販業者関係を確立するために新しい顧客を招待するには、 **[新しい顧客を招待する]** を選びます。</span><span class="sxs-lookup"><span data-stu-id="a90a7-157">Select **Invite new customers** to invite a customer to establish a reseller relationship with both you and the indirect provider at the same time.</span></span> <span data-ttu-id="a90a7-158">プロバイダーは顧客との再販業者関係を持っている必要があるため、顧客が新しいサブスクリプションを購入したり、既存のサブスクリプションに新しいライセンスを追加したりするときに、顧客に代わって注文を送信することができます。</span><span class="sxs-lookup"><span data-stu-id="a90a7-158">The provider needs to have a reseller relationship with your customer, so they can submit orders on your customer's behalf when the customer wants to buy new subscriptions or add new licenses to existing subscriptions.</span></span>

3. <span data-ttu-id="a90a7-159">次のページで、メール メッセージの下書きを確認します。</span><span class="sxs-lookup"><span data-stu-id="a90a7-159">On the next page, review the draft email message.</span></span> <span data-ttu-id="a90a7-160">メールで下書きメッセージを開くか、メッセージをクリップボードにコピーし、メールに貼り付けます。</span><span class="sxs-lookup"><span data-stu-id="a90a7-160">You can open the draft message in email, or you can copy the message to your clipboard and paste it into an email.</span></span>

4. <span data-ttu-id="a90a7-161">電子メールのテキストを編集して必要なものを指定しますが、自分のアカウントとプロバイダーのアカウントの両方に顧客を直接接続できるように、パーソナライズされたリンクを含めてください。</span><span class="sxs-lookup"><span data-stu-id="a90a7-161">Edit the text in the email to say what you need but be sure to include the link as it is personalized to connect the customer directly to both your account and your provider's account.</span></span> <span data-ttu-id="a90a7-162">**[完了]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="a90a7-162">Then select **Done**.</span></span>

5. <span data-ttu-id="a90a7-163">顧客が貴社とプロバイダーを指名リセラーとして承認すると、貴社には顧客のサブスクリプション、ライセンス、ユーザーを管理するための管理者のアクセス許可が付与され、間接プロバイダーは、顧客に代わって注文を送信できるようになります。</span><span class="sxs-lookup"><span data-stu-id="a90a7-163">After the customer authorizes you and your provider to be their resellers of record, you'll have administrator permissions to manage their subscriptions, licenses, and users on their behalf, and your indirect provider will be able to submit orders on their behalf.</span></span>
6. <span data-ttu-id="a90a7-164">顧客のアカウント、サービス、ユーザー、ライセンスを管理するには、顧客の名前の下矢印を選んで、顧客のレコードを展開します。</span><span class="sxs-lookup"><span data-stu-id="a90a7-164">To manage the customer's account, services, users, and licenses, expand the customer's record by selecting the down arrow near their name.</span></span>

<span data-ttu-id="a90a7-165">ダイレクト請求パートナーとは異なり、間接リセラーは、パートナーセンターで新しい顧客用に Azure AD テナントを作成することはできません。</span><span class="sxs-lookup"><span data-stu-id="a90a7-165">Unlike direct bill partners, indirect resellers can't create Azure AD tenants for their new customers in Partner Center.</span></span> <span data-ttu-id="a90a7-166">プロバイダーがテナントを作成し、この顧客に対する間接リセラーとして貴社を指定します。</span><span class="sxs-lookup"><span data-stu-id="a90a7-166">Your provider will create the tenant and will specify you as the indirect reseller for this customer.</span></span> <span data-ttu-id="a90a7-167">これにより、顧客がパートナー センターの顧客リストに表示されます。</span><span class="sxs-lookup"><span data-stu-id="a90a7-167">This ensures that the customer will appear in your customer list in Partner Center.</span></span>

>[!Note]
><span data-ttu-id="a90a7-168">貴社は、直接請求機能を使用して、間接リセラーとして獲得した顧客の購入を作成することはできません。</span><span class="sxs-lookup"><span data-stu-id="a90a7-168">You will not be able to use your direct bill capability to create purchases for customers you acquire as an indirect reseller.</span></span>

## <a name="managing-your-direct-bill-customers-and-your-indirect-reseller-customers"></a><span data-ttu-id="a90a7-169">直接請求の顧客と間接リセラーの顧客を管理する</span><span class="sxs-lookup"><span data-stu-id="a90a7-169">Managing your direct bill customers and your indirect reseller customers</span></span>

<span data-ttu-id="a90a7-170">直接請求の顧客の管理と、間接リセラーの顧客の管理は異なります。</span><span class="sxs-lookup"><span data-stu-id="a90a7-170">You manage your direct bill customers and your indirect reseller customers differently.</span></span>

### <a name="direct-bill-customers-things-you-wont-do-as-an-indirect-reseller"></a><span data-ttu-id="a90a7-171">ダイレクト請求顧客 (間接リセラーとしては実行されません)</span><span class="sxs-lookup"><span data-stu-id="a90a7-171">Direct bill customers (things you won't do as an indirect reseller)</span></span>

- <span data-ttu-id="a90a7-172">製品の注文を作成します</span><span class="sxs-lookup"><span data-stu-id="a90a7-172">Create orders for products</span></span>
- <span data-ttu-id="a90a7-173">Azure の予約の管理</span><span class="sxs-lookup"><span data-stu-id="a90a7-173">Manage Azure reservations</span></span>
- <span data-ttu-id="a90a7-174">注文履歴を管理します</span><span class="sxs-lookup"><span data-stu-id="a90a7-174">Manage their order history</span></span>
- <span data-ttu-id="a90a7-175">ソフトウェアを購入します</span><span class="sxs-lookup"><span data-stu-id="a90a7-175">Purchase software</span></span>
- <span data-ttu-id="a90a7-176">顧客に直接請求します</span><span class="sxs-lookup"><span data-stu-id="a90a7-176">Bill customers directly</span></span>

### <a name="indirect-reseller-customers"></a><span data-ttu-id="a90a7-177">間接リセラーの顧客</span><span class="sxs-lookup"><span data-stu-id="a90a7-177">Indirect reseller customers</span></span>

- <span data-ttu-id="a90a7-178">間接プロバイダーが顧客の製品を注文します</span><span class="sxs-lookup"><span data-stu-id="a90a7-178">Your indirect provider orders products for your customers</span></span>
- <span data-ttu-id="a90a7-179">顧客のライセンスとユーザーを管理する</span><span class="sxs-lookup"><span data-stu-id="a90a7-179">Manage customers' licenses and users</span></span>
- <span data-ttu-id="a90a7-180">サブスクリプションの更新を処理します</span><span class="sxs-lookup"><span data-stu-id="a90a7-180">Handle subscription renewals</span></span>

### <a name="to-identify-customers-that-you-acquired-as-a-direct-bill-partner"></a><span data-ttu-id="a90a7-181">直接請求パートナーとして獲得した顧客を識別するには</span><span class="sxs-lookup"><span data-stu-id="a90a7-181">To identify customers that you acquired as a direct bill partner</span></span>

1. <span data-ttu-id="a90a7-182">**[顧客]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="a90a7-182">Select **Customers**.</span></span>

2. <span data-ttu-id="a90a7-183">顧客を選択すると、その詳細が表示されます。</span><span class="sxs-lookup"><span data-stu-id="a90a7-183">Select a customer to view their details.</span></span>

3. <span data-ttu-id="a90a7-184">この顧客が直接請求パートナーとして獲得した顧客である場合は、**製品を追加** または **表示** するためのオプションが表示され、そのサブスクリプションが表示されます。</span><span class="sxs-lookup"><span data-stu-id="a90a7-184">If this customer is one you acquired as a direct bill partner, you will see options to **add** or **view products** and you will see their subscriptions.</span></span>

4. <span data-ttu-id="a90a7-185">その顧客と貴社の間に間接リセラーの関係がある場合、これらのオプションは利用できません。</span><span class="sxs-lookup"><span data-stu-id="a90a7-185">If the customer has an indirect reseller relationship with you, those options will not be available.</span></span>

## <a name="move-your-direct-bill-customers-to-your-indirect-provider"></a><span data-ttu-id="a90a7-186">直接請求の顧客を間接プロバイダーに移動する</span><span class="sxs-lookup"><span data-stu-id="a90a7-186">Move your direct bill customers to your indirect provider</span></span>

<span data-ttu-id="a90a7-187">間接プロバイダーは、リセラー関係が築かれるまで、既存の直接請求顧客に対して注文または既存のサブスクリプション転送を送信することはできません。</span><span class="sxs-lookup"><span data-stu-id="a90a7-187">Your indirect provider cannot submit orders or existing subscription transfers for your existing direct bill customers until they have a reseller relationship with them.</span></span> <span data-ttu-id="a90a7-188">間接プロバイダーと既存の直接請求顧客の間でリセラー関係を確立するには、次のいずれかの方法を使用できます。</span><span class="sxs-lookup"><span data-stu-id="a90a7-188">To establish the reseller relationship between your indirect provider and your existing direct bill customer, you can use one of the following methods:</span></span>

- [<span data-ttu-id="a90a7-189">リセラーのリレーションシップ拡張機能</span><span class="sxs-lookup"><span data-stu-id="a90a7-189">Reseller relationship extension</span></span>](#reseller-relationship-extension)

- [<span data-ttu-id="a90a7-190">間接リセラーの招待を顧客に送信する</span><span class="sxs-lookup"><span data-stu-id="a90a7-190">Send an indirect reseller invitation to the customer</span></span>](#send-an-indirect-reseller-invitation-to-the-customer)

<span data-ttu-id="a90a7-191">詳細な手順の概要については、「直接から間接への切り替え [」ドキュメントを参照してください。](https://partner.microsoft.com/resources/collection/Direct-Bill-transition-to-Indirect-reseller#/)</span><span class="sxs-lookup"><span data-stu-id="a90a7-191">You can find a detailed overview of the step-by-step process in the [Direct to indirect transition document](https://partner.microsoft.com/resources/collection/Direct-Bill-transition-to-Indirect-reseller#/)</span></span>

### <a name="reseller-relationship-extension"></a><span data-ttu-id="a90a7-192">リセラーのリレーションシップ拡張機能</span><span class="sxs-lookup"><span data-stu-id="a90a7-192">Reseller relationship extension</span></span>

<span data-ttu-id="a90a7-193">リセラーリレーションシップ拡張機能を使用して、既存の直接請求顧客と間接プロバイダーとの間にリセラー関係を確立するには、ダッシュボードパートナー センター使用します。</span><span class="sxs-lookup"><span data-stu-id="a90a7-193">You can use the reseller relationship extension feature to establish reseller relationship between your existing direct bill customers and your indirect provider using Partner Center Dashboard.</span></span> <span data-ttu-id="a90a7-194">機能を使用する前に、次の点に注意してください。</span><span class="sxs-lookup"><span data-stu-id="a90a7-194">Before using the feature, note the following:</span></span>

- <span data-ttu-id="a90a7-195">この機能は、間接リセラーに移行する直接請求パートナーが間接リセラー登録 を完了 [した場合にのみ使用できます](#get-started)。</span><span class="sxs-lookup"><span data-stu-id="a90a7-195">This feature is only available to direct bill partners who are transitioning to become an indirect reseller have completed the [indirect reseller enrollment](#get-started).</span></span>

- <span data-ttu-id="a90a7-196">この機能は、既存の直接請求顧客にのみ適用できます。</span><span class="sxs-lookup"><span data-stu-id="a90a7-196">You can only apply this feature to existing direct bill customers.</span></span> <span data-ttu-id="a90a7-197">間接リセラーのお客様 [には適用できません](#acquire-new-customers-as-indirect-reseller)。</span><span class="sxs-lookup"><span data-stu-id="a90a7-197">It is not applicable to [indirect reseller customers](#acquire-new-customers-as-indirect-reseller).</span></span>

- <span data-ttu-id="a90a7-198">間接プロバイダーからのパートナー招待を受け入れた間接プロバイダー [のみを選択できます](#accept-a-partnership-invitation-from-your-indirect-provider)。</span><span class="sxs-lookup"><span data-stu-id="a90a7-198">You can only select an indirect provider for which you have [accepted a partner invitation from your indirect provider](#accept-a-partnership-invitation-from-your-indirect-provider).</span></span>

- <span data-ttu-id="a90a7-199">この顧客に対して持っている請求情報のコピーは、間接プロバイダーが利用できます。</span><span class="sxs-lookup"><span data-stu-id="a90a7-199">A copy of the bill-to info you have for this customer will be made available to the indirect provider.</span></span> <span data-ttu-id="a90a7-200">請求情報には、この顧客の [アカウント] ページにアクセスして、[ダッシュボード] パートナー センターできます。</span><span class="sxs-lookup"><span data-stu-id="a90a7-200">You can access the bill-to info by accessing the Account page for this customer in Partner Center Dashboard.</span></span>

    > [!NOTE]
    > <span data-ttu-id="a90a7-201">リセラーのリレーションシップ拡張機能を使用すると、間接プロバイダーとこの顧客に対して持っている請求情報を共有できます。</span><span class="sxs-lookup"><span data-stu-id="a90a7-201">By using the reseller relationship extension feature, you consent to sharing the bill-to info you have for this customer with the indirect provider.</span></span>

- <span data-ttu-id="a90a7-202">間接プロバイダーには、顧客テナントに委任 [された管理特権](customers-revoke-admin-privileges.md) は付与されません。</span><span class="sxs-lookup"><span data-stu-id="a90a7-202">Your indirect provider will not be provided with [delegated administration privileges](customers-revoke-admin-privileges.md) to the customer tenant.</span></span> <span data-ttu-id="a90a7-203">間接プロバイダーに委任された管理特権が必要な場合は、代わりに間接リセラーの招待を顧客に送信する必要があります。</span><span class="sxs-lookup"><span data-stu-id="a90a7-203">If your indirect provider requires delegated administration privileges, you must send an indirect reseller invitation to the customer instead.</span></span>

- <span data-ttu-id="a90a7-204">再販業者の関係が確立されると、間接プロバイダーは、 [Microsoft 365 管理センター](https://admin.microsoft.com/AdminPortal/Home#/partners) の [パートナー関係] ページおよび [ [Microsoft Store for Business](/microsoft-store/work-with-partner-microsoft-store-business)] の下にある顧客に対して、CSP パートナーとして表示されます。</span><span class="sxs-lookup"><span data-stu-id="a90a7-204">Once the reseller relationship is established, the indirect provider will appear as a CSP partner to the customer under the Partner Relationships page in [Microsoft 365 Admin Center](https://admin.microsoft.com/AdminPortal/Home#/partners) and [Microsoft Store for Business](/microsoft-store/work-with-partner-microsoft-store-business).</span></span>

    > [!IMPORTANT]
    > <span data-ttu-id="a90a7-205">混乱や誤解を避けるために、パートナー契約によって契約必要は、取引先との関係拡張機能を使用して、既存の直接請求顧客と間接プロバイダーの間に再販業者の関係を確立する前に、お客様に直接請求を通知し、同意を得ることができます。</span><span class="sxs-lookup"><span data-stu-id="a90a7-205">To avoid confusion and misunderstanding, you are contractually obliged by your partner agreement to inform and obtain consent from the direct bill customer before you use the relationship extension feature to establish reseller relationship between an existing direct bill customer and an indirect provider.</span></span>

<span data-ttu-id="a90a7-206">既存の顧客テナントでこの機能を使用するには、次のようにします。</span><span class="sxs-lookup"><span data-stu-id="a90a7-206">To use this feature on an existing customer tenant:</span></span>

1. <span data-ttu-id="a90a7-207">**管理エージェント** としてパートナーセンターにログインします。</span><span class="sxs-lookup"><span data-stu-id="a90a7-207">Log in to Partner Center as an **Admin Agent**.</span></span>

2. <span data-ttu-id="a90a7-208">[ **Customers] ページ** で、既存の顧客を選択し、その **クイックリンク** アイコンをクリックして、顧客の概要ビューを展開します。</span><span class="sxs-lookup"><span data-stu-id="a90a7-208">In the **Customers page**, select an existing customer and click on its **Quick links** icon to expand the summary view of the customer.</span></span>

3. <span data-ttu-id="a90a7-209">[ **間接プロバイダー**] で、[ **間接プロバイダーの顧客の転送**] をクリックします。</span><span class="sxs-lookup"><span data-stu-id="a90a7-209">Under **Indirect provider(s)**, click **Transfer customer on an indirect provider**.</span></span>

    :::image type="content" source="images/direct/direct5-1.png" alt-text="顧客を間接プロバイダーに転送する":::

4. <span data-ttu-id="a90a7-211">ポップアップダイアログで、リセラーと顧客との関係を設定する **間接プロバイダー** を選択します。</span><span class="sxs-lookup"><span data-stu-id="a90a7-211">In the pop-up dialog, select the **Indirect Provider** you would like to have reseller relationship with the customer.</span></span>

5. <span data-ttu-id="a90a7-212">**保存して続行** をクリックします。</span><span class="sxs-lookup"><span data-stu-id="a90a7-212">Click **Save and continue**.</span></span>

6. <span data-ttu-id="a90a7-213">選択した間接プロバイダーが **間接プロバイダー** の下に表示されることを確認します。</span><span class="sxs-lookup"><span data-stu-id="a90a7-213">Verify the selected indirect provider shows up under **Indirect provider(s)**.</span></span>

    :::image type="content" source="images/direct/direct5-2.png" alt-text="間接プロバイダーの一覧":::

### <a name="send-an-indirect-reseller-invitation-to-the-customer"></a><span data-ttu-id="a90a7-215">間接リセラー招待を顧客に送信する</span><span class="sxs-lookup"><span data-stu-id="a90a7-215">Send an indirect reseller invitation to the customer</span></span>

<span data-ttu-id="a90a7-216">間接プロバイダーは、再販業者とパートナー関係がある場合に、既存の直接請求先の顧客の注文を送信することはできません。</span><span class="sxs-lookup"><span data-stu-id="a90a7-216">Your indirect provider cannot submit orders for your existing direct bill customers until they have a reseller relationship with them.</span></span> <span data-ttu-id="a90a7-217">既存の顧客と間接プロバイダーの間にリセラーの関係を確立するには、間接リセラーの招待を使用して顧客を招待します。</span><span class="sxs-lookup"><span data-stu-id="a90a7-217">To establish the reseller relationship between your existing customers and your indirect provider, invite the customer using an indirect reseller invitation.</span></span>

1. <span data-ttu-id="a90a7-218">パートナー センターの左側のナビゲーションから **[間接プロバイダー]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="a90a7-218">Select **Indirect providers** from your Partner Center left nav.</span></span>

2. <span data-ttu-id="a90a7-219">貴社と間接プロバイダーの両方について再販業者関係を確立するために新しい顧客を招待するには、 **[新しい顧客を招待する]** を選びます。</span><span class="sxs-lookup"><span data-stu-id="a90a7-219">Select **Invite new customers** to invite a customer to establish a reseller relationship with both you and the indirect provider at the same time.</span></span> <span data-ttu-id="a90a7-220">プロバイダーは顧客との再販業者関係を持っている必要があるため、顧客が新しいサブスクリプションを購入したり、既存のサブスクリプションに新しいライセンスを追加したりするときに、顧客に代わって注文を送信することができます。</span><span class="sxs-lookup"><span data-stu-id="a90a7-220">The provider needs to have a reseller relationship with your customer, so they can submit orders on your customer's behalf when the customer wants to buy new subscriptions or add new licenses to existing subscriptions.</span></span>

    :::image type="content" source="images/direct/direct6.png" alt-text="新しい顧客を招待する":::

3. <span data-ttu-id="a90a7-222">次のページで、メール メッセージの下書きを確認します。</span><span class="sxs-lookup"><span data-stu-id="a90a7-222">On the next page, review the draft email message.</span></span> <span data-ttu-id="a90a7-223">メールで下書きメッセージを開くか、メッセージをクリップボードにコピーし、メールに貼り付けます。</span><span class="sxs-lookup"><span data-stu-id="a90a7-223">You can open the draft message in email, or you can copy the message to your clipboard and paste it into an email.</span></span>

4. <span data-ttu-id="a90a7-224">電子メールのテキストを編集して必要なものを指定しますが、自分のアカウントとプロバイダーのアカウントの両方に顧客を直接接続できるように、パーソナライズされたリンクを含めてください。</span><span class="sxs-lookup"><span data-stu-id="a90a7-224">Edit the text in the email to say what you need but be sure to include the link as it is personalized to connect the customer directly to both your account and your provider's account.</span></span> <span data-ttu-id="a90a7-225">**[完了]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="a90a7-225">Then select **Done**.</span></span>

5. <span data-ttu-id="a90a7-226">顧客が貴社とプロバイダーを指名リセラーとして承認すると、貴社には顧客のサブスクリプション、ライセンス、ユーザーを管理するための管理者のアクセス許可が付与され、間接プロバイダーは、顧客に代わって注文を送信できるようになります。</span><span class="sxs-lookup"><span data-stu-id="a90a7-226">After the customer authorizes you and your provider to be their resellers of record, you'll have administrator permissions to manage their subscriptions, licenses, and users on their behalf, and your indirect provider will be able to submit orders on their behalf.</span></span>

6. <span data-ttu-id="a90a7-227">顧客のアカウント、サービス、ユーザー、ライセンスを管理するには、顧客の名前の下矢印を選んで、顧客のレコードを展開します。</span><span class="sxs-lookup"><span data-stu-id="a90a7-227">To manage the customer's account, services, users, and licenses, expand the customer's record by selecting the down arrow near their name.</span></span>

### <a name="microsoft-customer-agreement-acceptance"></a><span data-ttu-id="a90a7-228">Microsoft カスタマーアグリーメントへの同意</span><span class="sxs-lookup"><span data-stu-id="a90a7-228">Microsoft Customer Agreement acceptance</span></span>

<span data-ttu-id="a90a7-229">Microsoft Cloud Agreement は、2020年1月31日まで有効です。</span><span class="sxs-lookup"><span data-stu-id="a90a7-229">Microsoft Cloud Agreement is valid until January 31, 2020.</span></span> <span data-ttu-id="a90a7-230">その後、すべてのお客様 (既存および新規) は、新しい [Microsoft カスタマー契約](confirm-customer-agreement.md)に署名する必要があります。</span><span class="sxs-lookup"><span data-stu-id="a90a7-230">After that date, all customers, existing and new, must sign the new [Microsoft Customer Agreement](confirm-customer-agreement.md).</span></span> <span data-ttu-id="a90a7-231">お客様の移行の場合:</span><span class="sxs-lookup"><span data-stu-id="a90a7-231">For transitioning customers, if:</span></span>

- <span data-ttu-id="a90a7-232">**お客様はまだ Microsoft カスタマーアグリーメントに同意していません**</span><span class="sxs-lookup"><span data-stu-id="a90a7-232">**Customer has not accepted Microsoft Customer Agreement yet**</span></span>

   <span data-ttu-id="a90a7-233">間接プロバイダーと協力して、お客様が [Microsoft カスタマーアグリーメントに同意](confirm-customer-agreement.md)するようにしてください。</span><span class="sxs-lookup"><span data-stu-id="a90a7-233">Please work with Indirect Provider to have customer [accept the Microsoft Customer Agreement](confirm-customer-agreement.md).</span></span>

- <span data-ttu-id="a90a7-234">**お客様は、Microsoft 365 管理センターを通じて Microsoft カスタマーアグリーメントに同意しました**</span><span class="sxs-lookup"><span data-stu-id="a90a7-234">**Customer has accepted Microsoft Customer Agreement with you through the Microsoft 365 Admin Center**</span></span>

   <span data-ttu-id="a90a7-235">間接プロバイダーとの再販業者の関係が確立されると、受け入れが維持されます。</span><span class="sxs-lookup"><span data-stu-id="a90a7-235">The acceptance will be retained once the reseller relationship is established with the Indirect Provider.</span></span> <span data-ttu-id="a90a7-236">何もする必要はありません。</span><span class="sxs-lookup"><span data-stu-id="a90a7-236">There is nothing you need to do.</span></span>

- <span data-ttu-id="a90a7-237">**お客様がパートナーの構成証明を通じて Microsoft カスタマーアグリーメントに同意しました**</span><span class="sxs-lookup"><span data-stu-id="a90a7-237">**Customer has accepted Microsoft Customer Agreement with you through partner attestation**</span></span>

   <span data-ttu-id="a90a7-238">受け入れは保持されません。</span><span class="sxs-lookup"><span data-stu-id="a90a7-238">The acceptance will not be retained.</span></span> <span data-ttu-id="a90a7-239">[パートナーセンターでお客様の同意を更新するには、](confirm-customer-agreement.md#confirm-customer-acceptance-for-existing-customers)間接プロバイダーと協力してください。</span><span class="sxs-lookup"><span data-stu-id="a90a7-239">Please work with Indirect Provider to [update the customer's acceptance in Partner Center](confirm-customer-agreement.md#confirm-customer-acceptance-for-existing-customers).</span></span>

## <a name="transfer-existing-direct-bill-subscriptions-to-indirect-provider"></a><span data-ttu-id="a90a7-240">既存の直接請求書のサブスクリプションを間接プロバイダーに転送する</span><span class="sxs-lookup"><span data-stu-id="a90a7-240">Transfer existing direct bill subscriptions to indirect provider</span></span>

<span data-ttu-id="a90a7-241">CSP 間接モデルでは、間接リセラーには Microsoft との請求関係がありません。</span><span class="sxs-lookup"><span data-stu-id="a90a7-241">Under CSP indirect model, indirect resellers do not have billing relationships with Microsoft.</span></span> <span data-ttu-id="a90a7-242">間接リセラーは、間接プロバイダーを通じて顧客のサブスクリプションを取得します。</span><span class="sxs-lookup"><span data-stu-id="a90a7-242">Instead, indirect resellers obtain subscriptions for their customers through their indirect providers.</span></span> <span data-ttu-id="a90a7-243">ダイレクト請求パートナーから間接リセラーに移行している間は、直接請求パートナーとして所有している既存のサブスクリプションを間接プロバイダーに譲渡する必要があります。</span><span class="sxs-lookup"><span data-stu-id="a90a7-243">While transitioning from direct bill partner to indirect reseller, you need to transfer the existing subscriptions you have as the direct bill partner to your indirect provider.</span></span> <span data-ttu-id="a90a7-244">パートナーセンターダッシュボードのセルフサービスサブスクリプション転送機能を使用して、これを行うことができます。</span><span class="sxs-lookup"><span data-stu-id="a90a7-244">You can use the self-served subscription transfer feature in Partner Center Dashboard to do so.</span></span>

### <a name="prerequisites"></a><span data-ttu-id="a90a7-245">前提条件</span><span class="sxs-lookup"><span data-stu-id="a90a7-245">Prerequisites</span></span>

- <span data-ttu-id="a90a7-246">この機能は、既存の直接請求パートナーテナントを使用して間接リセラーの登録を完了したパートナーを移行する場合にのみ使用できます。</span><span class="sxs-lookup"><span data-stu-id="a90a7-246">This feature is only available to transitioning partners who have completed the indirect reseller enrollment using their existing direct bill partner tenants.</span></span>

- <span data-ttu-id="a90a7-247">特定の顧客に関連付けられているサブスクリプションを転送する前に、移行パートナーは顧客を間接プロバイダーに移動する必要があります。</span><span class="sxs-lookup"><span data-stu-id="a90a7-247">Before transferring subscriptions associated with a given customer, the transitioning partner must move the customer to an indirect provider.</span></span>

- <span data-ttu-id="a90a7-248">お客様は [、間接プロバイダーを通じて Microsoft カスタマー契約に同意](#microsoft-customer-agreement-acceptance)している必要があります。</span><span class="sxs-lookup"><span data-stu-id="a90a7-248">Customer must have [accepted Microsoft Customer Agreement through the Indirect Provider](#microsoft-customer-agreement-acceptance).</span></span>

### <a name="how-to-transition-to-indirect-reseller-status"></a><span data-ttu-id="a90a7-249">間接リセラーの状態に移行する方法</span><span class="sxs-lookup"><span data-stu-id="a90a7-249">How to transition to indirect reseller status</span></span>

<span data-ttu-id="a90a7-250">この機能は、4つの手順からなるプロセスです。</span><span class="sxs-lookup"><span data-stu-id="a90a7-250">The feature is a 4-step process, where:</span></span>

- <span data-ttu-id="a90a7-251">遷移中のパートナーは、サブスクリプションの譲渡要求を作成します。</span><span class="sxs-lookup"><span data-stu-id="a90a7-251">The transitioning partner creates a subscription transfer request.</span></span> <span data-ttu-id="a90a7-252">要求には、同じ顧客に関連付けられている 1 つ以上の既存のサブスクリプションが含まれているので、間接プロバイダーに対応しています。</span><span class="sxs-lookup"><span data-stu-id="a90a7-252">The request contains one or more existing subscriptions associated with the same customer and is addressed to an indirect provider.</span></span>

- <span data-ttu-id="a90a7-253">間接プロバイダーは、転送要求を確認して受け入れる (または拒否) します。</span><span class="sxs-lookup"><span data-stu-id="a90a7-253">The indirect provider reviews and accepts (or reject) the transfer request.</span></span>

- <span data-ttu-id="a90a7-254">間接プロバイダーは、転送要求が完了したと確認します。</span><span class="sxs-lookup"><span data-stu-id="a90a7-254">The indirect provider verifies that the transfer request is complete.</span></span>

- <span data-ttu-id="a90a7-255">移行パートナーは、転送要求が完了したと確認します。</span><span class="sxs-lookup"><span data-stu-id="a90a7-255">The transitioning partner verifies that the transfer request is complete.</span></span>

### <a name="transitioning-partner"></a><span data-ttu-id="a90a7-256">移行パートナー</span><span class="sxs-lookup"><span data-stu-id="a90a7-256">Transitioning partner</span></span>

> [!NOTE]
> <span data-ttu-id="a90a7-257">また [、API/SDK パートナー センターを使用して](/partner-center/develop/manage-customers) 、既存のサブスクリプションを間接プロバイダーに転送することもできます。</span><span class="sxs-lookup"><span data-stu-id="a90a7-257">You can also use [Partner Center API/SDK](/partner-center/develop/manage-customers) to transfer the existing subscriptions to your indirect provider.</span></span>
>
> - [<span data-ttu-id="a90a7-258">顧客のサブスクリプション譲渡の資格を取得する</span><span class="sxs-lookup"><span data-stu-id="a90a7-258">Get a customer's subscriptions transfer eligibility</span></span>](/partner-center/develop/get-customer-s-subscriptions-transfer-eligibility)
> - [<span data-ttu-id="a90a7-259">顧客からの譲渡を作成する</span><span class="sxs-lookup"><span data-stu-id="a90a7-259">Create a customer's transfer</span></span>](/partner-center/develop/create-a-transfer)
> - [<span data-ttu-id="a90a7-260">顧客の譲渡を撤回する</span><span class="sxs-lookup"><span data-stu-id="a90a7-260">Withdraw a customer's transfer</span></span>](/partner-center/develop/withdraw-a-transfer)
> - [<span data-ttu-id="a90a7-261">顧客の譲渡を承諾する</span><span class="sxs-lookup"><span data-stu-id="a90a7-261">Accept a customer's transfer</span></span>](/partner-center/develop/accept-a-transfer)
> - [<span data-ttu-id="a90a7-262">顧客の譲渡を拒否する</span><span class="sxs-lookup"><span data-stu-id="a90a7-262">Reject a Customer's transfer</span></span>](/partner-center/develop/reject-a-transfer)
> - [<span data-ttu-id="a90a7-263">顧客の譲渡を取得する</span><span class="sxs-lookup"><span data-stu-id="a90a7-263">Get a customer's transfers</span></span>](/partner-center/develop/get-all-of-a-customer-s-transfers)
> - [<span data-ttu-id="a90a7-264">ID で転送の詳細を取得する</span><span class="sxs-lookup"><span data-stu-id="a90a7-264">Get transfer details by id</span></span>](/partner-center/develop/get-transfer-by-id)

### <a name="transitioning-partner---create-transfer-request"></a><span data-ttu-id="a90a7-265">移行パートナー - 譲渡要求の作成</span><span class="sxs-lookup"><span data-stu-id="a90a7-265">Transitioning partner - create transfer request</span></span>

<span data-ttu-id="a90a7-266">移行パートナーとして譲渡要求を作成するには:</span><span class="sxs-lookup"><span data-stu-id="a90a7-266">To create a transfer request as the transitioning partner:</span></span>

1. <span data-ttu-id="a90a7-267">管理エージェント としてパートナー センターに **ログインします**。</span><span class="sxs-lookup"><span data-stu-id="a90a7-267">Log in to Partner Center as an **Admin Agent**.</span></span>

2. <span data-ttu-id="a90a7-268">[顧客 **] ページ** で目的の顧客を選択し、[クイック リンク] アイコンをクリックして顧客の概要ビューを展開します。</span><span class="sxs-lookup"><span data-stu-id="a90a7-268">In the **Customers** page, select the intended customer and click on the Quick links icon to expand the summary view of the customer.</span></span>

3. <span data-ttu-id="a90a7-269">[ **間接プロバイダー] で、** 目的の間接プロバイダーが一覧に表示されます。</span><span class="sxs-lookup"><span data-stu-id="a90a7-269">Under **Indirect provider(s)**, confirm that the intended indirect provider is listed.</span></span>

4. <span data-ttu-id="a90a7-270">[サブスクリプション **の表示] をクリックします**。</span><span class="sxs-lookup"><span data-stu-id="a90a7-270">Click **View Subscriptions**.</span></span>

5. <span data-ttu-id="a90a7-271">[サブスクリプション **] ページで** 、サブスクリプション転送 を **探します**。</span><span class="sxs-lookup"><span data-stu-id="a90a7-271">In the **Subscriptions** page, look for **Subscription Transfer**.</span></span>

6. <span data-ttu-id="a90a7-272">[サブスクリプション **の転送] の**[サブスクリプション転送 **の要求] をクリックします**。</span><span class="sxs-lookup"><span data-stu-id="a90a7-272">Under **Subscription Transfer**, click **Request subscription transfer**.</span></span>

    :::image type="content" source="images/direct/direct8.png" alt-text="サブスクリプションの譲渡を要求する":::

7. <span data-ttu-id="a90a7-274">[転送要求] ダイアログで、転送する 1 つ以上のサブスクリプションを選択します。</span><span class="sxs-lookup"><span data-stu-id="a90a7-274">In the transfer request dialog, select one or more subscriptions to be transferred.</span></span>

    :::image type="content" source="images/direct/direct9.png" alt-text="転送要求の作成":::

8. <span data-ttu-id="a90a7-276">**Create** をクリックしてください。</span><span class="sxs-lookup"><span data-stu-id="a90a7-276">Click **Create**.</span></span>

9. <span data-ttu-id="a90a7-277">アクティブなサブスクリプション転送要求が [サブスクリプション転送] に **表示されます**。</span><span class="sxs-lookup"><span data-stu-id="a90a7-277">An active subscription transfer request will appear under **Subscription Transfer**.</span></span>

    :::image type="content" source="images/direct/direct10.png" alt-text="要求一覧の転送":::

10. <span data-ttu-id="a90a7-279">サブスクリプションへの譲渡要求が作成されたことを間接プロバイダーに通知します。</span><span class="sxs-lookup"><span data-stu-id="a90a7-279">Inform your indirect provider that you have created a subscription transfer request to them.</span></span>

### <a name="indirect-provider---accept-transfer-request"></a><span data-ttu-id="a90a7-280">間接プロバイダー-転送要求の受け入れ</span><span class="sxs-lookup"><span data-stu-id="a90a7-280">Indirect provider - accept transfer request</span></span>

<span data-ttu-id="a90a7-281">間接プロバイダーとして転送要求を確認して受け入れるには、次のようにします。</span><span class="sxs-lookup"><span data-stu-id="a90a7-281">To review and accept a transfer request as the indirect provider:</span></span>

1. <span data-ttu-id="a90a7-282">管理エージェントまたは **営業担当\*\*\*\*者** としてパートナーセンターにログインします。</span><span class="sxs-lookup"><span data-stu-id="a90a7-282">Log in to Partner Center as an **Admin** Agent or **Sales Agent**.</span></span>

2. <span data-ttu-id="a90a7-283">[ **Customers** ] ページで、目的の顧客を選択し、そのクイックリンクアイコンをクリックして、顧客の概要ビューを展開します。</span><span class="sxs-lookup"><span data-stu-id="a90a7-283">In the **Customers** page, select the intended customer and click on its Quick links icon to expand the summary view of the customer.</span></span>

3. <span data-ttu-id="a90a7-284">[ **間接リセラー**] の下に、[移行パートナー] が表示されていることを確認します。</span><span class="sxs-lookup"><span data-stu-id="a90a7-284">Under **Indirect reseller(s)**, confirm the transitioning partner is listed.</span></span>

4. <span data-ttu-id="a90a7-285">[ **サブスクリプションの表示**] をクリックします。</span><span class="sxs-lookup"><span data-stu-id="a90a7-285">Click **View Subscriptions**.</span></span>

5. <span data-ttu-id="a90a7-286">[ **サブスクリプション** ] ページで、[ **サブスクリプションの譲渡**] を探します。</span><span class="sxs-lookup"><span data-stu-id="a90a7-286">In the **Subscriptions** page, look for **Subscription Transfer**.</span></span>

    :::image type="content" source="images/direct/direct11.png" alt-text="転送要求の表示":::

6. <span data-ttu-id="a90a7-288">[ **サブスクリプションの譲渡**] で、[転送要求] をクリックして確認します。</span><span class="sxs-lookup"><span data-stu-id="a90a7-288">Under **Subscription Transfer**, click on the transfer request to review.</span></span>

7. <span data-ttu-id="a90a7-289">必要に応じて、[ **承諾** ] (または [ **拒否**]) をクリックします。</span><span class="sxs-lookup"><span data-stu-id="a90a7-289">Click **Accept** (or **Reject**) as appropriate.</span></span>

    :::image type="content" source="images/direct/direct12.png" alt-text="譲渡要求の受け入れ":::

8. <span data-ttu-id="a90a7-291">転送要求が完了するまで待ちます。</span><span class="sxs-lookup"><span data-stu-id="a90a7-291">Wait for the transfer request to complete.</span></span>

### <a name="indirect-provider---verify-transfer-request-is-complete"></a><span data-ttu-id="a90a7-292">間接プロバイダー-転送要求の確認が完了しました</span><span class="sxs-lookup"><span data-stu-id="a90a7-292">Indirect provider - verify transfer request is complete</span></span>

1. <span data-ttu-id="a90a7-293">転送要求が正常に完了したら、サブスクリプションが [ **サブスクリプション**] の下に表示されることを確認します。</span><span class="sxs-lookup"><span data-stu-id="a90a7-293">After the transfer request is completed successfully, verify that you can see the subscriptions appear under **Subscriptions**.</span></span>

2. <span data-ttu-id="a90a7-294">移行パートナーに通知します。</span><span class="sxs-lookup"><span data-stu-id="a90a7-294">Inform the transitioning partner.</span></span>

### <a name="transitioning-partner---verify-transfer-request-is-complete"></a><span data-ttu-id="a90a7-295">パートナーの移行-転送要求の確認が完了しました</span><span class="sxs-lookup"><span data-stu-id="a90a7-295">Transitioning partner - verify transfer request is complete</span></span>

<span data-ttu-id="a90a7-296">移行中のパートナーは、次の操作を行う必要があります。</span><span class="sxs-lookup"><span data-stu-id="a90a7-296">The transitioning partner should do the following:</span></span>

1. <span data-ttu-id="a90a7-297">**管理エージェント** または **営業担当** 者としてパートナーセンターにサインインします。</span><span class="sxs-lookup"><span data-stu-id="a90a7-297">Sign into Partner Center as an **Admin Agent** or **Sales Agent**.</span></span>

2. <span data-ttu-id="a90a7-298">[顧客 **] ページ** で目的の顧客を選択し、[クイック リンク] アイコンをクリックして顧客の概要ビューを展開します。</span><span class="sxs-lookup"><span data-stu-id="a90a7-298">In the **Customers** page, select the intended customer and click on the **Quick links** icon to expand the summary view of the customer.</span></span>

3. <span data-ttu-id="a90a7-299">[サブスクリプション **の表示] をクリックします**。</span><span class="sxs-lookup"><span data-stu-id="a90a7-299">Click **View Subscriptions**.</span></span>

4. <span data-ttu-id="a90a7-300">[サブスクリプション **] ページで** 、サブスクリプション転送 を **探します**。</span><span class="sxs-lookup"><span data-stu-id="a90a7-300">In the **Subscriptions** page, look for **Subscription Transfer**.</span></span>

5. <span data-ttu-id="a90a7-301">転送要求が [完了] としてマークされているのを **確認します**。</span><span class="sxs-lookup"><span data-stu-id="a90a7-301">Verify that the transfer request is marked as **Complete**.</span></span>

6. <span data-ttu-id="a90a7-302">[サブスクリプション] ページで、サブスクリプションがアクティブとして表示されなくなった **か確認** します。</span><span class="sxs-lookup"><span data-stu-id="a90a7-302">Verify that the subscription(s) no longer appear as active in the **Subscriptions** page:</span></span>

   1. <span data-ttu-id="a90a7-303">これが Azure サブスクリプション (MS-AZR-0145P) の場合は、一覧に表示されなくなりました。</span><span class="sxs-lookup"><span data-stu-id="a90a7-303">If this is an Azure subscription (MS-AZR-0145P), it will no longer be listed.</span></span>

   2. <span data-ttu-id="a90a7-304">これがライセンス ベースのサブスクリプション (Office 365、Dynamics、Intune) の場合は、状態が [中断] と **表示されます**。</span><span class="sxs-lookup"><span data-stu-id="a90a7-304">If this is a license-based subscription (Office 365, Dynamics, Intune), it will be listed with state as **Suspended**.</span></span>

   :::image type="content" source="images/direct/direct13.png" alt-text="サブスクリプションの中断":::

### <a name="considerations"></a><span data-ttu-id="a90a7-306">考慮事項</span><span class="sxs-lookup"><span data-stu-id="a90a7-306">Considerations</span></span>

- <span data-ttu-id="a90a7-307">**譲渡後、サブスクリプション ID は異なります。**</span><span class="sxs-lookup"><span data-stu-id="a90a7-307">**Subscription ID will be different after transfer.**</span></span> <span data-ttu-id="a90a7-308">Azure サブスクリプション (MS-AZR-0145P) の場合は、前の所有者から保持されている Azure サブスクリプション ID が保持され、Azure 管理ポータルに表示されます。</span><span class="sxs-lookup"><span data-stu-id="a90a7-308">If it is an Azure subscription (MS-AZR-0145P), additionally, it will have an Azure Subscription ID, which is retained from the previous owner, and will appear in the Azure management portal.</span></span>

- <span data-ttu-id="a90a7-309">**同じサブスクリプションを複数の転送要求で参照することはできません。**</span><span class="sxs-lookup"><span data-stu-id="a90a7-309">**The same subscription cannot be referenced by multiple transfer requests.**</span></span> <span data-ttu-id="a90a7-310">既存のサブスクリプションを含む譲渡要求を作成した後は、最初の譲渡要求が取り消されるまで、同じサブスクリプションを含む追加の転送要求を作成することはできません。</span><span class="sxs-lookup"><span data-stu-id="a90a7-310">After you have created a transfer request, which includes an existing subscription, you cannot create additional transfer requests including the same subscription, until the first transfer request is canceled.</span></span>

- <span data-ttu-id="a90a7-311">**ライセンス ベースのサブスクリプションのアドオンは、基本サブスクリプションと共に転送する必要があります。**</span><span class="sxs-lookup"><span data-stu-id="a90a7-311">**Add-ons for license-based subscriptions must be transferred along with their base subscription.**</span></span> <span data-ttu-id="a90a7-312">譲渡要求を作成するときに、1 つ以上のアドオンを含む既存のサブスクリプションを選択した場合、アドオンは自動的に転送要求に含まれます。</span><span class="sxs-lookup"><span data-stu-id="a90a7-312">When creating a transfer request, if you pick an existing subscription with one or more add-ons, the add-ons will automatically be included in the transfer request.</span></span>

- <span data-ttu-id="a90a7-313">**サブスクリプションに対するライセンス数の変更は、既存の譲渡要求には反映されません。**</span><span class="sxs-lookup"><span data-stu-id="a90a7-313">**License count changes to a subscription will not be reflected in existing transfer request.**</span></span> <span data-ttu-id="a90a7-314">既存のサブスクリプションを含む譲渡要求を作成した後は、サブスクリプション (または関連付けられているアドオン) のライセンス数量を更新しないようにする必要があります。</span><span class="sxs-lookup"><span data-stu-id="a90a7-314">After you have created a transfer request which includes an existing subscription, you should avoid updating the license quantity of the subscription (or associated addons).</span></span> <span data-ttu-id="a90a7-315">そうすると、新しい数量は転送要求に反映されません。</span><span class="sxs-lookup"><span data-stu-id="a90a7-315">If you do so, the new quantity will not be reflected in the transfer request.</span></span> <span data-ttu-id="a90a7-316">間接プロバイダーが譲渡要求を受け入れると、結果のサブスクリプションの数量は古いになります。</span><span class="sxs-lookup"><span data-stu-id="a90a7-316">After the indirect provider accepts the transfer request, the resultant subscription will have the old quantity.</span></span> <span data-ttu-id="a90a7-317">新しい数量を間接プロバイダーに転送する場合は、既存の転送要求を取り消して新しい数量を再作成する必要があります。</span><span class="sxs-lookup"><span data-stu-id="a90a7-317">If you wish for the new quantity to be transferred to the indirect provider, you must cancel the existing transfer request and recreate a new one.</span></span>

- <span data-ttu-id="a90a7-318">**セルフサービスサブスクリプション転送を使用して、すべての購入を転送できるわけではありません。**</span><span class="sxs-lookup"><span data-stu-id="a90a7-318">**Not all purchases can be transferred using self-served subscription transfer.**</span></span> <span data-ttu-id="a90a7-319">現時点では、この機能を使用して、O365 サブスクリプションと Azure PAYG サブスクリプション (0145P) のみを転送できます。</span><span class="sxs-lookup"><span data-stu-id="a90a7-319">Currently, you can only transfer O365 subscriptions and Azure PAYG subscriptions (MS-AZR-0145P) using this feature.</span></span> <span data-ttu-id="a90a7-320">Azure プラン、azure 予約インスタンス、用語ベースのサブスクリプション、Azure Marketplace の SaaS サブスクリプションなど、その他の購入はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a90a7-320">Other purchases including Azure Plans, Azure Reserved Instances, Term-based Subscriptions and SaaS subscriptions for Azure Marketplace are not supported.</span></span> <span data-ttu-id="a90a7-321">[転送要求の送信] ページでサブスクリプションを転送できない理由が表示されます。</span><span class="sxs-lookup"><span data-stu-id="a90a7-321">You will see a reason why a subscription cannot be transferred in the submit transfer request page.</span></span> <span data-ttu-id="a90a7-322">これらのサブスクリプションを譲渡するには、 [既存のサブスクリプションをキャンセル](create-a-new-subscription.md#suspend-or-cancel-a-subscription) し、間接プロバイダーを通じて顧客向けの新しいプランを購入する必要があります。</span><span class="sxs-lookup"><span data-stu-id="a90a7-322">To transfer these subscriptions, you will need to [cancel the existing subscription](create-a-new-subscription.md#suspend-or-cancel-a-subscription) and purchase new offer for customer through Indirect Provider.</span></span>

- <span data-ttu-id="a90a7-323">**サンドボックス環境を使用してテストすることはできません。**</span><span class="sxs-lookup"><span data-stu-id="a90a7-323">**Cannot be tested using sandbox environment.**</span></span>

## <a name="enroll-for-indirect-reseller-incentives"></a><span data-ttu-id="a90a7-324">間接リセラー インセンティブに登録する</span><span class="sxs-lookup"><span data-stu-id="a90a7-324">Enroll for indirect reseller incentives</span></span>

<span data-ttu-id="a90a7-325">既存の直接請求パートナー テナントで間接リセラーとして正常に登録した後、30 日以内に、間接リセラー インセンティブへの登録の招待を受け取ります。</span><span class="sxs-lookup"><span data-stu-id="a90a7-325">After you have successfully enrolled as an indirect reseller on your existing direct bill partner tenant, you will receive an invitation to enroll for indirect reseller incentive within 30 days.</span></span> <span data-ttu-id="a90a7-326">招待は、CSP パートナー テナントに現在関連付けられているパートナー MPN アカウントに基づいています。</span><span class="sxs-lookup"><span data-stu-id="a90a7-326">The invitation is based on the partner MPN account that is currently associated with your CSP partner tenant.</span></span> <span data-ttu-id="a90a7-327">招待は、パートナー MPN アカウントに関連付けられているメール アドレスに送られます。</span><span class="sxs-lookup"><span data-stu-id="a90a7-327">The invitation will be sent to the email address associated with the partner MPN account.</span></span>

<span data-ttu-id="a90a7-328">また、パートナーは、その同じパートナー テナントで直接請求インセンティブ プログラムに登録する資格もあります。</span><span class="sxs-lookup"><span data-stu-id="a90a7-328">You are also eligible to enroll for direct bill incentive programs with that same partner tenant.</span></span> <span data-ttu-id="a90a7-329">プログラムは個別に管理する必要があります。</span><span class="sxs-lookup"><span data-stu-id="a90a7-329">You must manage the programs separately.</span></span>

## <a name="next-steps"></a><span data-ttu-id="a90a7-330">次の手順</span><span class="sxs-lookup"><span data-stu-id="a90a7-330">Next steps</span></span>

- [<span data-ttu-id="a90a7-331">間接リセラーになることについての追加情報</span><span class="sxs-lookup"><span data-stu-id="a90a7-331">Additional information on becoming an indirect reseller</span></span>](https://assetsprod.microsoft.com/csp-directbill-to-indirect-transition.pdf)
- [<span data-ttu-id="a90a7-332">CSP の直接パートナーの新しい要件</span><span class="sxs-lookup"><span data-stu-id="a90a7-332">CSP direct partner new requirements</span></span>](direct-partner-new-requirements.md)
- [<span data-ttu-id="a90a7-333">制限付きの直接請求機能</span><span class="sxs-lookup"><span data-stu-id="a90a7-333">Restricted direct bill capabilities</span></span>](restricted-direct-bill-capabilities.md)
