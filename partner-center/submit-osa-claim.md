---
title: 顧客の関連付けを作成する
ms.topic: article
ms.date: 10/28/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-incentives
description: 取引先レコード (CPOR) モデルを使用して顧客の関連付けを作成します。 Microsoft 365 & Dynamics 365 の顧客の売上、使用状況、インセンティブを管理するのに役立ちます。
author: MalloryPrincipe
ms.author: mallp
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 196009d9271324377be02d0b2d12ba8a4d7a993c
ms.sourcegitcommit: 09eabb559aae25518caf3f2a59ef16a3e123c207
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/23/2021
ms.locfileid: "112489953"
---
# <a name="customer-associations-via-the-claimed-partner-of-record-cpor-model-for-microsoft-365-and-dynamics-365"></a><span data-ttu-id="261d8-104">Microsoft 365 と Dynamics 365 の要求されたパートナーのレコード (CPOR) モデルによる顧客の関連付け</span><span class="sxs-lookup"><span data-stu-id="261d8-104">Customer associations via the Claimed Partner of Record (CPOR) model for Microsoft 365 and Dynamics 365</span></span>


<span data-ttu-id="261d8-105">**適切なロール**: インセンティブ管理者</span><span class="sxs-lookup"><span data-stu-id="261d8-105">**Appropriate roles**: Incentives admin</span></span>

<span data-ttu-id="261d8-106">2019年10月1日に、Microsoft は、パートナーの取引先レコード (CPOR) モデルを使用して、オンラインサービスアドバイザリ (OSA) 販売、Online Services Usage (OSU)-Microsoft 365、および OSU-Business アプリケーションインセンティブに関して、Microsoft 365 と Dynamics 365 のお客様との関連付けを管理しました。</span><span class="sxs-lookup"><span data-stu-id="261d8-106">On October 1, 2019, Microsoft began using the Claiming Partner of Record (CPOR) model to manage the associations you have with your Microsoft 365 and Dynamics 365 customers with regard to the Online Services Advisory (OSA) Sell, Online Services Usage (OSU)-Microsoft 365, and OSU-Business Application incentives.</span></span>

>[!Important]
> <span data-ttu-id="261d8-107">カスタマーアソシエーション (CPOR) の要求は、オンラインサービスアドバイザリ (OSA) 販売、Online Services Usage (OSU) Microsoft 365 および OSU-Business アプリケーションインセンティブプログラムにのみ適用されます。</span><span class="sxs-lookup"><span data-stu-id="261d8-107">Customer Association (CPOR) claims only apply to the Online Services Advisory (OSA) Sell, Online Services Usage (OSU)-Microsoft 365 and OSU-Business Application incentive programs.</span></span> <span data-ttu-id="261d8-108">クラウドソリューションプロバイダー (CSP)、管理されたリセラー、ホスティング、Surface などの別のプログラムに対して共同操作要求を送信する場合は、こちらに記載されている Co-op 要求プロセスを参照してください。</span><span class="sxs-lookup"><span data-stu-id="261d8-108">If you are submitting a co-op claim for another program such as Cloud Solution Provider (CSP), Managed Reseller, Hosting, or Surface, please refer to Co-op claims process outlined here.</span></span> <br><br><span data-ttu-id="261d8-109">要求を送信すると、Microsoft によって検証されます。</span><span class="sxs-lookup"><span data-stu-id="261d8-109">When you submit your claim, Microsoft validates it.</span></span> <span data-ttu-id="261d8-110">詳細については、こちらからお問い合わせください。</span><span class="sxs-lookup"><span data-stu-id="261d8-110">We may ask you for more information at this point.</span></span> <span data-ttu-id="261d8-111">また、お客様にアソシエーション要求を通知します。</span><span class="sxs-lookup"><span data-stu-id="261d8-111">We'll also notify the customer of your association request.</span></span> <span data-ttu-id="261d8-112">お客様は、5営業日以内にオプトアウトできます。オプトアウトされていない場合は、この特定のテナントとワークロードとの関連付けが公式になります。</span><span class="sxs-lookup"><span data-stu-id="261d8-112">Customers have five business days to opt out. If they don't opt out, your association with this specific tenant and workload will be official.</span></span> <span data-ttu-id="261d8-113">この時点で、顧客の使用状況データにアクセスできます。</span><span class="sxs-lookup"><span data-stu-id="261d8-113">At this point you'll have access to the customer's usage data.</span></span> 

