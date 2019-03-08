---
title: CSP パートナー向けの Cloudyn 製 Azure Cost Management |パートナー センター
ms.topic: article
ms.date: 10/29/2018
description: Cloudyn が提供する Azure Cost Management を使用するには、パートナー センター API へのアクセスをプロビジョニングする必要があります。
author: Janet
ms.author: janet
Keywords: Azure コスト管理アプリでは、管理コストの削減、web アプリ
robots: ''
ms.localizationpriority: medium
ms.openlocfilehash: 586ec2936b8491e91b4f2a56cbc392e4dee350b3
ms.sourcegitcommit: 4c34d6fcaf020bcc53eaa5f0379011a56149a14f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/05/2019
ms.locfileid: "57586085"
---
# <a name="azure-cost-management-app-for-azure-csp-partners"></a><span data-ttu-id="45f4a-104">Azure を販売する CSP パートナー様向けの Azure コスト管理アプリ</span><span class="sxs-lookup"><span data-stu-id="45f4a-104">Azure cost management app for Azure CSP partners</span></span>  

<span data-ttu-id="45f4a-105">**適用対象**</span><span class="sxs-lookup"><span data-stu-id="45f4a-105">**Applies to**</span></span>

-  <span data-ttu-id="45f4a-106">パートナー センター</span><span class="sxs-lookup"><span data-stu-id="45f4a-106">Partner Center</span></span>

