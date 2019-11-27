---
title: CSP パートナー向けの Cloudyn 製 Azure Cost Management |パートナー センター
ms.topic: article
ms.date: 11/13/2019
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Cloudyn web アプリを登録し、パートナーセンターで秘密キーを使用する方法について説明します。これにより、アプリを使用して、お客様の Azure の使用状況とコストを追跡することができます。
author: Janet
ms.author: janet
Keywords: Azure コスト管理アプリ, コストの管理, Web アプリ
robots: ''
ms.localizationpriority: medium
ms.openlocfilehash: b05f2085aad63f8a0e23fa44de97550d13053f86
ms.sourcegitcommit: 524d3121e5053a74911e2fd4e9cf5aab14f6b48d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/20/2019
ms.locfileid: "74253296"
---
# <a name="azure-cost-management-app-for-azure-csp-partners"></a><span data-ttu-id="e1c79-104">Azure を販売する CSP パートナー様向けの Azure コスト管理アプリ</span><span class="sxs-lookup"><span data-stu-id="e1c79-104">Azure cost management app for Azure CSP partners</span></span>  

<span data-ttu-id="e1c79-105">**適用対象**</span><span class="sxs-lookup"><span data-stu-id="e1c79-105">**Applies to**</span></span>

- <span data-ttu-id="e1c79-106">パートナー センター</span><span class="sxs-lookup"><span data-stu-id="e1c79-106">Partner Center</span></span>
- <span data-ttu-id="e1c79-107">クラウド ソリューション プロバイダー プログラム パートナー</span><span class="sxs-lookup"><span data-stu-id="e1c79-107">Cloud Solution Provider program partners</span></span>

<span data-ttu-id="e1c79-108">**適切なロール**</span><span class="sxs-lookup"><span data-stu-id="e1c79-108">**Appropriate roles**</span></span>

- <span data-ttu-id="e1c79-109">全体管理者</span><span class="sxs-lookup"><span data-stu-id="e1c79-109">Global admin</span></span>
- <span data-ttu-id="e1c79-110">管理エージェント</span><span class="sxs-lookup"><span data-stu-id="e1c79-110">Admin agent</span></span>

