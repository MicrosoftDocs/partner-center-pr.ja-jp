---
title: Power BI 用のパートナーセンター分析のインストール
ms.topic: article
ms.date: 07/10/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: この記事の手順に従って、Power BI 用のパートナーセンター分析アプリ (CSP のダイレクトパートナー向け) をインストールしてプレビューします。
fwlink: https://go.microsoft.com/fwlink/?linkid=852583
author: v-sumukh
ms.author: v-sumukh
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: ad0c2f3ee7d130c49dea6ba354e6794e29fd9e9f
ms.sourcegitcommit: a691d4cbe144a8fd71e344fd293cc658ac11d6f3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/27/2021
ms.locfileid: "105633694"
---
# <a name="install-and-preview-the-partner-center-analytics-app-for-microsoft-power-bi"></a><span data-ttu-id="d2b9c-103">Power BI 用パートナー センター分析アプリをインストールしてプレビューする</span><span class="sxs-lookup"><span data-stu-id="d2b9c-103">Install and preview the Partner Center Analytics app for Microsoft Power BI</span></span>


<span data-ttu-id="d2b9c-104">**適切なロール**</span><span class="sxs-lookup"><span data-stu-id="d2b9c-104">**Appropriate roles**</span></span>

- <span data-ttu-id="d2b9c-105">グローバル管理者</span><span class="sxs-lookup"><span data-stu-id="d2b9c-105">Global admin</span></span>
- <span data-ttu-id="d2b9c-106">ユーザー管理の管理者</span><span class="sxs-lookup"><span data-stu-id="d2b9c-106">User management admin</span></span>
- <span data-ttu-id="d2b9c-107">販売代理店</span><span class="sxs-lookup"><span data-stu-id="d2b9c-107">Sales agent</span></span>
- <span data-ttu-id="d2b9c-108">管理エージェント</span><span class="sxs-lookup"><span data-stu-id="d2b9c-108">Admin agent</span></span>

## <a name="before-you-begin"></a><span data-ttu-id="d2b9c-109">開始する前に</span><span class="sxs-lookup"><span data-stu-id="d2b9c-109">Before you begin</span></span>

<span data-ttu-id="d2b9c-110">使用可能な Power BI アプリの次の一覧から、自分のビジネスに最も関係のあるアプリケーションを選択します。</span><span class="sxs-lookup"><span data-stu-id="d2b9c-110">Select the application that is most relevant to your business from the following list of available Power BI apps:</span></span>

