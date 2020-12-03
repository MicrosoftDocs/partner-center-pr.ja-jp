---
title: CSP 用の Cloudyn 製 Azure Cost Management
ms.topic: article
ms.date: 05/04/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Cloudyn web アプリを登録し、パートナーセンターで秘密キーを使用する方法について説明します。これにより、アプリを使用して、お客様の Azure の使用状況とコストを追跡することができます。
author: aparnagkrishnan
ms.author: aparnag
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: defa691a3bc70cbda45f01cb447d89364a49e3b8
ms.sourcegitcommit: 2d9aab15ddc20cb3d9537e68ace33d36f7d8a250
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/02/2020
ms.locfileid: "96534992"
---
# <a name="track-customer-azure-usage-and-costs-with-the-azure-cost-management-app-for-csp-partners"></a><span data-ttu-id="c8848-103">CSP パートナー向けの Azure cost management アプリを使用して、お客様の Azure の使用状況とコストを追跡します</span><span class="sxs-lookup"><span data-stu-id="c8848-103">Track customer Azure usage and costs with the Azure cost management app for CSP partners</span></span>  

<span data-ttu-id="c8848-104">**適切なロール**</span><span class="sxs-lookup"><span data-stu-id="c8848-104">**Appropriate roles**</span></span>

- <span data-ttu-id="c8848-105">グローバル管理者</span><span class="sxs-lookup"><span data-stu-id="c8848-105">Global admin</span></span>
- <span data-ttu-id="c8848-106">管理エージェント</span><span class="sxs-lookup"><span data-stu-id="c8848-106">Admin agent</span></span>

