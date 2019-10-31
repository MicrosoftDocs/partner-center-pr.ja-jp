---
title: CPOR モデルを使用して顧客の関連付けを作成する |パートナーセンター
ms.topic: article
ms.date: 10/29/2019
description: CPOR モデルを使用して顧客の関連付けを作成する
author: LauraBrenner
ms.author: labrenne
keywords: インセンティブ要求、共同操作要求、共同操作ファンド、OSU、OSA、ISV、収益関連
ms.localizationpriority: medium
ms.openlocfilehash: 9acac203d44e3942f9a07bc5af90528e558bce39
ms.sourcegitcommit: 014669c26592a3ab35c2aa7f3ff615f5f1091752
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 10/30/2019
ms.locfileid: "73083867"
---
<span data-ttu-id="8892d-104">**適用対象**</span><span class="sxs-lookup"><span data-stu-id="8892d-104">**Applies to**</span></span>

-  <span data-ttu-id="8892d-105">パートナー センター</span><span class="sxs-lookup"><span data-stu-id="8892d-105">Partner Center</span></span>

# <a name="create-a-customer-association-using-the-cpor-model"></a><span data-ttu-id="8892d-106">CPOR モデルを使用して顧客の関連付けを作成する</span><span class="sxs-lookup"><span data-stu-id="8892d-106">Create a customer association using the CPOR model</span></span>

<span data-ttu-id="8892d-107">2019年10月1日に、Microsoft は、パートナーの取引先レコード (CPOR) モデルを使用して、オンラインサービスアドバイザリ (OSA) の販売、オンラインサービス使用状況 (OSU) に関して、Microsoft 365 と Dynamics 365 のお客様との関連付けを管理しました。Microsoft 365 と OSU-ビジネスアプリケーションインセンティブ。</span><span class="sxs-lookup"><span data-stu-id="8892d-107">On October 1, 2019, Microsoft began using the Claiming Partner of Record (CPOR) model to manage the associations you have with your Microsoft 365 and Dynamics 365 customers with regards to the Online Services Advisory (OSA) Sell, Online Services Usage (OSU)-Microsoft 365 and OSU-Business Application incentives.</span></span>

<span data-ttu-id="8892d-108">要求を送信すると、Microsoft によって検証されます。</span><span class="sxs-lookup"><span data-stu-id="8892d-108">When you submit your claim, Microsoft validates it.</span></span> <span data-ttu-id="8892d-109">詳細については、こちらからお問い合わせください。</span><span class="sxs-lookup"><span data-stu-id="8892d-109">We may ask you for more information at this point.</span></span> <span data-ttu-id="8892d-110">また、お客様にアソシエーション要求を通知します。</span><span class="sxs-lookup"><span data-stu-id="8892d-110">We’ll also notify the customer of your association request.</span></span> <span data-ttu-id="8892d-111">お客様は、5営業日以内にオプトアウトできます。オプトアウトされていない場合は、この特定のテナントとワークロードとの関連付けが公式になります。</span><span class="sxs-lookup"><span data-stu-id="8892d-111">Customers have five business days to opt out. If they don’t opt out, your association with this specific tenant and workload will be official.</span></span> <span data-ttu-id="8892d-112">この時点で、顧客の使用状況データにアクセスできます。</span><span class="sxs-lookup"><span data-stu-id="8892d-112">At this point you’ll have access to the customer’s usage data.</span></span> 

<span data-ttu-id="8892d-113">要求を完了するには、次の情報が必要です。</span><span class="sxs-lookup"><span data-stu-id="8892d-113">You’ll need the following information to complete a claim:</span></span>

- <span data-ttu-id="8892d-114">要求を行うエンティティの**MPN ID**</span><span class="sxs-lookup"><span data-stu-id="8892d-114">The **MPN ID** for your entity that makes the claim</span></span>