[<span data-ttu-id="e1c79-111">Azure Cost Management の詳細情報</span><span class="sxs-lookup"><span data-stu-id="e1c79-111">Get More information about Azure Cost Management</span></span>](https://go.microsoft.com/fwlink/p/?linkid=857893)

## <a name="before-you-begin"></a><span data-ttu-id="e1c79-112">アンインストールの準備</span><span class="sxs-lookup"><span data-stu-id="e1c79-112">Before you begin</span></span>
<span data-ttu-id="e1c79-113">Azure Cost Management を使用する前に、次の要件を満たしていることを確認してください。</span><span class="sxs-lookup"><span data-stu-id="e1c79-113">Before you can use Azure Cost Management, be sure you meet the following requirements:</span></span>

- <span data-ttu-id="e1c79-114">クラウド ソリューション プロバイダー プログラムのパートナー様であること。</span><span class="sxs-lookup"><span data-stu-id="e1c79-114">You are a partner in the Cloud Solution Provider program.</span></span>
- <span data-ttu-id="e1c79-115">パートナー センター API Web アプリを作成できること。</span><span class="sxs-lookup"><span data-stu-id="e1c79-115">You have the ability to create a Partner Center API web app.</span></span>

## <a name="overview"></a><span data-ttu-id="e1c79-116">概要</span><span class="sxs-lookup"><span data-stu-id="e1c79-116">Overview</span></span>

<span data-ttu-id="e1c79-117">Cloudyn は、お客様による Azure の使用量とその使用量に対するコストを追跡、管理できる Web アプリです。</span><span class="sxs-lookup"><span data-stu-id="e1c79-117">Cloudyn is a web app that allows you to track and manage how much your customers are using Azure and the costs of that usage.</span></span> <span data-ttu-id="e1c79-118">このアプリは、パートナー センター API 経由で使用します。</span><span class="sxs-lookup"><span data-stu-id="e1c79-118">You use it through the Partner Center API.</span></span>

## <a name="register-your-web-app-in-the-partner-center"></a><span data-ttu-id="e1c79-119">パートナー センターで Web アプリを登録する</span><span class="sxs-lookup"><span data-stu-id="e1c79-119">Register your web app in the Partner Center</span></span>
<span data-ttu-id="e1c79-120">パートナー センターで Azure Active Directory Web アプリを登録すると、アプリがパートナー センター API にアクセスできるようになります。</span><span class="sxs-lookup"><span data-stu-id="e1c79-120">When you register an Azure Active Directory web app in Partner Center you enable access to the Partner Center API.</span></span> 
1.  <span data-ttu-id="e1c79-121">[全体管理者または管理エージェント アカウント](https://partnercenter.microsoft.com/pcv/dashboard/overview)を使って、[パートナー センター](create-user-accounts-and-set-permissions.md)にサインインします。</span><span class="sxs-lookup"><span data-stu-id="e1c79-121">Sign into [the Partner Center](https://partnercenter.microsoft.com/pcv/dashboard/overview) using a [global admin or admin agent account](create-user-accounts-and-set-permissions.md).</span></span>
2.  <span data-ttu-id="e1c79-122">**パートナー センター**から、 **[アカウント設定]** &gt; **[アプリ管理](https://partnercenter.microsoft.com/pcv/apiintegration/appmanagement)** を選択します。</span><span class="sxs-lookup"><span data-stu-id="e1c79-122">From the **Partner Center**, select **Account settings** &gt; **[App management](https://partnercenter.microsoft.com/pcv/apiintegration/appmanagement)**.</span></span>
3.  <span data-ttu-id="e1c79-123">**[Web アプリ]** セクションで、 **[新しいアプリの追加]** をクリックします。</span><span class="sxs-lookup"><span data-stu-id="e1c79-123">In the **Web App** section, click **Add new web app**.</span></span>
<br> <span data-ttu-id="e1c79-124">**注**: 既にアプリを作成済みの場合は、手順 3 を省略することができます。</span><span class="sxs-lookup"><span data-stu-id="e1c79-124">**Note**: If you have previously created a web app, you can skip step 3.</span></span>
4.  <span data-ttu-id="e1c79-125">登録する Web アプリの **商取引 ID** GUID と **アプリ ID** GUID をコピーして保存します。</span><span class="sxs-lookup"><span data-stu-id="e1c79-125">Copy and save the **Commerce ID** GUID and the **App ID** GUID for your web app.</span></span> <span data-ttu-id="e1c79-126">Azure cost management アプリの 30 日間無料試用版を利用するには、両方の ID が必要です。</span><span class="sxs-lookup"><span data-stu-id="e1c79-126">You will need both IDs to use the 30-day free trial of the Azure cost management app.</span></span>

## <a name="add-a-secret-key-to-your-app"></a><span data-ttu-id="e1c79-127">アプリへの秘密鍵の追加</span><span class="sxs-lookup"><span data-stu-id="e1c79-127">Add a secret key to your app</span></span>
1. <span data-ttu-id="e1c79-128">**[キーの追加]** ボタンの横のドロップ ダウンで、1 年間または 2 年間の期間を選択します。</span><span class="sxs-lookup"><span data-stu-id="e1c79-128">In the drop down next to the **Add key** button, select a duration of 1 or 2 years.</span></span>
2. <span data-ttu-id="e1c79-129">**[キーの追加]** をクリックします。</span><span class="sxs-lookup"><span data-stu-id="e1c79-129">Click **Add key**.</span></span> 
3. <span data-ttu-id="e1c79-130">秘密キーの値を書き留めて保存します。</span><span class="sxs-lookup"><span data-stu-id="e1c79-130">Copy and save the secret key value.</span></span> <span data-ttu-id="e1c79-131">この値は、30 日間無料試用版の利用に必要です。</span><span class="sxs-lookup"><span data-stu-id="e1c79-131">You will need this for the 30-day free trial.</span></span><br>
   > [!NOTE]  
   > <span data-ttu-id="e1c79-132">アプリケーションの秘密キーは、有効期限の長いパスワードのようなものです。</span><span class="sxs-lookup"><span data-stu-id="e1c79-132">The application secret keys are like passwords with longer expiration dates.</span></span> <span data-ttu-id="e1c79-133">後日使用できるように、安全な場所にキーの値を保存してください。</span><span class="sxs-lookup"><span data-stu-id="e1c79-133">Please save the key value in a secure location for future use.</span></span>

## <a name="next-steps"></a><span data-ttu-id="e1c79-134">次の手順</span><span class="sxs-lookup"><span data-stu-id="e1c79-134">Next steps</span></span>
<span data-ttu-id="e1c79-135">[30 日間無料試用版](https://go.microsoft.com/fwlink/?linkid=857895) をご利用ください。</span><span class="sxs-lookup"><span data-stu-id="e1c79-135">Start a [30-day free trial](https://go.microsoft.com/fwlink/?linkid=857895).</span></span>
<span data-ttu-id="e1c79-136">試用を開始するには、次の情報が必要です。</span><span class="sxs-lookup"><span data-stu-id="e1c79-136">You need the following details to start the trial:</span></span>
- <span data-ttu-id="e1c79-137">パートナー センターのログイン資格情報</span><span class="sxs-lookup"><span data-stu-id="e1c79-137">Partner Center sign in credentials</span></span>
- <span data-ttu-id="e1c79-138">商取引 ID GUID</span><span class="sxs-lookup"><span data-stu-id="e1c79-138">Commerce ID GUID</span></span>
- <span data-ttu-id="e1c79-139">アプリ ID GUID</span><span class="sxs-lookup"><span data-stu-id="e1c79-139">App ID GUID</span></span>
- <span data-ttu-id="e1c79-140">アプリケーションの秘密キーの値</span><span class="sxs-lookup"><span data-stu-id="e1c79-140">Application secret key value</span></span>
