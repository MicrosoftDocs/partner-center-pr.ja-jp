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
ms.openlocfilehash: 64467ec608c2ca87dbc2b7d5dfb02adb08f13c18
ms.sourcegitcommit: 0a6b1e6d845391539f54213efff00af4d23f028c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/14/2020
ms.locfileid: "86302329"
---
# <a name="install-and-preview-the-partner-center-analytics-app-for-microsoft-power-bi"></a><span data-ttu-id="f8e6c-103">Power BI 用パートナー センター分析アプリをインストールしてプレビューする</span><span class="sxs-lookup"><span data-stu-id="f8e6c-103">Install and preview the Partner Center Analytics app for Microsoft Power BI</span></span>

<span data-ttu-id="f8e6c-104">**適用対象**</span><span class="sxs-lookup"><span data-stu-id="f8e6c-104">**Applies to**</span></span>

- <span data-ttu-id="f8e6c-105">パートナー センター</span><span class="sxs-lookup"><span data-stu-id="f8e6c-105">Partner Center</span></span>

<span data-ttu-id="f8e6c-106">**適切なロール**</span><span class="sxs-lookup"><span data-stu-id="f8e6c-106">**Appropriate roles**</span></span>
-   <span data-ttu-id="f8e6c-107">グローバル管理者</span><span class="sxs-lookup"><span data-stu-id="f8e6c-107">Global admin</span></span>
-   <span data-ttu-id="f8e6c-108">ユーザー管理者</span><span class="sxs-lookup"><span data-stu-id="f8e6c-108">User admin</span></span>
-   <span data-ttu-id="f8e6c-109">販売代理店</span><span class="sxs-lookup"><span data-stu-id="f8e6c-109">Sales agent</span></span>
-   <span data-ttu-id="f8e6c-110">管理エージェント</span><span class="sxs-lookup"><span data-stu-id="f8e6c-110">Admin agent</span></span>

## <a name="before-you-begin"></a><span data-ttu-id="f8e6c-111">開始する前に</span><span class="sxs-lookup"><span data-stu-id="f8e6c-111">Before you begin</span></span>

