---
title: Power BI 用のパートナーセンター分析のインストール
ms.topic: article
ms.date: 05/19/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: この記事の手順に従って、Power BI 用のパートナーセンター分析アプリ (CSP のダイレクトパートナー向け) をインストールしてプレビューします。
fwlink: https://go.microsoft.com/fwlink/?linkid=852583
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 7e2a1d17a7520cca1a6e1da540cc58d2d365d8cb
ms.sourcegitcommit: ecc5472c986e67525dbfcc6fc328c991d6db77ba
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/10/2020
ms.locfileid: "84679309"
---
# <a name="install-and-preview-the-partner-center-analytics-app-for-microsoft-power-bi"></a><span data-ttu-id="c9b8e-103">Power BI 用パートナー センター分析アプリをインストールしてプレビューする</span><span class="sxs-lookup"><span data-stu-id="c9b8e-103">Install and preview the Partner Center Analytics app for Microsoft Power BI</span></span>

<span data-ttu-id="c9b8e-104">**適用対象**</span><span class="sxs-lookup"><span data-stu-id="c9b8e-104">**Applies to**</span></span>

- <span data-ttu-id="c9b8e-105">パートナー センター</span><span class="sxs-lookup"><span data-stu-id="c9b8e-105">Partner Center</span></span>

<span data-ttu-id="c9b8e-106">**適切なロール**</span><span class="sxs-lookup"><span data-stu-id="c9b8e-106">**Appropriate roles**</span></span>
-   <span data-ttu-id="c9b8e-107">グローバル管理者</span><span class="sxs-lookup"><span data-stu-id="c9b8e-107">Global admin</span></span>
-   <span data-ttu-id="c9b8e-108">ユーザー管理者</span><span class="sxs-lookup"><span data-stu-id="c9b8e-108">User admin</span></span>
-   <span data-ttu-id="c9b8e-109">販売代理店</span><span class="sxs-lookup"><span data-stu-id="c9b8e-109">Sales agent</span></span>
-   <span data-ttu-id="c9b8e-110">管理エージェント</span><span class="sxs-lookup"><span data-stu-id="c9b8e-110">Admin agent</span></span>

## <a name="before-you-begin"></a><span data-ttu-id="c9b8e-111">開始する前に</span><span class="sxs-lookup"><span data-stu-id="c9b8e-111">Before you begin</span></span>

