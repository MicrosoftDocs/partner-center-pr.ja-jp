---
title: 顧客の関連付けを作成する
ms.topic: article
ms.date: 10/28/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-incentives
description: 顧客関連付けと 指名パートナーの指定 (CPOR) モデルを作成します。 Dynamics 365 のお客様の売上、使用状況、インセンティブMicrosoft 365 &管理するのに役立ちます。
author: MalloryPrincipe
ms.author: mallp
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 9526a47d0b6d734bde48f403c11fa84d734511c1
ms.sourcegitcommit: 7a6836bd962d5b426a8cb34a9132a87cbbbf39f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/13/2021
ms.locfileid: "109856102"
---
# <a name="customer-associations-via-the-claimed-partner-of-record-cpor-model-for-microsoft-365-and-dynamics-365"></a><span data-ttu-id="d20a7-104">Microsoft 365 および Dynamics 365 のレコード要求パートナー (CPOR) モデルを使用した顧客の関連付け</span><span class="sxs-lookup"><span data-stu-id="d20a7-104">Customer associations via the Claimed Partner of Record (CPOR) model for Microsoft 365 and Dynamics 365</span></span>


<span data-ttu-id="d20a7-105">**適切なロール**: インセンティブ管理者</span><span class="sxs-lookup"><span data-stu-id="d20a7-105">**Appropriate roles**: Incentives admin</span></span>

<span data-ttu-id="d20a7-106">2019 年 10 月 1 日に、Microsoft は 指名パートナーの指定 (CPOR) モデルを使用して、オンライン サービス アドバイザリ (OSA) 販売、オンライン サービス使用状況 (OSU)-Microsoft 365、および OSU-Business アプリケーション インセンティブに関する Microsoft 365 および Dynamics 365 のお客様との関連付けを管理し始めました。</span><span class="sxs-lookup"><span data-stu-id="d20a7-106">On October 1, 2019, Microsoft began using the Claiming Partner of Record (CPOR) model to manage the associations you have with your Microsoft 365 and Dynamics 365 customers with regard to the Online Services Advisory (OSA) Sell, Online Services Usage (OSU)-Microsoft 365, and OSU-Business Application incentives.</span></span>

>[!Important]
> <span data-ttu-id="d20a7-107">顧客の関連付け (CPOR) 要求は、Online Services Advisory (OSA) の販売、オンライン サービスの使用状況 (OSU)-Microsoft 365 および OSU-Business アプリケーション インセンティブ プログラムにのみ適用されます。</span><span class="sxs-lookup"><span data-stu-id="d20a7-107">Customer Association (CPOR) claims only apply to the Online Services Advisory (OSA) Sell, Online Services Usage (OSU)-Microsoft 365 and OSU-Business Application incentive programs.</span></span> <span data-ttu-id="d20a7-108">クラウド ソリューション プロバイダー、Managed Reseller、ホスティング、Surface などの別のプログラムの共同申請を送信する場合は、ここに記載されている共同申請プロセスを参照してください。</span><span class="sxs-lookup"><span data-stu-id="d20a7-108">If you are submitting a co-op claim for another program such as Cloud Solution Provider, Managed Reseller, Hosting, or Surface, please refer to Co-op claims process outlined here.</span></span> <br><br><span data-ttu-id="d20a7-109">要求を送信すると、Microsoft によって検証されます。</span><span class="sxs-lookup"><span data-stu-id="d20a7-109">When you submit your claim, Microsoft validates it.</span></span> <span data-ttu-id="d20a7-110">詳細については、この時点で詳しい情報をお願いする場合があります。</span><span class="sxs-lookup"><span data-stu-id="d20a7-110">We may ask you for more information at this point.</span></span> <span data-ttu-id="d20a7-111">また、関連付け要求を顧客に通知します。</span><span class="sxs-lookup"><span data-stu-id="d20a7-111">We'll also notify the customer of your association request.</span></span> <span data-ttu-id="d20a7-112">お客様はオプトアウトする 5 営業日を持っています。オプトアウトしない場合、この特定のテナントとワークロードとの関連付けは公式になります。</span><span class="sxs-lookup"><span data-stu-id="d20a7-112">Customers have five business days to opt out. If they don't opt out, your association with this specific tenant and workload will be official.</span></span> <span data-ttu-id="d20a7-113">この時点で、顧客の使用状況データにアクセスできます。</span><span class="sxs-lookup"><span data-stu-id="d20a7-113">At this point you'll have access to the customer's usage data.</span></span> 