<span data-ttu-id="261d8-114">要求を完了するには、次の情報が必要です。</span><span class="sxs-lookup"><span data-stu-id="261d8-114">You'll need the following information to complete a claim:</span></span>

- <span data-ttu-id="261d8-115">要求を行うエンティティの **MPN id** (Microsoft Partner Network id)</span><span class="sxs-lookup"><span data-stu-id="261d8-115">The **MPN ID** (Microsoft Partner Network ID) for your entity that makes the claim</span></span>

- <span data-ttu-id="261d8-116">顧客の **ドメイン名** (詳細については、「 [テナント ID、ドメイン名、ユーザーオブジェクト ID の検索](find-ids-and-domain-names.md)」を参照してください)</span><span class="sxs-lookup"><span data-stu-id="261d8-116">Customer's **domain name** (for more information, see [Find tenant ID, domain name, user object ID](find-ids-and-domain-names.md))</span></span>

- <span data-ttu-id="261d8-117">顧客の **ディレクトリ id** または **テナント id** (詳細については、「 [テナント id、ドメイン名、ユーザーオブジェクト ID の検索](find-ids-and-domain-names.md)」を参照してください)</span><span class="sxs-lookup"><span data-stu-id="261d8-117">Customer's **Directory ID** or **Tenant ID** (for more information, see [Find tenant ID, domain name, user object ID](find-ids-and-domain-names.md))</span></span>

- <span data-ttu-id="261d8-118">Business Applications や Microsoft 365 などの **ソリューション領域**</span><span class="sxs-lookup"><span data-stu-id="261d8-118">The **Solution area**, such as Business Applications or Microsoft 365</span></span>

- <span data-ttu-id="261d8-119">実行した **アクティビティ** と、販売前、使用状況、収益の関連付けなど、作成する要求の種類</span><span class="sxs-lookup"><span data-stu-id="261d8-119">The **Activity** you have performed and the type of claim you want to make, such as Pre-sales, Usage, or Revenue association</span></span>

- <span data-ttu-id="261d8-120">お客様の **連絡先の名前**、役職、および電子メールアドレス</span><span class="sxs-lookup"><span data-stu-id="261d8-120">Your customer's **Contact name**, title, and email address</span></span>

- <span data-ttu-id="261d8-121">Dynamics 365 では、顧客の **技術担当者** 名、役職、および電子メールアドレスも入力する必要があります。</span><span class="sxs-lookup"><span data-stu-id="261d8-121">For Dynamics 365, you also need to provide your customer's **Technical contact** name, title, and email address</span></span>

- <span data-ttu-id="261d8-122">自分の会社の **連絡先名** と電子メールアドレス</span><span class="sxs-lookup"><span data-stu-id="261d8-122">Your own company's **Contact name** and email address</span></span>

- <span data-ttu-id="261d8-123">この要求の **名前** を作成します</span><span class="sxs-lookup"><span data-stu-id="261d8-123">You'll create a **Name** for this claim</span></span>

- <span data-ttu-id="261d8-124">要求している **製品** またはワークロード</span><span class="sxs-lookup"><span data-stu-id="261d8-124">The **Product(s)** or workload(s) you're claiming</span></span>

- <span data-ttu-id="261d8-125">顧客によって署名された作業ステートメントなど、**実行の証拠 (PoE)**。</span><span class="sxs-lookup"><span data-stu-id="261d8-125">**Proof of execution (PoE)**, such as a statement of work signed by the customer.</span></span> <span data-ttu-id="261d8-126">また、使用する PoE テンプレートをダウンロードすることもできます。</span><span class="sxs-lookup"><span data-stu-id="261d8-126">You can also download a PoE template to use.</span></span>