<span data-ttu-id="f8e6c-112">使用可能な Power BI アプリの次の一覧から、自分のビジネスに最も関係のあるアプリケーションを選択します。</span><span class="sxs-lookup"><span data-stu-id="f8e6c-112">Select the application that is most relevant to your business from the following list of available Power BI apps:</span></span>
- [<span data-ttu-id="f8e6c-113">直接プロバイダー</span><span class="sxs-lookup"><span data-stu-id="f8e6c-113">Direct Provider</span></span>](https://appsource.microsoft.com/product/power-bi/partnercenteranalytics.direct_provider_partner_analytics)

- [<span data-ttu-id="f8e6c-114">間接プロバイダー</span><span class="sxs-lookup"><span data-stu-id="f8e6c-114">Indirect Provider</span></span>](https://appsource.microsoft.com/product/power-bi/partnercenteranalytics.indirect_provider_partner_analytics)

- [<span data-ttu-id="f8e6c-115">間接リセラー</span><span class="sxs-lookup"><span data-stu-id="f8e6c-115">Indirect Reseller</span></span>](https://appsource.microsoft.com/product/power-bi/partnercenteranalytics.indirect_reseller_partner_analytics)

<span data-ttu-id="f8e6c-116">パートナー センター分析アプリのプレビュー バージョンをインストールする前に、次の要件を満たしていることを確認してください。</span><span class="sxs-lookup"><span data-stu-id="f8e6c-116">Before you install the Partner Center Analytics app preview version, be sure that you meet the following requirements.</span></span>

- <span data-ttu-id="f8e6c-117">自分のビジネスに合った Power BI アプリを選択している。</span><span class="sxs-lookup"><span data-stu-id="f8e6c-117">You pick the correct Power BI app for your business.</span></span>

- <span data-ttu-id="f8e6c-118">Power BI pro ライセンスを持っている。</span><span class="sxs-lookup"><span data-stu-id="f8e6c-118">You have a Power BI pro license.</span></span>

- <span data-ttu-id="f8e6c-119">テナントにテンプレートアプリをインストールするためのアクセス許可があります。</span><span class="sxs-lookup"><span data-stu-id="f8e6c-119">You have permissions to install template apps on your tenant.</span></span>

- <span data-ttu-id="f8e6c-120">Power BI にログインできる。</span><span class="sxs-lookup"><span data-stu-id="f8e6c-120">You can sign in to Power BI.</span></span>

- <span data-ttu-id="f8e6c-121">[会社の Azure Active Directory (Azure AD) テナント](azure-active-directory-tenants-and-partner-center.md)に、グローバル管理者、管理エージェント、または課金管理者としてサインインできます。</span><span class="sxs-lookup"><span data-stu-id="f8e6c-121">You can sign in as a global admin, admin agent, or billing admin to [your company's Azure Active Directory (Azure AD) tenant](azure-active-directory-tenants-and-partner-center.md).</span></span>

## <a name="to-install-the-app"></a><span data-ttu-id="f8e6c-122">アプリをインストールするには</span><span class="sxs-lookup"><span data-stu-id="f8e6c-122">To install the app</span></span>

1. <span data-ttu-id="f8e6c-123">上記のセクションで、指定されたアプリソースリンク (Direct Provider/間接プロバイダ/間接リセラー) をクリックします。</span><span class="sxs-lookup"><span data-stu-id="f8e6c-123">Click on the app source link given (Direct Provider/Indirect Provider/Indirect Reseller) in the above section.</span></span>

2. <span data-ttu-id="f8e6c-124">[**今すぐ入手**する] をクリックします。</span><span class="sxs-lookup"><span data-stu-id="f8e6c-124">Click on **GET IT NOW**.</span></span> 

3. <span data-ttu-id="f8e6c-125">[**続行**] をクリックして使用条件に同意します。</span><span class="sxs-lookup"><span data-stu-id="f8e6c-125">Agree terms and conditions by clicking **Continue**.</span></span>

4. <span data-ttu-id="f8e6c-126">[アカウントを既にお持ちの場合] の下で **[サインイン]** を選びます。</span><span class="sxs-lookup"><span data-stu-id="f8e6c-126">Under Already have an account? select **Sign In**.</span></span>

5. <span data-ttu-id="f8e6c-127">次のページで Power BI のユーザー名とパスワードを入力し、[サインイン]を選びます。</span><span class="sxs-lookup"><span data-stu-id="f8e6c-127">On the next page, enter your Power BI user name and password and then select Sign In.</span></span>

6. <span data-ttu-id="f8e6c-128">ワークスペース名を指定して、ワークスペースをインストールします。</span><span class="sxs-lookup"><span data-stu-id="f8e6c-128">Install the workspace by providing the workspace name.</span></span>

7. <span data-ttu-id="f8e6c-129">インストールされているテンプレートアプリは、[アプリ] セクションで確認できます。</span><span class="sxs-lookup"><span data-stu-id="f8e6c-129">You can find the template apps installed under Apps Section.</span></span>

8. <span data-ttu-id="f8e6c-130">[アプリ] をクリックし、インストールされているアプリを選択します。</span><span class="sxs-lookup"><span data-stu-id="f8e6c-130">Click on Apps and choose the installed apps.</span></span>

9. <span data-ttu-id="f8e6c-131">[新しいアプリの開始] 画面が開きます。</span><span class="sxs-lookup"><span data-stu-id="f8e6c-131">Get Started with your new app screen opens.</span></span>

10. <span data-ttu-id="f8e6c-132">データに接続するには、[**接続**] をクリックします。</span><span class="sxs-lookup"><span data-stu-id="f8e6c-132">To connect to the data Click **Connect**.</span></span>

11. <span data-ttu-id="f8e6c-133">[ **Partner Center Analytics への接続**] ポップアップウィンドウで、[**認証方法**] が [ **oAuth2** ] に設定されていることを確認するか、表示されていない場合は一覧から**oAuth2**を選択します。</span><span class="sxs-lookup"><span data-stu-id="f8e6c-133">On the **Connect to Partner Center Analytics** pop-up window, verify that the **Authentication method** is set to **oAuth2** or select **oAuth2** from the list if it's not.</span></span> 

> [!NOTE]  
>  <span data-ttu-id="f8e6c-134">このウィンドウが表示されるまでに数分間かかることがあります。</span><span class="sxs-lookup"><span data-stu-id="f8e6c-134">This window may take a few minutes to appear.</span></span>

12. <span data-ttu-id="f8e6c-135">[ **Partner Center Analytics コネクタ**] ページで、会社の Azure AD テナントのグローバル管理者、管理エージェント、または課金管理者の資格情報を使用してサインインし、[**サインイン**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="f8e6c-135">On the **Partner Center Analytics Connector** page, sign in with global admin, admin agent, or billing admin credentials for your company's Azure AD tenant, and then select **Sign In**.</span></span>
 
13. <span data-ttu-id="f8e6c-136">アクセスするかどうかを尋ねられたら、**[同意する]** を選びます。</span><span class="sxs-lookup"><span data-stu-id="f8e6c-136">When prompted for access, select **Accept**.</span></span> 

<span data-ttu-id="f8e6c-137">パートナー センターの分析サービスが Power BI に接続されると、データの読み込みが開始します。</span><span class="sxs-lookup"><span data-stu-id="f8e6c-137">Once the Partner Center Analytics service is connected to Power BI, data will begin to load.</span></span> <span data-ttu-id="f8e6c-138">データ量によっては、この読み込みに最大 10 分間かかります。</span><span class="sxs-lookup"><span data-stu-id="f8e6c-138">Depending on the amount of data, this can take up to 10 minutes.</span></span> 

<span data-ttu-id="f8e6c-139">データの読み込みが完了すると、Power BI でパートナー センターの分析アプリのダッシュボードとレポートを使用できるようになります。</span><span class="sxs-lookup"><span data-stu-id="f8e6c-139">After the data finishes loading, you can start using the Partner Center Analytics app dashboard and reports in Power BI.</span></span>

## <a name="next-steps"></a><span data-ttu-id="f8e6c-140">次の手順</span><span class="sxs-lookup"><span data-stu-id="f8e6c-140">Next steps</span></span>

[<span data-ttu-id="f8e6c-141">Microsoft Power BI 用パートナー センター分析アプリでビジネス データを表示する</span><span class="sxs-lookup"><span data-stu-id="f8e6c-141">View your business data with the Partner Center Analytics app for Microsoft Power BI</span></span>](power-bi-app-for-direct-partners-use.md)