<span data-ttu-id="d20a7-114">要求を完了するには、次の情報が必要です。</span><span class="sxs-lookup"><span data-stu-id="d20a7-114">You'll need the following information to complete a claim:</span></span>

- <span data-ttu-id="d20a7-115">要求 **を作成** するエンティティの MPN ID</span><span class="sxs-lookup"><span data-stu-id="d20a7-115">The **MPN ID** for your entity that makes the claim</span></span>

- <span data-ttu-id="d20a7-116">顧客のドメイン **名 これを**[見つける](find-ids-and-domain-names.md)</span><span class="sxs-lookup"><span data-stu-id="d20a7-116">Customer's **domain name** [Find this](find-ids-and-domain-names.md)</span></span>

- <span data-ttu-id="d20a7-117">顧客のディレクトリ **ID または** テナント **ID を見**[つける](find-ids-and-domain-names.md)</span><span class="sxs-lookup"><span data-stu-id="d20a7-117">Customer's **Directory ID** or **Tenant ID** [Find this](find-ids-and-domain-names.md)</span></span>

- <span data-ttu-id="d20a7-118">ソリューション **領域 (** 例: Business Applications または Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="d20a7-118">The **Solution area**, such as Business Applications or Microsoft 365</span></span>

- <span data-ttu-id="d20a7-119">実行 **した** アクティビティと、事前販売、使用状況、収益の関連付けなど、作成する要求の種類</span><span class="sxs-lookup"><span data-stu-id="d20a7-119">The **Activity** you have performed and the type of claim you want to make, such as Pre-sales, Usage, or Revenue association</span></span>

- <span data-ttu-id="d20a7-120">顧客の連絡先 **名、** タイトル、電子メール アドレス</span><span class="sxs-lookup"><span data-stu-id="d20a7-120">Your customer's **Contact name**, title, and email address</span></span>

- <span data-ttu-id="d20a7-121">Dynamics 365 の場合は、顧客の技術連絡先の名前、タイトル、電子メール アドレスも指定する必要があります</span><span class="sxs-lookup"><span data-stu-id="d20a7-121">For Dynamics 365, you also need to provide your customer's **Technical contact** name, title, and email address</span></span>

- <span data-ttu-id="d20a7-122">会社の連絡先名 **と電子** メール アドレス</span><span class="sxs-lookup"><span data-stu-id="d20a7-122">Your own company's **Contact name** and email address</span></span>

- <span data-ttu-id="d20a7-123">この要求の **名前を** 作成します</span><span class="sxs-lookup"><span data-stu-id="d20a7-123">You'll create a **Name** for this claim</span></span>

- <span data-ttu-id="d20a7-124">要求 **する** 製品またはワークロード</span><span class="sxs-lookup"><span data-stu-id="d20a7-124">The **Product(s)** or workload(s) you're claiming</span></span>

- <span data-ttu-id="d20a7-125">**実行証明 (PoE)**(顧客によって署名された作業のステートメントなど)。</span><span class="sxs-lookup"><span data-stu-id="d20a7-125">**Proof of execution (PoE)**, such as a statement of work signed by the customer.</span></span> <span data-ttu-id="d20a7-126">使用する PoE テンプレートをダウンロードすることもできます。</span><span class="sxs-lookup"><span data-stu-id="d20a7-126">You can also download a PoE template to use.</span></span>

- <span data-ttu-id="d20a7-127">収益の関連付けを要求するパートナーのみ: **Dynamics ソリューション** の販売者名、**顧客名\*\*\*\*、ISV** 製品/ソリューションの名前。</span><span class="sxs-lookup"><span data-stu-id="d20a7-127">For partners claiming revenue association only: **Dynamics solution seller name**, **Customer name**, and **Name of ISV product/solution**.</span></span> 

<span data-ttu-id="d20a7-128">また、次の点も理解する必要があります。</span><span class="sxs-lookup"><span data-stu-id="d20a7-128">You should also understand the following points:</span></span>

- <span data-ttu-id="d20a7-129">既存の顧客Microsoft 365場合は、このプロセスを使用して OSU インセンティブを獲得し続けるユーザーに再関連付けする必要があります。</span><span class="sxs-lookup"><span data-stu-id="d20a7-129">If you have existing Microsoft 365 customers, you'll need to re-associate with those you want to continue to earn OSU incentives by using this process.</span></span>

- <span data-ttu-id="d20a7-130">Dynamics 365 または Power BI のお客様と既存の関連付けがある場合、これらの関連付けはサブスクリプションの有効期限が切れるまで有効なままです。</span><span class="sxs-lookup"><span data-stu-id="d20a7-130">If you have existing associations with Dynamics 365 or Power BI customers, these associations will remain valid, until the expiration of their subscriptions.</span></span>

- <span data-ttu-id="d20a7-131">顧客は複数のパートナーを持つ場合がありますが、各ワークロード (OSU-Microsoft 365 の場合) またはサブスクリプション (OSA-Sell および OSU-Business アプリケーションの場合) は、1 つのパートナーにのみ関連付けできます。</span><span class="sxs-lookup"><span data-stu-id="d20a7-131">A customer can have multiple partners, but each workload (for OSU-Microsoft 365) or subscription (for OSA-Sell and OSU-Business Applications) can only be associated with one partner.</span></span>

## <a name="create-a-customer-association"></a><span data-ttu-id="d20a7-132">顧客の関連付けを作成する</span><span class="sxs-lookup"><span data-stu-id="d20a7-132">Create a customer association</span></span>

1. <span data-ttu-id="d20a7-133">[パートナー センターのダッシュボード](https://partner.microsoft.com/dashboard/)にサインインします。</span><span class="sxs-lookup"><span data-stu-id="d20a7-133">Sign into the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span></span>

2. <span data-ttu-id="d20a7-134">[インセンティブ] **タブを選択** し、[概要] **を選択** してから、[顧客の関連付 **け] を選択します**。</span><span class="sxs-lookup"><span data-stu-id="d20a7-134">Select the **Incentives** tab, select **Overview**, and then select **Customer associations**.</span></span>

3. <span data-ttu-id="d20a7-135">[顧客の関連付け] ページの上部にある [+ 顧客の関連 **付け] を選択します**。</span><span class="sxs-lookup"><span data-stu-id="d20a7-135">At the top of the Customer associations page, select **+ Customer association**.</span></span>

4. <span data-ttu-id="d20a7-136">顧客に関連付けるパートナーの場所の **[MPN ID]** を選択し、顧客のドメイン名とディレクトリ ID を追加します。</span><span class="sxs-lookup"><span data-stu-id="d20a7-136">Select the **MPN ID** of the partner location to be associated with the customer, and then add the customer's domain name and Directory ID.</span></span> [<span data-ttu-id="d20a7-137">これを見つける</span><span class="sxs-lookup"><span data-stu-id="d20a7-137">Find this</span></span>](find-ids-and-domain-names.md)

5. <span data-ttu-id="d20a7-138">**[続行]** をクリックします。</span><span class="sxs-lookup"><span data-stu-id="d20a7-138">Select **Continue**.</span></span>

6. <span data-ttu-id="d20a7-139">[ソリューション] 領域 **と [アクティビティ** ] を **選択します**。</span><span class="sxs-lookup"><span data-stu-id="d20a7-139">Select the **Solution area** and **Activity**.</span></span> 

   >[!Note]
   >
   ><span data-ttu-id="d20a7-140">[売上] をBusiness Applications[使用量]または [売上前] 、または[収益の関連付け] を選択し、[続行] を **選択します**。</span><span class="sxs-lookup"><span data-stu-id="d20a7-140">If you select Business Applications, select either **Usage and/or Pre-sales**, or **Revenue association**, and then select **Continue**.</span></span> 
   <br><br><span data-ttu-id="d20a7-141">[Revenue association]\(収益の関連付け\) を選択した場合、以下に示す内容とは少し異なる情報の入力を求められます。</span><span class="sxs-lookup"><span data-stu-id="d20a7-141">If you select Revenue association, you'll be prompted for slightly different information than what's listed below.</span></span>

7. <span data-ttu-id="d20a7-142">[顧客の関連付け] ページで **適切な情報を入力** し、[要求の作成] **を選択します**。</span><span class="sxs-lookup"><span data-stu-id="d20a7-142">Enter the appropriate information on the **Associate customer** page, and then select **Create claim**.</span></span>

8. <span data-ttu-id="d20a7-143">この顧客の関連付けに関連付けられている製品を選択し、[続行] を **選択します**。</span><span class="sxs-lookup"><span data-stu-id="d20a7-143">Select the product(s) associated with this customer association, and then select **Continue**.</span></span>

9. <span data-ttu-id="d20a7-144">お客様の連絡先情報と会社の連絡先情報を入力します。</span><span class="sxs-lookup"><span data-stu-id="d20a7-144">Complete the customer contact information and your company's contact information.</span></span> <span data-ttu-id="d20a7-145">すべてのフィールドが必須です。</span><span class="sxs-lookup"><span data-stu-id="d20a7-145">All fields are required.</span></span> 

   >[!NOTE]
   ><span data-ttu-id="d20a7-146">製品が Dynamics 365 で、選択した製品にこの特定の顧客に対して複数のサブスクリプションがある場合は、サブスクリプション ID も入力する必要があります。</span><span class="sxs-lookup"><span data-stu-id="d20a7-146">If your product is Dynamics 365, and the product you choose has multiple subscriptions for this particular customer, you'll also need to enter the subscription ID.</span></span>

10. <span data-ttu-id="d20a7-147">実行証明 (PoE) を指定します。</span><span class="sxs-lookup"><span data-stu-id="d20a7-147">Supply your proof of execution (PoE).</span></span> <span data-ttu-id="d20a7-148">このボックスにドラッグするか、補足ドキュメントを参照するか、 **[テンプレートのダウンロード]** を選択してテンプレートを使用することができます。</span><span class="sxs-lookup"><span data-stu-id="d20a7-148">You can drag it to the box, browse to your own supporting documentation, or use a template by selecting **Download template**.</span></span> 

11. <span data-ttu-id="d20a7-149">必要に応じてコメントを追加して保存し、 **[Submit claim]\(請求の送信\)** を選択します。</span><span class="sxs-lookup"><span data-stu-id="d20a7-149">Add and save comments if you like, and then select **Submit claim**.</span></span> <span data-ttu-id="d20a7-150">顧客の関連付けの承認を依頼するメールをお客様に送信します。</span><span class="sxs-lookup"><span data-stu-id="d20a7-150">We'll send an email to the customer requesting approval of your customer association.</span></span>

   >[!NOTE]
   ><span data-ttu-id="d20a7-151">顧客の関連付けを送信した後は、編集を行う必要があります。</span><span class="sxs-lookup"><span data-stu-id="d20a7-151">Once you submit your customer association, you can't edit it.</span></span>

<span data-ttu-id="d20a7-152">顧客の関連付けの状態は、 **[状態]** フィールドに表示されます。</span><span class="sxs-lookup"><span data-stu-id="d20a7-152">The status of your customer association appears in the **Status** field.</span></span>

<span data-ttu-id="d20a7-153">**[履歴]** を選択すると、顧客の関連付けの履歴が表示されます。</span><span class="sxs-lookup"><span data-stu-id="d20a7-153">Select **History** to view the history of a customer association.</span></span>

## <a name="next-steps"></a><span data-ttu-id="d20a7-154">次の手順</span><span class="sxs-lookup"><span data-stu-id="d20a7-154">Next steps</span></span>

- [<span data-ttu-id="d20a7-155">顧客の関連付けを管理する</span><span class="sxs-lookup"><span data-stu-id="d20a7-155">Manage customer associations</span></span>](incentives-manage-customer-associations.md)