- <span data-ttu-id="8892d-115">顧客の**ドメイン名**[検索](https://docs.microsoft.com/partner-center/find-customer-domain-name)</span><span class="sxs-lookup"><span data-stu-id="8892d-115">Customer’s **domain name** [Find this](https://docs.microsoft.com/partner-center/find-customer-domain-name)</span></span>

- <span data-ttu-id="8892d-116">顧客の**ディレクトリ id**または**テナント id**を[検索](https://docs.microsoft.com/partner-center/find-customer-domain-name)します</span><span class="sxs-lookup"><span data-stu-id="8892d-116">Customer’s **Directory ID** or **Tenant ID** [Find this](https://docs.microsoft.com/partner-center/find-customer-domain-name)</span></span>

- <span data-ttu-id="8892d-117">Business Applications や Microsoft 365 などの**ソリューション領域**</span><span class="sxs-lookup"><span data-stu-id="8892d-117">The **Solution area**, such as Business Applications or Microsoft 365</span></span>

- <span data-ttu-id="8892d-118">実行した**アクティビティ**と、販売前、使用状況、収益の関連付けなど、作成する要求の種類</span><span class="sxs-lookup"><span data-stu-id="8892d-118">The **Activity** you have performed and the type of claim you want to make, such as Pre-sales, Usage, or Revenue association</span></span>

- <span data-ttu-id="8892d-119">お客様の**連絡先の名前**、役職、および電子メールアドレス</span><span class="sxs-lookup"><span data-stu-id="8892d-119">Your customer’s **Contact name**, title, and email address</span></span>

- <span data-ttu-id="8892d-120">Dynamics 365 では、顧客の**技術担当者**名、役職、および電子メールアドレスも入力する必要があります。</span><span class="sxs-lookup"><span data-stu-id="8892d-120">For Dynamics 365, you also need to provide your customer’s **Technical contact** name, title, and email address</span></span>

- <span data-ttu-id="8892d-121">自分の会社の**連絡先名**と電子メールアドレス</span><span class="sxs-lookup"><span data-stu-id="8892d-121">Your own company’s **Contact name** and email address</span></span>

- <span data-ttu-id="8892d-122">この要求の**名前**を作成します</span><span class="sxs-lookup"><span data-stu-id="8892d-122">You’ll create a **Name** for this claim</span></span>

- <span data-ttu-id="8892d-123">要求している**製品**またはワークロード</span><span class="sxs-lookup"><span data-stu-id="8892d-123">The **Product(s)** or workload(s) you’re claiming</span></span>

- <span data-ttu-id="8892d-124">顧客によって署名された作業ステートメントなど、**実行の証拠 (POE)** 。</span><span class="sxs-lookup"><span data-stu-id="8892d-124">**Proof of execution (POE)**, such as a statement of work signed by the customer.</span></span> <span data-ttu-id="8892d-125">また、使用する POE テンプレートをダウンロードすることもできます。</span><span class="sxs-lookup"><span data-stu-id="8892d-125">You can also download a POE template to use.</span></span>

- <span data-ttu-id="8892d-126">収益の関連付けのみを要求しているパートナーの場合: **Dynamics ソリューション販売者名**、**顧客名**、および**ISV 製品/ソリューションの名前**。</span><span class="sxs-lookup"><span data-stu-id="8892d-126">For partners claiming revenue association only: **Dynamics solution seller name**, **Customer name**, and **Name of ISV product/solution**.</span></span> 

<span data-ttu-id="8892d-127">また、次の点についても理解しておく必要があります。</span><span class="sxs-lookup"><span data-stu-id="8892d-127">You should also understand the following points:</span></span>
- <span data-ttu-id="8892d-128">既存の Microsoft 365 のお客様の場合は、このプロセスを使用して引き続き OSU インセンティブを獲得する必要があります。</span><span class="sxs-lookup"><span data-stu-id="8892d-128">If you have existing Microsoft 365 customers, you’ll need to re-associate with those you want to continue to earn OSU incentives by using this process.</span></span>
- <span data-ttu-id="8892d-129">Dynamics 365 または Power BI の顧客との既存の関連付けがある場合、これらの関連付けは、サブスクリプションの有効期限が切れるまで有効のままになります。</span><span class="sxs-lookup"><span data-stu-id="8892d-129">If you have existing associations with Dynamics 365 or Power BI customers, these associations will remain valid, until the expiration of their subscriptions.</span></span>
- <span data-ttu-id="8892d-130">顧客は複数のパートナーを持つことができますが、各ワークロード (OSU-Microsoft 365) またはサブスクリプション (OSA 販売と OSU-Business Applications) は、1つのパートナーにのみ関連付けることができます。</span><span class="sxs-lookup"><span data-stu-id="8892d-130">A customer can have multiple partners, but each workload (for OSU-Microsoft 365) or subscription (for OSA-Sell and OSU-Business Applications) can only be associated with one partner.</span></span>

## <a name="create-a-customer-association"></a><span data-ttu-id="8892d-131">顧客の関連付けを作成する</span><span class="sxs-lookup"><span data-stu-id="8892d-131">Create a customer association</span></span>
1.  <span data-ttu-id="8892d-132">パートナーセンターのダッシュボードで、 **[インセンティブ]** の下にある **[概要]** を選択し、 **[顧客の関連付け]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="8892d-132">In the Partner Center dashboard, under **Incentives**, select **Overview**, and then select **Customer associations**.</span></span> 

2.  <span data-ttu-id="8892d-133">顧客の関連付け ページの上部で、 **+ 顧客の関連付け** を選択します。</span><span class="sxs-lookup"><span data-stu-id="8892d-133">At the top of the Customer associations page, select **+ Customer association**.</span></span>

3.  <span data-ttu-id="8892d-134">顧客に関連付けるパートナーの場所の**MPN ID**を選択し、顧客のドメイン名とディレクトリ ID を追加します。</span><span class="sxs-lookup"><span data-stu-id="8892d-134">Select the **MPN ID** of the partner location to be associated with the customer, and then add the customer’s domain name and Directory ID.</span></span> [<span data-ttu-id="8892d-135">これらはどこにありますか。</span><span class="sxs-lookup"><span data-stu-id="8892d-135">Where are these?</span></span>](https://docs.microsoft.com/partner-center/find-customer-domain-name)

<span data-ttu-id="8892d-136">**[続行]** を選びます。</span><span class="sxs-lookup"><span data-stu-id="8892d-136">Select **Continue**.</span></span>

4.  <span data-ttu-id="8892d-137">ソリューションの**区分**と**アクティビティ**を選択します。</span><span class="sxs-lookup"><span data-stu-id="8892d-137">Select the **Solution area** and **Activity**.</span></span> 

>[!Note]

><span data-ttu-id="8892d-138">[Business Applications] を選択した場合は、[**使用状況] または [事前売上**] または **[収益の関連付け]** を選択し、 **[続行]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="8892d-138">If you select Business Applications, select either **Usage and/or Pre-sales**, or **Revenue association**, and then select **Continue**.</span></span> 

><span data-ttu-id="8892d-139">[収益の関連付け] を選択した場合は、以下の情報とは少し異なる情報を入力するように求められます。</span><span class="sxs-lookup"><span data-stu-id="8892d-139">If you select Revenue association, you’ll be prompted for slightly different information than what’s listed below.</span></span> 

5.  <span data-ttu-id="8892d-140">**[顧客の関連付け]** ページで適切な情報を入力し、 **[要求の作成]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="8892d-140">Enter the appropriate information on the **Associate customer** page, and then select **Create claim**.</span></span>

6.  <span data-ttu-id="8892d-141">この顧客の関連付けに関連付けられている製品を選択し、 **[続行]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="8892d-141">Select the product(s) associated with this customer association, and then select **Continue**.</span></span>

7.  <span data-ttu-id="8892d-142">お客様の連絡先情報と会社の連絡先情報を入力します。</span><span class="sxs-lookup"><span data-stu-id="8892d-142">Complete the customer contact information and your company’s contact information.</span></span> <span data-ttu-id="8892d-143">すべてのフィールドは必須です。</span><span class="sxs-lookup"><span data-stu-id="8892d-143">All fields are required.</span></span> 

>[!Note]

<span data-ttu-id="8892d-144">製品が Dynamics 365 で、選択した製品がこの特定の顧客に対して複数のサブスクリプションを持っている場合は、サブスクリプション ID も入力する必要があります。</span><span class="sxs-lookup"><span data-stu-id="8892d-144">If your product is Dynamics 365, and the product you choose has multiple subscriptions for this particular customer, you’ll also need to enter the subscription ID.</span></span>

8.  <span data-ttu-id="8892d-145">実行の証拠 (POE) を提供します。</span><span class="sxs-lookup"><span data-stu-id="8892d-145">Supply your proof of execution (POE).</span></span> <span data-ttu-id="8892d-146">このボタンをボックスにドラッグするか、独自のサポートドキュメントを参照するか、[テンプレートの**ダウンロード**] を選択してテンプレートを使用することができます。</span><span class="sxs-lookup"><span data-stu-id="8892d-146">You can drag it to the box, browse to your own supporting documentation, or use a template by selecting **Download template**.</span></span> 

9.  <span data-ttu-id="8892d-147">必要に応じてコメントを追加して保存し、 **[要求の送信]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="8892d-147">Add and save comments if you like, and then select **Submit claim**.</span></span> <span data-ttu-id="8892d-148">顧客の関連付けの承認を要求する電子メールをお客様に送信します。</span><span class="sxs-lookup"><span data-stu-id="8892d-148">We’ll send an email to the customer requesting approval of your customer association.</span></span> 

>[!NOTE]

><span data-ttu-id="8892d-149">顧客の関連付けを送信した後は、それを編集することはできません。</span><span class="sxs-lookup"><span data-stu-id="8892d-149">Once you submit your customer association, you can’t edit it.</span></span> 

<span data-ttu-id="8892d-150">顧客の関連付けの状態が **[状態]** フィールドに表示されます。</span><span class="sxs-lookup"><span data-stu-id="8892d-150">The status of your customer association appears in the **Status** field.</span></span> 

<span data-ttu-id="8892d-151">**[履歴]** を選択して、顧客の関連付けの履歴を表示します。</span><span class="sxs-lookup"><span data-stu-id="8892d-151">Select **History** to view the history of a customer association.</span></span>