[<span data-ttu-id="c8848-107">Azure Cost Management の詳細情報</span><span class="sxs-lookup"><span data-stu-id="c8848-107">Get More information about Azure Cost Management</span></span>](https://go.microsoft.com/fwlink/p/?linkid=857893)

## <a name="before-you-begin"></a><span data-ttu-id="c8848-108">開始する前に</span><span class="sxs-lookup"><span data-stu-id="c8848-108">Before you begin</span></span>
<span data-ttu-id="c8848-109">Azure Cost Management を使用する前に、次の要件を満たしていることを確認してください。</span><span class="sxs-lookup"><span data-stu-id="c8848-109">Before you can use Azure Cost Management, be sure you meet the following requirements:</span></span>

- <span data-ttu-id="c8848-110">クラウド ソリューション プロバイダー プログラムのパートナー様であること。</span><span class="sxs-lookup"><span data-stu-id="c8848-110">You are a partner in the Cloud Solution Provider program.</span></span>
- <span data-ttu-id="c8848-111">パートナー センター API Web アプリを作成できること。</span><span class="sxs-lookup"><span data-stu-id="c8848-111">You have the ability to create a Partner Center API web app.</span></span>

## <a name="overview"></a><span data-ttu-id="c8848-112">概要</span><span class="sxs-lookup"><span data-stu-id="c8848-112">Overview</span></span>

<span data-ttu-id="c8848-113">Cloudyn は、お客様による Azure の使用量とその使用量に対するコストを追跡、管理できる Web アプリです。</span><span class="sxs-lookup"><span data-stu-id="c8848-113">Cloudyn is a web app that allows you to track and manage how much your customers are using Azure and the costs of that usage.</span></span> <span data-ttu-id="c8848-114">このアプリは、パートナー センター API 経由で使用します。</span><span class="sxs-lookup"><span data-stu-id="c8848-114">You use it through the Partner Center API.</span></span>

## <a name="register-your-web-app-in-the-partner-center"></a><span data-ttu-id="c8848-115">パートナー センターで Web アプリを登録する</span><span class="sxs-lookup"><span data-stu-id="c8848-115">Register your web app in the Partner Center</span></span>
<span data-ttu-id="c8848-116">パートナー センターで Azure Active Directory Web アプリを登録すると、アプリがパートナー センター API にアクセスできるようになります。</span><span class="sxs-lookup"><span data-stu-id="c8848-116">When you register an Azure Active Directory web app in Partner Center you enable access to the Partner Center API.</span></span> 
1.  <span data-ttu-id="c8848-117">[グローバル管理者または管理エージェント アカウント](create-user-accounts-and-set-permissions.md)を使って、[パートナー センター](https://partnercenter.microsoft.com/pcv/dashboard/overview)にサインインします。</span><span class="sxs-lookup"><span data-stu-id="c8848-117">Sign into [Partner Center](https://partnercenter.microsoft.com/pcv/dashboard/overview) using a [global admin or admin agent account](create-user-accounts-and-set-permissions.md).</span></span>
2.  <span data-ttu-id="c8848-118">**パートナーセンター** で、[**アカウント設定**] [ &gt; **[アプリ管理](https://partnercenter.microsoft.com/pcv/apiintegration/appmanagement)**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="c8848-118">From **Partner Center**, select **Account settings** &gt; **[App management](https://partnercenter.microsoft.com/pcv/apiintegration/appmanagement)**.</span></span>
3.  <span data-ttu-id="c8848-119">**[Web アプリ]** セクションで、**[新しいアプリの追加]** をクリックします。</span><span class="sxs-lookup"><span data-stu-id="c8848-119">In the **Web App** section, click **Add new web app**.</span></span>
<br> <span data-ttu-id="c8848-120">**注**: 既にアプリを作成済みの場合は、手順 3 を省略することができます。</span><span class="sxs-lookup"><span data-stu-id="c8848-120">**Note**: If you have previously created a web app, you can skip step 3.</span></span>
4.  <span data-ttu-id="c8848-121">登録する Web アプリの **商取引 ID** GUID と **アプリ ID** GUID をコピーして保存します。</span><span class="sxs-lookup"><span data-stu-id="c8848-121">Copy and save the **Commerce ID** GUID and the **App ID** GUID for your web app.</span></span> <span data-ttu-id="c8848-122">Azure cost management アプリの 30 日間無料試用版を利用するには、両方の ID が必要です。</span><span class="sxs-lookup"><span data-stu-id="c8848-122">You will need both IDs to use the 30-day free trial of the Azure cost management app.</span></span>

## <a name="add-a-secret-key-to-your-app"></a><span data-ttu-id="c8848-123">アプリへの秘密鍵の追加</span><span class="sxs-lookup"><span data-stu-id="c8848-123">Add a secret key to your app</span></span>
1. <span data-ttu-id="c8848-124">**[キーの追加]** ボタンの横のドロップ ダウンで、1 年間または 2 年間の期間を選択します。</span><span class="sxs-lookup"><span data-stu-id="c8848-124">In the drop down next to the **Add key** button, select a duration of 1 or 2 years.</span></span>
2. <span data-ttu-id="c8848-125">[ **キーの追加**] をクリックします。</span><span class="sxs-lookup"><span data-stu-id="c8848-125">Click **Add key**.</span></span> 
3. <span data-ttu-id="c8848-126">秘密キーの値を書き留めて保存します。</span><span class="sxs-lookup"><span data-stu-id="c8848-126">Copy and save the secret key value.</span></span> <span data-ttu-id="c8848-127">この値は、30 日間無料試用版の利用に必要です。</span><span class="sxs-lookup"><span data-stu-id="c8848-127">You will need this for the 30-day free trial.</span></span><br>
   > [!NOTE]  
   > <span data-ttu-id="c8848-128">アプリケーションの秘密キーは、有効期限の長いパスワードのようなものです。</span><span class="sxs-lookup"><span data-stu-id="c8848-128">The application secret keys are like passwords with longer expiration dates.</span></span> <span data-ttu-id="c8848-129">後日使用できるように、安全な場所にキーの値を保存してください。</span><span class="sxs-lookup"><span data-stu-id="c8848-129">Please save the key value in a secure location for future use.</span></span>

## <a name="next-steps"></a><span data-ttu-id="c8848-130">次のステップ</span><span class="sxs-lookup"><span data-stu-id="c8848-130">Next steps</span></span>
<span data-ttu-id="c8848-131">[30 日間無料試用版](https://go.microsoft.com/fwlink/?linkid=857895) をご利用ください。</span><span class="sxs-lookup"><span data-stu-id="c8848-131">Start a [30-day free trial](https://go.microsoft.com/fwlink/?linkid=857895).</span></span>
<span data-ttu-id="c8848-132">試用を開始するには、次の情報が必要です。</span><span class="sxs-lookup"><span data-stu-id="c8848-132">You need the following details to start the trial:</span></span>
- <span data-ttu-id="c8848-133">パートナー センターのログイン資格情報</span><span class="sxs-lookup"><span data-stu-id="c8848-133">Partner Center sign in credentials</span></span>
- <span data-ttu-id="c8848-134">商取引 ID GUID</span><span class="sxs-lookup"><span data-stu-id="c8848-134">Commerce ID GUID</span></span>
- <span data-ttu-id="c8848-135">アプリ ID GUID</span><span class="sxs-lookup"><span data-stu-id="c8848-135">App ID GUID</span></span>
- <span data-ttu-id="c8848-136">アプリケーションの秘密キーの値</span><span class="sxs-lookup"><span data-stu-id="c8848-136">Application secret key value</span></span>