<span data-ttu-id="c9b8e-112">使用可能な Power BI アプリの次の一覧から、自分のビジネスに最も関係のあるアプリケーションを選択します。</span><span class="sxs-lookup"><span data-stu-id="c9b8e-112">Select the application that is most relevant to your business from the following list of available Power BI apps:</span></span>
- [<span data-ttu-id="c9b8e-113">直接プロバイダー</span><span class="sxs-lookup"><span data-stu-id="c9b8e-113">Direct Provider</span></span>](https://appsource.microsoft.com/en-us/product/power-bi/partnercenteranalytics.direct_provider_partner_analytics)

- [<span data-ttu-id="c9b8e-114">間接プロバイダー</span><span class="sxs-lookup"><span data-stu-id="c9b8e-114">Indirect Provider</span></span>](https://appsource.microsoft.com/en-us/product/power-bi/partnercenteranalytics.indirect_provider_partner_analytics)

- [<span data-ttu-id="c9b8e-115">間接リセラー</span><span class="sxs-lookup"><span data-stu-id="c9b8e-115">Indirect Reseller</span></span>](https://appsource.microsoft.com/en-us/product/power-bi/partnercenteranalytics.indirect_reseller_partner_analytics)

<span data-ttu-id="c9b8e-116">パートナー センター分析アプリのプレビュー バージョンをインストールする前に、次の要件を満たしていることを確認してください。</span><span class="sxs-lookup"><span data-stu-id="c9b8e-116">Before you install the Partner Center Analytics app preview version, be sure that you meet the following requirements.</span></span>

- <span data-ttu-id="c9b8e-117">自分のビジネスに合った Power BI アプリを選択している。</span><span class="sxs-lookup"><span data-stu-id="c9b8e-117">You pick the correct Power BI app for your business.</span></span>

- <span data-ttu-id="c9b8e-118">Power BI pro ライセンスを持っている。</span><span class="sxs-lookup"><span data-stu-id="c9b8e-118">You have a Power BI pro license.</span></span>

- <span data-ttu-id="c9b8e-119">テナントにテンプレートアプリをインストールするためのアクセス許可があります。</span><span class="sxs-lookup"><span data-stu-id="c9b8e-119">You have permissions to install template apps on your tenant.</span></span>

- <span data-ttu-id="c9b8e-120">Power BI にログインできる。</span><span class="sxs-lookup"><span data-stu-id="c9b8e-120">You can sign in to Power BI.</span></span>

- <span data-ttu-id="c9b8e-121">[会社の Azure Active Directory (Azure AD) テナント](azure-active-directory-tenants-and-partner-center.md)に、グローバル管理者、管理エージェント、または課金管理者としてサインインできます。</span><span class="sxs-lookup"><span data-stu-id="c9b8e-121">You can sign in as a global admin, admin agent, or billing admin to [your company's Azure Active Directory (Azure AD) tenant](azure-active-directory-tenants-and-partner-center.md).</span></span>

## <a name="to-install-the-app"></a><span data-ttu-id="c9b8e-122">アプリをインストールするには</span><span class="sxs-lookup"><span data-stu-id="c9b8e-122">To install the app</span></span>

1. <span data-ttu-id="c9b8e-123">上記のセクションで、指定されたアプリソースリンク (Direct Provider/間接プロバイダ/間接リセラー) をクリックします。</span><span class="sxs-lookup"><span data-stu-id="c9b8e-123">Click on the app source link given (Direct Provider/Indirect Provider/Indirect Reseller) in the above section.</span></span>

2. <span data-ttu-id="c9b8e-124">[**今すぐ入手**する] をクリックします。</span><span class="sxs-lookup"><span data-stu-id="c9b8e-124">Click on **GET IT NOW**.</span></span> 

3. <span data-ttu-id="c9b8e-125">[**続行**] をクリックして使用条件に同意します。</span><span class="sxs-lookup"><span data-stu-id="c9b8e-125">Agree terms and conditions by clicking **Continue**.</span></span>

4. <span data-ttu-id="c9b8e-126">[アカウントを既にお持ちの場合] の下で **[サインイン]** を選びます。</span><span class="sxs-lookup"><span data-stu-id="c9b8e-126">Under Already have an account? select **Sign In**.</span></span>

5. <span data-ttu-id="c9b8e-127">次のページで Power BI のユーザー名とパスワードを入力し、[サインイン]を選びます。</span><span class="sxs-lookup"><span data-stu-id="c9b8e-127">On the next page, enter your Power BI user name and password and then select Sign In.</span></span>

6. <span data-ttu-id="c9b8e-128">Workspacename を指定して、ワークスペースをインストールします。</span><span class="sxs-lookup"><span data-stu-id="c9b8e-128">Install the workspace by providing the workspacename.</span></span>

7. <span data-ttu-id="c9b8e-129">インストールされているテンプレートアプリは、[アプリ] セクションで確認できます。</span><span class="sxs-lookup"><span data-stu-id="c9b8e-129">You can find the template apps installed under Apps Section.</span></span>

8. <span data-ttu-id="c9b8e-130">[アプリ] をクリックし、インストールされているアプリを選択します。</span><span class="sxs-lookup"><span data-stu-id="c9b8e-130">Click on Apps and choose the installed apps.</span></span>

9. <span data-ttu-id="c9b8e-131">[新しいアプリの開始] 画面が開きます。</span><span class="sxs-lookup"><span data-stu-id="c9b8e-131">Get Started with your new app screen opens.</span></span>

10. <span data-ttu-id="c9b8e-132">データに接続するには、[**接続**] をクリックします。</span><span class="sxs-lookup"><span data-stu-id="c9b8e-132">To connect to the data Click **Connect**.</span></span>

11. <span data-ttu-id="c9b8e-133">[ **Partner Center Analytics への接続**] ポップアップウィンドウで、[**認証方法**] が [ **oAuth2** ] に設定されていることを確認するか、表示されていない場合は一覧から**oAuth2**を選択します。</span><span class="sxs-lookup"><span data-stu-id="c9b8e-133">On the **Connect to Partner Center Analytics** pop-up window, verify that the **Authentication method** is set to **oAuth2** or select **oAuth2** from the list if it's not.</span></span> 

> [!NOTE]  
>  <span data-ttu-id="c9b8e-134">このウィンドウが表示されるまでに数分間かかることがあります。</span><span class="sxs-lookup"><span data-stu-id="c9b8e-134">This window may take a few minutes to appear.</span></span>

12. <span data-ttu-id="c9b8e-135">[ **Partner Center Analytics コネクタ**] ページで、会社の Azure AD テナントのグローバル管理者、管理エージェント、または課金管理者の資格情報を使用してサインインし、[**サインイン**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="c9b8e-135">On the **Partner Center Analytics Connector** page, sign in with global admin, admin agent, or billing admin credentials for your company's Azure AD tenant, and then select **Sign In**.</span></span>
 
13. <span data-ttu-id="c9b8e-136">アクセスするかどうかを尋ねられたら、**[同意する]** を選びます。</span><span class="sxs-lookup"><span data-stu-id="c9b8e-136">When prompted for access, select **Accept**.</span></span> 

<span data-ttu-id="c9b8e-137">パートナー センターの分析サービスが Power BI に接続されると、データの読み込みが開始します。</span><span class="sxs-lookup"><span data-stu-id="c9b8e-137">Once the Partner Center Analytics service is connected to Power BI, data will begin to load.</span></span> <span data-ttu-id="c9b8e-138">データ量によっては、この読み込みに最大 10 分間かかります。</span><span class="sxs-lookup"><span data-stu-id="c9b8e-138">Depending on the amount of data, this can take up to 10 minutes.</span></span> 

<span data-ttu-id="c9b8e-139">データの読み込みが完了すると、Power BI でパートナー センターの分析アプリのダッシュボードとレポートを使用できるようになります。</span><span class="sxs-lookup"><span data-stu-id="c9b8e-139">After the data finishes loading, you can start using the Partner Center Analytics app dashboard and reports in Power BI.</span></span>

## <a name="next-steps"></a><span data-ttu-id="c9b8e-140">次の手順</span><span class="sxs-lookup"><span data-stu-id="c9b8e-140">Next steps</span></span>

[<span data-ttu-id="c9b8e-141">Microsoft Power BI 用パートナー センター分析アプリでビジネス データを表示する</span><span class="sxs-lookup"><span data-stu-id="c9b8e-141">View your business data with the Partner Center Analytics app for Microsoft Power BI</span></span>](power-bi-app-for-direct-partners-use.md)