[<span data-ttu-id="45f4a-107">Azure Cost Management について詳細を取得します。</span><span class="sxs-lookup"><span data-stu-id="45f4a-107">Get More information about Azure Cost Management</span></span>](https://go.microsoft.com/fwlink/p/?linkid=857893)

## <a name="before-you-begin"></a><span data-ttu-id="45f4a-108">始める前に</span><span class="sxs-lookup"><span data-stu-id="45f4a-108">Before you begin</span></span>
<span data-ttu-id="45f4a-109">Azure Cost Management を使用する前に、次の要件を満たしていることを確認してください。</span><span class="sxs-lookup"><span data-stu-id="45f4a-109">Before you can use Azure Cost Management, be sure you meet the following requirements:</span></span>

- <span data-ttu-id="45f4a-110">クラウド ソリューション プロバイダー プログラムのパートナー様であること。</span><span class="sxs-lookup"><span data-stu-id="45f4a-110">You are a partner in the Cloud Solution Provider program.</span></span>
- <span data-ttu-id="45f4a-111">パートナー センター API Web アプリを作成できること。</span><span class="sxs-lookup"><span data-stu-id="45f4a-111">You have the ability to create a Partner Center API web app.</span></span>

## <a name="overview"></a><span data-ttu-id="45f4a-112">概要</span><span class="sxs-lookup"><span data-stu-id="45f4a-112">Overview</span></span>

<span data-ttu-id="45f4a-113">Cloudyn が提供する Azure cost management は、お客様による Azure の使用量とその使用量に対応するコストを追跡、管理できる Web アプリです。</span><span class="sxs-lookup"><span data-stu-id="45f4a-113">Azure cost management by Cloudyn is a web app that allows you to track and manage how much your customers are using Azure and the costs of that usage.</span></span> <span data-ttu-id="45f4a-114">このアプリは、パートナー センター API 経由で使用します。</span><span class="sxs-lookup"><span data-stu-id="45f4a-114">You use it through the Partner Center API.</span></span>

## <a name="register-your-web-app-in-the-partner-center"></a><span data-ttu-id="45f4a-115">パートナー センターで Web アプリを登録する</span><span class="sxs-lookup"><span data-stu-id="45f4a-115">Register your web app in the Partner Center</span></span>
<span data-ttu-id="45f4a-116">パートナー センターで Azure Active Directory Web アプリを登録すると、アプリがパートナー センター API にアクセスできるようになります。</span><span class="sxs-lookup"><span data-stu-id="45f4a-116">When you register an Azure Active Directory web app in Partner Center you enable access to the the Partner Center API.</span></span> 
1.  <span data-ttu-id="45f4a-117">[全体管理者または管理エージェント アカウント](create-user-accounts-and-set-permissions.md)を使って、[パートナー センター](https://partnercenter.microsoft.com/en-us/pcv/dashboard/overview)にサインインします。</span><span class="sxs-lookup"><span data-stu-id="45f4a-117">Sign into [the Partner Center](https://partnercenter.microsoft.com/en-us/pcv/dashboard/overview) using a [global admin or admin agent account](create-user-accounts-and-set-permissions.md).</span></span>
2.  <span data-ttu-id="45f4a-118">**パートナー センター**、**アカウント設定** &gt; **[アプリ管理](https://partnercenter.microsoft.com/en-us/pcv/apiintegration/appmanagement)** します。</span><span class="sxs-lookup"><span data-stu-id="45f4a-118">From the **Partner Center**, select **Account settings** &gt; **[App management](https://partnercenter.microsoft.com/en-us/pcv/apiintegration/appmanagement)**.</span></span>
3.  <span data-ttu-id="45f4a-119">**[Web アプリ]** セクションで、**[新しいアプリの追加]** をクリックします。</span><span class="sxs-lookup"><span data-stu-id="45f4a-119">In the **Web App** section, click **Add new web app**.</span></span>
<br> <span data-ttu-id="45f4a-120">**注意**:Web アプリを作成していた場合は、手順 3. を省略できます。</span><span class="sxs-lookup"><span data-stu-id="45f4a-120">**Note**: If you have previously created a web app, you can skip step 3.</span></span>
4.  <span data-ttu-id="45f4a-121">登録する Web アプリの **商取引 ID** GUID と **アプリ ID** GUID をコピーして保存します。</span><span class="sxs-lookup"><span data-stu-id="45f4a-121">Copy and save the **Commerce ID** GUID and the **App ID** GUID for your web app.</span></span> <span data-ttu-id="45f4a-122">Azure cost management アプリの 30 日間無料試用版を利用するには、両方の ID が必要です。</span><span class="sxs-lookup"><span data-stu-id="45f4a-122">You will need both IDs to use the 30-day free trial of the Azure cost management app.</span></span>

## <a name="add-a-secret-key-to-your-app"></a><span data-ttu-id="45f4a-123">アプリへの秘密鍵の追加</span><span class="sxs-lookup"><span data-stu-id="45f4a-123">Add a secret key to your app</span></span>
1. <span data-ttu-id="45f4a-124">**[キーの追加]** ボタンの横のドロップ ダウンで、1 年間または 2 年間の期間を選択します。</span><span class="sxs-lookup"><span data-stu-id="45f4a-124">In the drop down next to the **Add key** button, select a duration of 1 or 2 years.</span></span>
2. <span data-ttu-id="45f4a-125">**[キーの追加]** をクリックします。</span><span class="sxs-lookup"><span data-stu-id="45f4a-125">Click **Add key**.</span></span> 
3. <span data-ttu-id="45f4a-126">秘密キーの値を書き留めて保存します。</span><span class="sxs-lookup"><span data-stu-id="45f4a-126">Copy and save the secret key value.</span></span> <span data-ttu-id="45f4a-127">この値は、30 日間無料試用版の利用に必要です。</span><span class="sxs-lookup"><span data-stu-id="45f4a-127">You will need this for the 30-day free trial.</span></span><br>
   > [!NOTE]  
   > <span data-ttu-id="45f4a-128">アプリケーションの秘密キーでは、パスワードより長い有効期限と同様です。</span><span class="sxs-lookup"><span data-stu-id="45f4a-128">The application secret keys are like passwords with longer expiration dates.</span></span> <span data-ttu-id="45f4a-129">後日使用できるように、安全な場所にキーの値を保存してください。</span><span class="sxs-lookup"><span data-stu-id="45f4a-129">Please save the key value in a secure location for future use.</span></span>

## <a name="next-steps"></a><span data-ttu-id="45f4a-130">次のステップ</span><span class="sxs-lookup"><span data-stu-id="45f4a-130">Next steps</span></span>
<span data-ttu-id="45f4a-131">[30 日間無料試用版](https://go.microsoft.com/fwlink/?linkid=857895) をご利用ください。</span><span class="sxs-lookup"><span data-stu-id="45f4a-131">Start a [30-day free trial](https://go.microsoft.com/fwlink/?linkid=857895).</span></span>
<span data-ttu-id="45f4a-132">試用を開始するには、次の情報が必要です。</span><span class="sxs-lookup"><span data-stu-id="45f4a-132">You need the following details to start the trial:</span></span>
- <span data-ttu-id="45f4a-133">パートナー センターのログイン資格情報</span><span class="sxs-lookup"><span data-stu-id="45f4a-133">Partner Center sign in credentials</span></span>
- <span data-ttu-id="45f4a-134">商取引 ID GUID</span><span class="sxs-lookup"><span data-stu-id="45f4a-134">Commerce ID GUID</span></span>
- <span data-ttu-id="45f4a-135">アプリ ID GUID</span><span class="sxs-lookup"><span data-stu-id="45f4a-135">App ID GUID</span></span>
- <span data-ttu-id="45f4a-136">アプリケーションの秘密キーの値</span><span class="sxs-lookup"><span data-stu-id="45f4a-136">Application secret key value</span></span>
