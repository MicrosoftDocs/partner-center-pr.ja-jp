---
title: "CSP パートナー向けの Cloudyn 製 Azure Cost Management |パートナー センター"
description: "Cloudyn が提供する Azure Cost Management を使用するには、パートナー センター API へのアクセスをプロビジョニングする必要があります。"
author: Janet
Keywords: Azure cost management app, manage costs, web apps
robots: 
ms.openlocfilehash: 3d122e0f88867d16df3713f79e735126b7f40dd4
ms.sourcegitcommit: 628443b08dde9d2f02553b46e669504c620c3da4
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/21/2017
---
# <a name="azure-cost-management-app-for-azure-csp-partners"></a><span data-ttu-id="3aecf-103">Azure を販売する CSP パートナー様向けの Azure コスト管理アプリ</span><span class="sxs-lookup"><span data-stu-id="3aecf-103">Azure cost management app for Azure CSP partners</span></span>  

**<span data-ttu-id="3aecf-104">適用対象</span><span class="sxs-lookup"><span data-stu-id="3aecf-104">Applies to</span></span>**

-  <span data-ttu-id="3aecf-105">パートナー センター</span><span class="sxs-lookup"><span data-stu-id="3aecf-105">Partner Center</span></span>

[<span data-ttu-id="3aecf-106">Azure Cost Management の詳細情報を取得する</span><span class="sxs-lookup"><span data-stu-id="3aecf-106">Get More information about Azure Cost Management</span></span>](https://go.microsoft.com/fwlink/p/?linkid=857893)

## <a name="before-you-begin"></a><span data-ttu-id="3aecf-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="3aecf-107">Before you begin</span></span>
<span data-ttu-id="3aecf-108">Azure Cost Management を使用する前に、次の要件を満たしていることを確認してください。</span><span class="sxs-lookup"><span data-stu-id="3aecf-108">Before you can use Azure Cost Management, be sure you meet the following requirements:</span></span>
- <span data-ttu-id="3aecf-109">クラウド ソリューション プロバイダー プログラムのパートナー様であること。</span><span class="sxs-lookup"><span data-stu-id="3aecf-109">You are a partner in the Cloud Solution Provider program.</span></span>
- <span data-ttu-id="3aecf-110">パートナー センター API Web アプリを作成できること。</span><span class="sxs-lookup"><span data-stu-id="3aecf-110">You have the ability to create a Partner Center API web app.</span></span>

## <a name="overview"></a><span data-ttu-id="3aecf-111">概要</span><span class="sxs-lookup"><span data-stu-id="3aecf-111">Overview</span></span>

<span data-ttu-id="3aecf-112">Cloudyn が提供する Azure cost management は、お客様による Azure の使用量とその使用量に対応するコストを追跡、管理できる Web アプリです。</span><span class="sxs-lookup"><span data-stu-id="3aecf-112">Azure cost management by Cloudyn is a web app that allows you to track and manage how much your customers are using Azure and the costs of that usage.</span></span> <span data-ttu-id="3aecf-113">このアプリは、パートナー センター API 経由で使用します。</span><span class="sxs-lookup"><span data-stu-id="3aecf-113">You use it through the Partner Center API.</span></span>

## <a name="register-your-web-app-in-partner-center"></a><span data-ttu-id="3aecf-114">パートナー センターで Web アプリを登録する</span><span class="sxs-lookup"><span data-stu-id="3aecf-114">Register your web app in Partner Center</span></span>
<span data-ttu-id="3aecf-115">パートナー センターで Azure Active Directory Web アプリを登録すると、アプリがパートナー センター API にアクセスできるようになります。</span><span class="sxs-lookup"><span data-stu-id="3aecf-115">When you register an Azure Active Directory web app in Partner Center you enable access to the Partner Center API.</span></span> 
1.  <span data-ttu-id="3aecf-116">[グローバル管理者または管理エージェント アカウント](create-user-accounts-and-set-permissions.md)を使って、[パートナー センター](https://partnercenter.microsoft.com/en-us/pcv/dashboard/overview)にサインインします。</span><span class="sxs-lookup"><span data-stu-id="3aecf-116">Sign into [Partner Center](https://partnercenter.microsoft.com/en-us/pcv/dashboard/overview) using a [global admin or admin agent account](create-user-accounts-and-set-permissions.md).</span></span>
2.  <span data-ttu-id="3aecf-117">**[ダッシュボード]** で、**[アカウント設定]** &gt; **[[アプリ管理]](https://partnercenter.microsoft.com/en-us/pcv/apiintegration/appmanagement)** を選びます。</span><span class="sxs-lookup"><span data-stu-id="3aecf-117">From the **Dashboard**, select **Account settings** &gt; **[App management](https://partnercenter.microsoft.com/en-us/pcv/apiintegration/appmanagement)**.</span></span>
3.  <span data-ttu-id="3aecf-118">**[Web アプリ]** セクションで、**[新しいアプリの追加]** をクリックします。</span><span class="sxs-lookup"><span data-stu-id="3aecf-118">In the **Web App** section, click **Add new web app**.</span></span>
<br> <span data-ttu-id="3aecf-119">**注**: 既にアプリを作成済みの場合は、手順 3 を省略することができます。</span><span class="sxs-lookup"><span data-stu-id="3aecf-119">**Note**: If you have previously created a web app, you can skip step 3.</span></span>
4.  <span data-ttu-id="3aecf-120">登録する Web アプリの **商取引 ID** GUID と **アプリ ID** GUID をコピーして保存します。</span><span class="sxs-lookup"><span data-stu-id="3aecf-120">Copy and save the **Commerce ID** GUID and the **App ID** GUID for your web app.</span></span> <span data-ttu-id="3aecf-121">Azure cost management アプリの 30 日間無料試用版を利用するには、両方の ID が必要です。</span><span class="sxs-lookup"><span data-stu-id="3aecf-121">You will need both IDs to use the 30-day free trial of the Azure cost management app.</span></span>

## <a name="add-a-secret-key-to-your-app"></a><span data-ttu-id="3aecf-122">アプリへの秘密鍵の追加</span><span class="sxs-lookup"><span data-stu-id="3aecf-122">Add a secret key to your app</span></span>
1.  <span data-ttu-id="3aecf-123">**[キーの追加]** ボタンの横のドロップ ダウンで、1 年間または 2 年間の期間を選択します。</span><span class="sxs-lookup"><span data-stu-id="3aecf-123">In the drop down next to the **Add key** button, select a duration of 1 or 2 years.</span></span>
2.  <span data-ttu-id="3aecf-124">**[キーの追加]** をクリックします。</span><span class="sxs-lookup"><span data-stu-id="3aecf-124">Click **Add key**.</span></span> 
3.  <span data-ttu-id="3aecf-125">秘密キーの値を書き留めて保存します。</span><span class="sxs-lookup"><span data-stu-id="3aecf-125">Copy and save the secret key value.</span></span> <span data-ttu-id="3aecf-126">この値は、30 日間無料試用版の利用に必要です。</span><span class="sxs-lookup"><span data-stu-id="3aecf-126">You will need this for the 30-day free trial.</span></span>
<br><span data-ttu-id="3aecf-127">**注**: アプリケーションの秘密キーは、有効期限の長いパスワードのようなものです。</span><span class="sxs-lookup"><span data-stu-id="3aecf-127">**Note**: The application secret keys are like passwords with longer expiration dates.</span></span> <span data-ttu-id="3aecf-128">後日使用できるように、安全な場所にキーの値を保存してください。</span><span class="sxs-lookup"><span data-stu-id="3aecf-128">Please save the key value in a secure location for future use.</span></span>

## <a name="next-steps"></a><span data-ttu-id="3aecf-129">次のステップ</span><span class="sxs-lookup"><span data-stu-id="3aecf-129">Next steps</span></span>
<span data-ttu-id="3aecf-130">[30 日間無料試用版](https://go.microsoft.com/fwlink/?linkid=857895) をご利用ください。</span><span class="sxs-lookup"><span data-stu-id="3aecf-130">Start a [30-day free trial](https://go.microsoft.com/fwlink/?linkid=857895).</span></span>
<span data-ttu-id="3aecf-131">試用を開始するには、次の情報が必要です。</span><span class="sxs-lookup"><span data-stu-id="3aecf-131">You need the following details to start the trial:</span></span>
- <span data-ttu-id="3aecf-132">パートナー センターのログイン資格情報</span><span class="sxs-lookup"><span data-stu-id="3aecf-132">Partner Center sign in credentials</span></span>
- <span data-ttu-id="3aecf-133">商取引 ID GUID</span><span class="sxs-lookup"><span data-stu-id="3aecf-133">Commerce ID GUID</span></span>
- <span data-ttu-id="3aecf-134">アプリ ID GUID</span><span class="sxs-lookup"><span data-stu-id="3aecf-134">App ID GUID</span></span>
- <span data-ttu-id="3aecf-135">アプリケーションの秘密キーの値</span><span class="sxs-lookup"><span data-stu-id="3aecf-135">Application secret key value</span></span>