- [<span data-ttu-id="d2b9c-111">直接プロバイダー</span><span class="sxs-lookup"><span data-stu-id="d2b9c-111">Direct Provider</span></span>](https://appsource.microsoft.com/product/power-bi/partnercenteranalytics.direct_provider_partner_analytics)

- [<span data-ttu-id="d2b9c-112">間接プロバイダー</span><span class="sxs-lookup"><span data-stu-id="d2b9c-112">Indirect Provider</span></span>](https://appsource.microsoft.com/product/power-bi/partnercenteranalytics.indirect_provider_partner_analytics)

- [<span data-ttu-id="d2b9c-113">間接リセラー</span><span class="sxs-lookup"><span data-stu-id="d2b9c-113">Indirect Reseller</span></span>](https://appsource.microsoft.com/product/power-bi/partnercenteranalytics.indirect_reseller_partner_analytics)

<span data-ttu-id="d2b9c-114">パートナー センター分析アプリのプレビュー バージョンをインストールする前に、次の要件を満たしていることを確認してください。</span><span class="sxs-lookup"><span data-stu-id="d2b9c-114">Before you install the Partner Center Analytics app preview version, be sure that you meet the following requirements.</span></span>

- <span data-ttu-id="d2b9c-115">自分のビジネスに合った Power BI アプリを選択している。</span><span class="sxs-lookup"><span data-stu-id="d2b9c-115">You pick the correct Power BI app for your business.</span></span>

- <span data-ttu-id="d2b9c-116">Power BI pro ライセンスを持っている。</span><span class="sxs-lookup"><span data-stu-id="d2b9c-116">You have a Power BI pro license.</span></span>

- <span data-ttu-id="d2b9c-117">テナントにテンプレートアプリをインストールするためのアクセス許可があります。</span><span class="sxs-lookup"><span data-stu-id="d2b9c-117">You have permissions to install template apps on your tenant.</span></span>

- <span data-ttu-id="d2b9c-118">Power BI にログインできる。</span><span class="sxs-lookup"><span data-stu-id="d2b9c-118">You can sign in to Power BI.</span></span>

- <span data-ttu-id="d2b9c-119">[会社の Azure Active Directory (Azure AD) テナント](azure-active-directory-tenants-and-partner-center.md)に、グローバル管理者、管理エージェント、または課金管理者としてサインインできます。</span><span class="sxs-lookup"><span data-stu-id="d2b9c-119">You can sign in as a global admin, admin agent, or billing admin to [your company's Azure Active Directory (Azure AD) tenant](azure-active-directory-tenants-and-partner-center.md).</span></span>

## <a name="to-install-the-app"></a><span data-ttu-id="d2b9c-120">アプリをインストールするには</span><span class="sxs-lookup"><span data-stu-id="d2b9c-120">To install the app</span></span>

1. <span data-ttu-id="d2b9c-121">上記のセクションで、指定されたアプリソースリンク (Direct Provider/間接プロバイダ/間接リセラー) を選択します。</span><span class="sxs-lookup"><span data-stu-id="d2b9c-121">Select the app source link given (Direct Provider/Indirect Provider/Indirect Reseller) in the above section.</span></span>

2. <span data-ttu-id="d2b9c-122">**[今すぐ入手する]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="d2b9c-122">Select **GET IT NOW**.</span></span> 

3. <span data-ttu-id="d2b9c-123">[ **続行**] を選択して、使用条件に同意します。</span><span class="sxs-lookup"><span data-stu-id="d2b9c-123">Agree terms and conditions by selecting **Continue**.</span></span>

4. <span data-ttu-id="d2b9c-124">[アカウントを既にお持ちの場合] の下で **[サインイン]** を選びます。</span><span class="sxs-lookup"><span data-stu-id="d2b9c-124">Under Already have an account? select **Sign In**.</span></span>

5. <span data-ttu-id="d2b9c-125">次のページで Power BI のユーザー名とパスワードを入力し、**[サインイン]** を選びます。</span><span class="sxs-lookup"><span data-stu-id="d2b9c-125">On the next page, enter your Power BI user name and password and then select **Sign In**.</span></span>

6. <span data-ttu-id="d2b9c-126">ワークスペース名を指定して、ワークスペースをインストールします。</span><span class="sxs-lookup"><span data-stu-id="d2b9c-126">Install the workspace by providing the workspace name.</span></span>

7. <span data-ttu-id="d2b9c-127">インストールされているテンプレートアプリは、[アプリ] セクションで確認できます。</span><span class="sxs-lookup"><span data-stu-id="d2b9c-127">You can find the template apps installed under Apps Section.</span></span>

8. <span data-ttu-id="d2b9c-128">[ **アプリ** ] を選択し、インストールされているアプリを選択します。</span><span class="sxs-lookup"><span data-stu-id="d2b9c-128">Select **Apps** and choose the installed apps.</span></span>

9. <span data-ttu-id="d2b9c-129">[新しいアプリの開始] 画面が開きます。</span><span class="sxs-lookup"><span data-stu-id="d2b9c-129">Get Started with your new app screen opens.</span></span>

10. <span data-ttu-id="d2b9c-130">データに接続するには、[ **接続**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="d2b9c-130">To connect to the data, select **Connect**.</span></span>

11. <span data-ttu-id="d2b9c-131">[ **Partner Center Analytics への接続** ] ポップアップウィンドウで、[ **認証方法** ] が [ **oAuth2** ] に設定されていることを確認するか、表示されていない場合は一覧から **oAuth2** を選択します。</span><span class="sxs-lookup"><span data-stu-id="d2b9c-131">On the **Connect to Partner Center Analytics** pop-up window, verify that the **Authentication method** is set to **oAuth2** or select **oAuth2** from the list if it's not.</span></span> 

> [!NOTE]  
>  <span data-ttu-id="d2b9c-132">このウィンドウが表示されるまでに数分間かかることがあります。</span><span class="sxs-lookup"><span data-stu-id="d2b9c-132">This window may take a few minutes to appear.</span></span>

12. <span data-ttu-id="d2b9c-133">[ **Partner Center Analytics コネクタ** ] ページで、会社の Azure AD テナントのグローバル管理者、管理エージェント、または課金管理者の資格情報を使用してサインインし、[ **サインイン**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="d2b9c-133">On the **Partner Center Analytics Connector** page, sign in with global admin, admin agent, or billing admin credentials for your company's Azure AD tenant, and then select **Sign In**.</span></span>
 
13. <span data-ttu-id="d2b9c-134">アクセスするかどうかを尋ねられたら、**[同意する]** を選びます。</span><span class="sxs-lookup"><span data-stu-id="d2b9c-134">When prompted for access, select **Accept**.</span></span> 

<span data-ttu-id="d2b9c-135">パートナー センターの分析サービスが Power BI に接続されると、データの読み込みが開始します。</span><span class="sxs-lookup"><span data-stu-id="d2b9c-135">Once the Partner Center Analytics service is connected to Power BI, data will begin to load.</span></span> <span data-ttu-id="d2b9c-136">データ量によっては、この読み込みに最大 10 分間かかります。</span><span class="sxs-lookup"><span data-stu-id="d2b9c-136">Depending on the amount of data, this can take up to 10 minutes.</span></span> 

<span data-ttu-id="d2b9c-137">データの読み込みが完了すると、Power BI でパートナー センターの分析アプリのダッシュボードとレポートを使用できるようになります。</span><span class="sxs-lookup"><span data-stu-id="d2b9c-137">After the data finishes loading, you can start using the Partner Center Analytics app dashboard and reports in Power BI.</span></span>

## <a name="next-steps"></a><span data-ttu-id="d2b9c-138">次のステップ</span><span class="sxs-lookup"><span data-stu-id="d2b9c-138">Next steps</span></span>

[<span data-ttu-id="d2b9c-139">Microsoft Power BI 用パートナー センター分析アプリでビジネス データを表示する</span><span class="sxs-lookup"><span data-stu-id="d2b9c-139">View your business data with the Partner Center Analytics app for Microsoft Power BI</span></span>](power-bi-app-for-direct-partners-use.md)