- <span data-ttu-id="261d8-127">収益の関連付けのみを要求しているパートナーの場合: **Dynamics ソリューション販売者名**、 **顧客名**、および **ISV 製品/ソリューションの名前**。</span><span class="sxs-lookup"><span data-stu-id="261d8-127">For partners claiming revenue association only: **Dynamics solution seller name**, **Customer name**, and **Name of ISV product/solution**.</span></span> 

<span data-ttu-id="261d8-128">また、次の点についても理解しておく必要があります。</span><span class="sxs-lookup"><span data-stu-id="261d8-128">You should also understand the following points:</span></span>

- <span data-ttu-id="261d8-129">既存の Microsoft 365 のお客様の場合は、このプロセスを使用して、引き続き OSU インセンティブを獲得する必要があります。</span><span class="sxs-lookup"><span data-stu-id="261d8-129">If you have existing Microsoft 365 customers, you'll need to reassociate with those you want to continue to earn OSU incentives by using this process.</span></span>

- <span data-ttu-id="261d8-130">Dynamics 365 または Power BI の顧客との既存の関連付けがある場合、これらの関連付けは、サブスクリプションの有効期限が切れるまで有効のままになります。</span><span class="sxs-lookup"><span data-stu-id="261d8-130">If you have existing associations with Dynamics 365 or Power BI customers, these associations will remain valid, until the expiration of their subscriptions.</span></span>

- <span data-ttu-id="261d8-131">顧客は複数のパートナーを持つことができますが、各ワークロード (OSU-Microsoft 365 の場合) またはサブスクリプション (OSA-Sell アプリケーションと OSU-Business アプリケーションの場合) は、1つのパートナーにのみ関連付けることができます。</span><span class="sxs-lookup"><span data-stu-id="261d8-131">A customer can have multiple partners, but each workload (for OSU-Microsoft 365) or subscription (for OSA-Sell and OSU-Business Applications) can only be associated with one partner.</span></span>

## <a name="create-a-customer-association"></a><span data-ttu-id="261d8-132">顧客の関連付けを作成する</span><span class="sxs-lookup"><span data-stu-id="261d8-132">Create a customer association</span></span>

1. <span data-ttu-id="261d8-133">[パートナー センター ダッシュボード](https://partner.microsoft.com/dashboard/)にサインインします。</span><span class="sxs-lookup"><span data-stu-id="261d8-133">Sign in to the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span></span>

2. <span data-ttu-id="261d8-134">[ **インセンティブ** ] タブを選択し、[ **概要**] を選択して、[ **顧客の関連付け**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="261d8-134">Select the **Incentives** tab, select **Overview**, and then select **Customer associations**.</span></span>

3. <span data-ttu-id="261d8-135">[顧客の関連付け] ページの上部で、[ **+ 顧客の関連付け**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="261d8-135">At the top of the Customer associations page, select **+ Customer association**.</span></span>

4. <span data-ttu-id="261d8-136">顧客に関連付けるパートナーの場所の **[MPN ID]** を選択し、顧客のドメイン名とディレクトリ ID を追加します。</span><span class="sxs-lookup"><span data-stu-id="261d8-136">Select the **MPN ID** of the partner location to be associated with the customer, and then add the customer's domain name and Directory ID.</span></span> [<span data-ttu-id="261d8-137">検索する文字列</span><span class="sxs-lookup"><span data-stu-id="261d8-137">Find this</span></span>](find-ids-and-domain-names.md)

5. <span data-ttu-id="261d8-138">**[続行]** をクリックします。</span><span class="sxs-lookup"><span data-stu-id="261d8-138">Select **Continue**.</span></span>

6. <span data-ttu-id="261d8-139">ソリューションの **区分** と **アクティビティ** を選択します。</span><span class="sxs-lookup"><span data-stu-id="261d8-139">Select the **Solution area** and **Activity**.</span></span> 

   >[!Note]
   >
   ><span data-ttu-id="261d8-140">[Business Applications] を選択した場合は、[ **使用状況] または [事前売上**] または [ **収益の関連付け**] を選択し、[ **続行**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="261d8-140">If you select Business Applications, select either **Usage and/or Pre-sales**, or **Revenue association**, and then select **Continue**.</span></span> 
   <br><br><span data-ttu-id="261d8-141">[Revenue association]\(収益の関連付け\) を選択した場合、以下に示す内容とは少し異なる情報の入力を求められます。</span><span class="sxs-lookup"><span data-stu-id="261d8-141">If you select Revenue association, you'll be prompted for slightly different information than what's listed below.</span></span>

7. <span data-ttu-id="261d8-142">[ **顧客の関連付け** ] ページで適切な情報を入力し、[ **要求の作成**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="261d8-142">Enter the appropriate information on the **Associate customer** page, and then select **Create claim**.</span></span>

8. <span data-ttu-id="261d8-143">この顧客の関連付けに関連付けられている製品を選択し、[ **続行**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="261d8-143">Select the product(s) associated with this customer association, and then select **Continue**.</span></span>

9. <span data-ttu-id="261d8-144">お客様の連絡先情報と会社の連絡先情報を入力します。</span><span class="sxs-lookup"><span data-stu-id="261d8-144">Complete the customer contact information and your company's contact information.</span></span> <span data-ttu-id="261d8-145">すべてのフィールドが必須です。</span><span class="sxs-lookup"><span data-stu-id="261d8-145">All fields are required.</span></span> 

   >[!NOTE]
   ><span data-ttu-id="261d8-146">製品が Dynamics 365 で、選択した製品がこの特定の顧客に対して複数のサブスクリプションを持っている場合は、サブスクリプション ID も入力する必要があります。</span><span class="sxs-lookup"><span data-stu-id="261d8-146">If your product is Dynamics 365, and the product you choose has multiple subscriptions for this particular customer, you'll also need to enter the subscription ID.</span></span>

10. <span data-ttu-id="261d8-147">PoE を提供します。</span><span class="sxs-lookup"><span data-stu-id="261d8-147">Supply your PoE.</span></span> <span data-ttu-id="261d8-148">このボックスにドラッグするか、補足ドキュメントを参照するか、 **[テンプレートのダウンロード]** を選択してテンプレートを使用することができます。</span><span class="sxs-lookup"><span data-stu-id="261d8-148">You can drag it to the box, browse to your own supporting documentation, or use a template by selecting **Download template**.</span></span> 

11. <span data-ttu-id="261d8-149">必要に応じてコメントを追加して保存し、 **[Submit claim]\(請求の送信\)** を選択します。</span><span class="sxs-lookup"><span data-stu-id="261d8-149">Add and save comments if you like, and then select **Submit claim**.</span></span> <span data-ttu-id="261d8-150">顧客の関連付けの承認を依頼するメールをお客様に送信します。</span><span class="sxs-lookup"><span data-stu-id="261d8-150">We'll send an email to the customer requesting approval of your customer association.</span></span>

   >[!NOTE]
   ><span data-ttu-id="261d8-151">顧客の関連付けを送信した後は、それを編集することはできません。</span><span class="sxs-lookup"><span data-stu-id="261d8-151">Once you submit your customer association, you can't edit it.</span></span>

<span data-ttu-id="261d8-152">顧客の関連付けの状態は、 **[状態]** フィールドに表示されます。</span><span class="sxs-lookup"><span data-stu-id="261d8-152">The status of your customer association appears in the **Status** field.</span></span>

<span data-ttu-id="261d8-153">**[履歴]** を選択すると、顧客の関連付けの履歴が表示されます。</span><span class="sxs-lookup"><span data-stu-id="261d8-153">Select **History** to view the history of a customer association.</span></span>

## <a name="next-steps"></a><span data-ttu-id="261d8-154">次の手順</span><span class="sxs-lookup"><span data-stu-id="261d8-154">Next steps</span></span>

- [<span data-ttu-id="261d8-155">顧客の関連付けを管理する</span><span class="sxs-lookup"><span data-stu-id="261d8-155">Manage customer associations</span></span>](incentives-manage-customer-associations.md)