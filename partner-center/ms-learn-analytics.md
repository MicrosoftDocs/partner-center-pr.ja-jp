---
title: パートナーセンターの Insights Microsoft Learn analytics
ms.topic: article
ms.date: 08/13/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 個々のトレーニング、完成したモジュール、完成したラーニングパスなどのデータを活用して、会社の学習器を追跡します。
author: shganesh-dev
ms.author: shganesh
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 5b9a0ea8c4eefee1a87b9ccd626b1f2864234521
ms.sourcegitcommit: f24089cd27b1de6ecf6ddbefb6cbb2d340e144de
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/01/2021
ms.locfileid: "106132317"
---
# <a name="the-microsoft-learn-analytics-report-shows-the-status-of-learners-in-your-company"></a><span data-ttu-id="c19ea-103">Microsoft Learn 分析レポートに社内の学習者の状態が表示されます</span><span class="sxs-lookup"><span data-stu-id="c19ea-103">The Microsoft Learn analytics report shows the status of learners in your company</span></span>

<span data-ttu-id="c19ea-104">**適切なロール**</span><span class="sxs-lookup"><span data-stu-id="c19ea-104">**Appropriate roles**</span></span>

- <span data-ttu-id="c19ea-105">グローバル管理者</span><span class="sxs-lookup"><span data-stu-id="c19ea-105">Global admin</span></span>
- <span data-ttu-id="c19ea-106">MPN パートナー管理者</span><span class="sxs-lookup"><span data-stu-id="c19ea-106">MPN partner admin</span></span>

<span data-ttu-id="c19ea-107">Microsoft Learn レポートには、完了したモジュールとその学習パスを含む、会社の学習器に関する情報が表示されます。</span><span class="sxs-lookup"><span data-stu-id="c19ea-107">The Microsoft Learn report provides you with information on the learners in your company including the modules they've completed and the learning paths they are on.</span></span> <span data-ttu-id="c19ea-108">このレポートには、個々の学習器の状態が表示されます。</span><span class="sxs-lookup"><span data-stu-id="c19ea-108">The report displays the status of each individual learner.</span></span> <span data-ttu-id="c19ea-109">会社のグローバル管理者と MPN admin は、データを表示できます。</span><span class="sxs-lookup"><span data-stu-id="c19ea-109">The global admin and the MPN admin for your company can view the data.</span></span>

## <a name="how-to-read-the-report"></a><span data-ttu-id="c19ea-110">レポートを読み取る方法</span><span class="sxs-lookup"><span data-stu-id="c19ea-110">How to read the report</span></span>

### <a name="summary-charts"></a><span data-ttu-id="c19ea-111">概要グラフ</span><span class="sxs-lookup"><span data-stu-id="c19ea-111">Summary charts</span></span>

<span data-ttu-id="c19ea-112">これらのグラフは、トレーニングされた個人、モジュールの完了、およびラーニングパスの数と月単位の累積傾向をまとめたものです。</span><span class="sxs-lookup"><span data-stu-id="c19ea-112">These charts summarize count and monthly cumulative trends for trained individuals, module completions, and learning paths.</span></span>


<span data-ttu-id="c19ea-113">トレーニングされた **個人数**: 選択した日付範囲内に少なくとも1つのモジュールを完了したすべての個別の学習器の数</span><span class="sxs-lookup"><span data-stu-id="c19ea-113">**Trained individuals count**: A count of all distinct learners who have completed at least one module during the selected date range</span></span> 

<span data-ttu-id="c19ea-114">トレーニングされた **個人の傾向ミニグラフ**: アクティブな学習器の月単位の累積数</span><span class="sxs-lookup"><span data-stu-id="c19ea-114">**Trained individuals trend mini chart**: Month over month cumulative count of the active learners</span></span> 

<span data-ttu-id="c19ea-115">**モジュール完了回数**: 選択した日付範囲におけるパートナー企業の学習器によるモジュール入力候補の数。</span><span class="sxs-lookup"><span data-stu-id="c19ea-115">**Module completions count**: Count of Module completions by the learners in the partner's company during the selected date range.</span></span>
<span data-ttu-id="c19ea-116">たとえば、"モジュール 1" が15人のユーザーによって完了され、"モジュール 2" が同じ15人のユーザーによって完了した場合、モジュールの入力候補カウントは30になります。</span><span class="sxs-lookup"><span data-stu-id="c19ea-116">For example,  if “Module 1" is completed by 15 individuals, and the “Module 2" has been completed by the same 15 individuals, the module completions count will be 30.</span></span> <span data-ttu-id="c19ea-117">モジュールの完了日は、選択した日付の範囲内である必要があります。</span><span class="sxs-lookup"><span data-stu-id="c19ea-117">The module completion date should fall in the date range selected.</span></span>

<span data-ttu-id="c19ea-118">**モジュール入力の傾向ミニグラフ**: モジュールが完了した月の累積カウント</span><span class="sxs-lookup"><span data-stu-id="c19ea-118">**Module completions trend mini chart**: Month over month cumulative count of the module completions</span></span> 

<span data-ttu-id="c19ea-119">**ラーニングパスの入力候補数**: 選択した日付範囲におけるパートナー企業の学習器によるラーニングパスの入力候補の数。</span><span class="sxs-lookup"><span data-stu-id="c19ea-119">**Learning path completions count**: Count of Learning path completions by the learners in the partner's company during the selected date range.</span></span>
<span data-ttu-id="c19ea-120">たとえば、ラーニングパス "Path 1" が20人の個人によって完了し、ラーニングパス "path 2" が同じ20人のユーザーによって完了された場合、ラーニングパスの完了数は40になります。</span><span class="sxs-lookup"><span data-stu-id="c19ea-120">For example, if Learning Path “Path 1" is completed by 20 individuals, and the Learning Path “path 2" has been completed by the same 20 individuals, the Learning Path completion count will be 40.</span></span> <span data-ttu-id="c19ea-121">ラーニングパスの完了日は、選択した日付範囲内である必要があります。</span><span class="sxs-lookup"><span data-stu-id="c19ea-121">The Learning path completion date should fall within the selected  date range.</span></span>

<span data-ttu-id="c19ea-122">**ラーニングパス入力候補傾向ミニグラフ**: 学習パス入力候補の月単位の累積数</span><span class="sxs-lookup"><span data-stu-id="c19ea-122">**Learning path completions trend mini chart**: Month over month cumulative count of the learning path completions</span></span> 

### <a name="trained-individuals-monthly-trend"></a><span data-ttu-id="c19ea-123">トレーニングを受けた個人の月間傾向</span><span class="sxs-lookup"><span data-stu-id="c19ea-123">Trained individuals' monthly trend</span></span>

<span data-ttu-id="c19ea-124">このデータは、その月に最初にモジュールを完了した会社のユーザーの傾向です。</span><span class="sxs-lookup"><span data-stu-id="c19ea-124">This data is the trend of your company's users who have completed a module for the first time in that month.</span></span> 

<span data-ttu-id="c19ea-125">**X 軸** は、選択された時間フィルターの月です。</span><span class="sxs-lookup"><span data-stu-id="c19ea-125">**X-Axis** is month for the time filter selected.</span></span> 

<span data-ttu-id="c19ea-126">**Y 軸** は、その月の間に (モジュールの初回完了を) 登録したアクティブな学習器の数です。</span><span class="sxs-lookup"><span data-stu-id="c19ea-126">**Y-Axis** is count of active learners who have registered (first-time completion of a module) during that month.</span></span> <span data-ttu-id="c19ea-127">これは累積的ではありません。</span><span class="sxs-lookup"><span data-stu-id="c19ea-127">This is not cumulative.</span></span>

### <a name="module-completions-monthly-trend"></a><span data-ttu-id="c19ea-128">モジュール入力候補の月単位の傾向</span><span class="sxs-lookup"><span data-stu-id="c19ea-128">Module completions monthly trend</span></span>

<span data-ttu-id="c19ea-129">このデータは、その月のすべての会社のユーザーによって完了したモジュールの傾向を示します。</span><span class="sxs-lookup"><span data-stu-id="c19ea-129">This data is the trend of modules completed by all your company's users during that month.</span></span> <span data-ttu-id="c19ea-130">(累積ではない)</span><span class="sxs-lookup"><span data-stu-id="c19ea-130">(not cumulative)</span></span> 

<span data-ttu-id="c19ea-131">**X 軸** は、選択された時間フィルターの月です。</span><span class="sxs-lookup"><span data-stu-id="c19ea-131">**X-Axis** is month for the time filter selected.</span></span> 

<span data-ttu-id="c19ea-132">**Y 軸** は、その月のモジュールの完了のカウントです。</span><span class="sxs-lookup"><span data-stu-id="c19ea-132">**Y-Axis** is count of the module completions during that month.</span></span> <span data-ttu-id="c19ea-133">これは累積的ではありません。</span><span class="sxs-lookup"><span data-stu-id="c19ea-133">This is not cumulative.</span></span>

### <a name="learning-path-completions-monthly-trend"></a><span data-ttu-id="c19ea-134">ラーニングパス入力候補の月単位の傾向</span><span class="sxs-lookup"><span data-stu-id="c19ea-134">Learning path completions monthly trend</span></span>

<span data-ttu-id="c19ea-135">このデータは、その月に会社のユーザーが行ったラーニングパスの傾向を示しています。</span><span class="sxs-lookup"><span data-stu-id="c19ea-135">This data is the trend of learning paths completed by your company's users during that month.</span></span> <span data-ttu-id="c19ea-136">(累積ではない)</span><span class="sxs-lookup"><span data-stu-id="c19ea-136">(not cumulative)</span></span> 

<span data-ttu-id="c19ea-137">**X 軸** は、選択された時間フィルターの月です。</span><span class="sxs-lookup"><span data-stu-id="c19ea-137">**X-Axis** is month for the time filter selected.</span></span> 

<span data-ttu-id="c19ea-138">**Y 軸** は、その月のモジュールの完了数です。</span><span class="sxs-lookup"><span data-stu-id="c19ea-138">**Y-Axis** is count of module completions in that month.</span></span> <span data-ttu-id="c19ea-139">これは累積的ではありません。</span><span class="sxs-lookup"><span data-stu-id="c19ea-139">This is not cumulative.</span></span>

### <a name="learning-path-completion-tabs"></a><span data-ttu-id="c19ea-140">ラーニングパスの入力候補タブ</span><span class="sxs-lookup"><span data-stu-id="c19ea-140">Learning path completion tabs</span></span> 

<span data-ttu-id="c19ea-141">**[モジュール] タブ**</span><span class="sxs-lookup"><span data-stu-id="c19ea-141">**Module tab**</span></span>

<span data-ttu-id="c19ea-142">このタブには、会社で完了したモジュール名の上位5つの内訳が表示されます。モジュールが関連付けられている製品。モジュールに関連するユーザーロール。</span><span class="sxs-lookup"><span data-stu-id="c19ea-142">This tab includes breakdown of modules completed in your company by top five module names; the product to which the module is associated; and the user role pertinent to the module.</span></span>  

- <span data-ttu-id="c19ea-143">モジュール入力候補ドーナツグラフ: モジュール名によってモジュールの完了 (概要セクションに表示されるカウント) の内訳。</span><span class="sxs-lookup"><span data-stu-id="c19ea-143">Module completions donut chart: breakdown of the module completions (count displayed in the summary section) by the module names.</span></span>

<span data-ttu-id="c19ea-144">グラフの中央に表示される数値は、完了したモジュールの総数です</span><span class="sxs-lookup"><span data-stu-id="c19ea-144">Number displayed in the center of the chart is the total modules completed</span></span>

- <span data-ttu-id="c19ea-145">ロール別の入力候補: モジュールの役割によってモジュールの完了が分類されます。</span><span class="sxs-lookup"><span data-stu-id="c19ea-145">Completions by role: breakdown of the module completions by the role of the module.</span></span> <span data-ttu-id="c19ea-146">モジュールが複数のロールに関連付けられている場合は、各ロールがモジュールの完了数に追加されます。</span><span class="sxs-lookup"><span data-stu-id="c19ea-146">If a module is associated with multiple roles, then each of the roles is added to the count of module completions.</span></span>

<span data-ttu-id="c19ea-147">グラフの中央に表示される数値は、モジュールの完了に関する個別のロールの数です。</span><span class="sxs-lookup"><span data-stu-id="c19ea-147">Number displayed in the center of the chart is the number of distinct roles for the module completions.</span></span> 

- <span data-ttu-id="c19ea-148">製品別の入力候補: モジュールがマップされている製品によるモジュール入力候補の内訳。</span><span class="sxs-lookup"><span data-stu-id="c19ea-148">Completions by product: breakdown of the module completions by the product the module is mapped to.</span></span> <span data-ttu-id="c19ea-149">モジュールが複数の製品に関連付けられている場合は、各製品がモジュールの入力候補の数に追加されます。</span><span class="sxs-lookup"><span data-stu-id="c19ea-149">If a module is associated with multiple products, then each of the products is added to the count of module completions.</span></span>    

<span data-ttu-id="c19ea-150">グラフの中央に表示される数値は、モジュールの完了に関する個別の製品の数です。</span><span class="sxs-lookup"><span data-stu-id="c19ea-150">Number displayed in the center of the chart is the number of distinct products for the module completions.</span></span>  

<span data-ttu-id="c19ea-151">**[ラーニングパス] タブ**</span><span class="sxs-lookup"><span data-stu-id="c19ea-151">**Learning path tab**</span></span>   

<span data-ttu-id="c19ea-152">このタブには、会社で完了したラーニングパスの内訳が5つのモジュール名で表示されます。ラーニングパスのマップ先の製品。また、このラーニングパスに関連するロールがあります。</span><span class="sxs-lookup"><span data-stu-id="c19ea-152">This tab includes a breakdown of learning paths completed in your company by top five module names; the product the learning path is mapped to; and the role pertinent to this learning path.</span></span>  

- <span data-ttu-id="c19ea-153">ラーニングパスの入力候補ドーナツグラフ: ラーニングパスの入力候補 ([概要] セクションに表示されるカウント) の内訳を名前別に表示します。</span><span class="sxs-lookup"><span data-stu-id="c19ea-153">Learning paths completions donut chart: breakdown of the Learning path completions (count displayed in the summary section) by name.</span></span>

- <span data-ttu-id="c19ea-154">ロール別の入力候補 \*: ロールによって完了したラーニングパスの内訳。</span><span class="sxs-lookup"><span data-stu-id="c19ea-154">Completions by role\*: breakdown of the learning paths completions by the role.</span></span> <span data-ttu-id="c19ea-155">モジュールが複数のロールに関連付けられている場合は、各ロールがモジュールの完了数に追加されます。</span><span class="sxs-lookup"><span data-stu-id="c19ea-155">If a module is associated with multiple roles, then each of the roles is added to the count of module completions.</span></span>

- <span data-ttu-id="c19ea-156">製品別の入力候補: ラーニングパスがマップされている製品によって入力されたラーニングパスの内訳。</span><span class="sxs-lookup"><span data-stu-id="c19ea-156">Completions by product: breakdown of the learning paths completions by the Product to which the learning path is mapped.</span></span> <span data-ttu-id="c19ea-157">モジュールが複数の製品に関連付けられている場合は、各製品がモジュールの入力候補の数に追加されます。</span><span class="sxs-lookup"><span data-stu-id="c19ea-157">If a module is associated with multiple products, then each of the products is added to the count of module completions.</span></span>

### <a name="completions-by-learning-individuals"></a><span data-ttu-id="c19ea-158">個人を学習した後の入力候補</span><span class="sxs-lookup"><span data-stu-id="c19ea-158">Completions by learning individuals</span></span>

<span data-ttu-id="c19ea-159">ここには、会社のトレーニング済みユーザーと、完成したモジュールとラーニングパスの詳細が表示されます。</span><span class="sxs-lookup"><span data-stu-id="c19ea-159">This lists the trained users in your company and details of their completed modules and learning paths.</span></span>

<span data-ttu-id="c19ea-160">Microsoft Learn は、ユーザーオブジェクト ID を使用して学習器を識別します。</span><span class="sxs-lookup"><span data-stu-id="c19ea-160">Microsoft Learn identifies learners with a User Object ID.</span></span> <span data-ttu-id="c19ea-161">[ **モジュール] タブ** では、すべての学習器が、完了したモジュールによって並べ替えられます。</span><span class="sxs-lookup"><span data-stu-id="c19ea-161">Under the **Modules tab**, all learners are sorted by the modules completed.</span></span> <span data-ttu-id="c19ea-162">これらは、Microsoft Learn ユーザー名、オブジェクト ID、およびモジュール数と共に表示されます。</span><span class="sxs-lookup"><span data-stu-id="c19ea-162">They are displayed with their Microsoft Learn username, Object ID, and modules count.</span></span> <span data-ttu-id="c19ea-163">ユーザー名を使用して検索できます。</span><span class="sxs-lookup"><span data-stu-id="c19ea-163">You can search using username.</span></span> 

<span data-ttu-id="c19ea-164">[ **ラーニングパス] タブ** の下に、ラーニングパスの完了によって並べ替えられたすべての学習器が、学習者の表示名、オブジェクト ID、およびモジュール数と共に表示されます。</span><span class="sxs-lookup"><span data-stu-id="c19ea-164">Under the **Learning paths tab** all learners sorted by learning paths completed, are displayed with the learner display name, Object ID, and module count.</span></span>

<span data-ttu-id="c19ea-165">ユーザーオブジェクト ID を使用して学習器の詳細を取得するには、次のようにします。</span><span class="sxs-lookup"><span data-stu-id="c19ea-165">To get a learner's details using the User Object ID:</span></span> 

1. <span data-ttu-id="c19ea-166">[Graph Explorer](https://developer.microsoft.com/graph/graph-explorer )にサインインします。</span><span class="sxs-lookup"><span data-stu-id="c19ea-166">Sign in to [Graph Explorer](https://developer.microsoft.com/graph/graph-explorer ).</span></span> <span data-ttu-id="c19ea-167">(会社の Azure AD テナントのグローバル管理者である必要があります)。</span><span class="sxs-lookup"><span data-stu-id="c19ea-167">(You must be the global admin of your company's Azure AD tenant.)</span></span>

2. <span data-ttu-id="c19ea-168">Graph Explorer で [強調表示](https://graph.microsoft.com/v1.0/users/a9633ad7-c8dc-4587-b119-0bc286b0711f) されている領域にユーザーオブジェクト ID をコピーします。</span><span class="sxs-lookup"><span data-stu-id="c19ea-168">Copy the user object ID to the [area highlighted](https://graph.microsoft.com/v1.0/users/a9633ad7-c8dc-4587-b119-0bc286b0711f) in Graph Explorer.</span></span> 

## <a name="faq"></a><span data-ttu-id="c19ea-169">よく寄せられる質問</span><span class="sxs-lookup"><span data-stu-id="c19ea-169">FAQ</span></span>

1. <span data-ttu-id="c19ea-170">会社の学習の詳細が表示されません。</span><span class="sxs-lookup"><span data-stu-id="c19ea-170">I am unable to see my company's Learning details.</span></span>

<span data-ttu-id="c19ea-171">このレポートは、パートナーセンターでアカウントを所有しているパートナーが利用できます。</span><span class="sxs-lookup"><span data-stu-id="c19ea-171">This report is available to partners who have an account in Partner Center.</span></span> <span data-ttu-id="c19ea-172">パートナーメンバーシップセンターにまだ参加していない場合は、このレポートを表示することはできません。</span><span class="sxs-lookup"><span data-stu-id="c19ea-172">If you are still in Partner Membership Center, you'll not be able to see this report.</span></span>

2.  <span data-ttu-id="c19ea-173">社内のだれがこのレポートを表示できますか。</span><span class="sxs-lookup"><span data-stu-id="c19ea-173">Who in our company can view this report?</span></span> 

<span data-ttu-id="c19ea-174">全体管理者と MPN 管理者は、レポートを表示できます。</span><span class="sxs-lookup"><span data-stu-id="c19ea-174">The global admin and the MPN admin can view the report.</span></span>

3. <span data-ttu-id="c19ea-175">すべてのユーザー Microsoft Learn アカウントをパートナーセンターアカウントに関連付けるにはどうすればよいですか。</span><span class="sxs-lookup"><span data-stu-id="c19ea-175">How can I make sure all our users associate their Microsoft Learn accounts with their Partner Center account?</span></span>

<span data-ttu-id="c19ea-176">全体管理者が新しいユーザーを追加した後、そのユーザーは **自分のプロファイル** にアクセスして Microsoft Learn アカウントを関連付ける必要があります。</span><span class="sxs-lookup"><span data-stu-id="c19ea-176">After the global admin adds a new user, that user needs to go to their **My profile** to associate their Microsoft Learn account.</span></span>

- <span data-ttu-id="c19ea-177">ダッシュボードの右上隅にある **自分のアカウント** アイコンを選択し、[ **マイプロファイル**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="c19ea-177">Select the **Your account** icon in the right corner of the dashboard, and then select **My profile**.</span></span> 

-  <span data-ttu-id="c19ea-178">**ラーニング** では、ユーザーは自分の Microsoft learning アカウントに関連付けて、パートナーの大学に Microsoft アカウントを接続することができます。</span><span class="sxs-lookup"><span data-stu-id="c19ea-178">Under **Your learning** a user will be able to associate their Microsoft Learning account and connect their Microsoft account to Partner University.</span></span>

3. <span data-ttu-id="c19ea-179">このレポートで MSA アカウントを使用して Microsoft Learn にサインインしているすべての会社のユーザーを表示できますか。</span><span class="sxs-lookup"><span data-stu-id="c19ea-179">Can I see all the company's users who sign into Microsoft Learn with an MSA account in this report?</span></span>

<span data-ttu-id="c19ea-180">現時点で最適な方法は、これらのユーザーを Azure AD テナントに追加し、パートナーセンターに追加して、パートナーセンターで **自分のプロファイル** を使用して Microsoft Learn アカウントを関連付けることができるようにすることです。</span><span class="sxs-lookup"><span data-stu-id="c19ea-180">Currently, the best way to do this is to add these users to your Azure AD tenant and then add them to Partner Center so that they can associate their Microsoft Learn account through **My profile** in Partner Center.</span></span> 

<span data-ttu-id="c19ea-181">MSA アカウントのみをトレーニングに使用するユーザーについては、Microsoft Learn チームが、仕事用の電子メールを Microsoft Learn プロファイルに関連付けることができるようになります。</span><span class="sxs-lookup"><span data-stu-id="c19ea-181">For users who only use their MSA account for training, in the near future, the Microsoft Learn team will enable the ability for them to associate their work email to their Microsoft Learn profile.</span></span> 

## <a name="next-steps"></a><span data-ttu-id="c19ea-182">次のステップ</span><span class="sxs-lookup"><span data-stu-id="c19ea-182">Next steps</span></span>

<span data-ttu-id="c19ea-183">詳細なレポートについては、「 [Partner Center Insights](partner-center-insights.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="c19ea-183">For more reports, see [Partner Center Insights](partner-center-insights.md).</span></span>

>[!NOTE] 
> <span data-ttu-id="c19ea-184">このレポートを作成する生データは、Insights ダッシュボードの [レポートのダウンロード] セクションからダウンロードできます。</span><span class="sxs-lookup"><span data-stu-id="c19ea-184">You can download the raw data powering this report from the Download Reports section in the Insights dashboard.</span></span> [<span data-ttu-id="c19ea-185">詳細情報</span><span class="sxs-lookup"><span data-stu-id="c19ea-185">Learn More</span></span>](pci-download-reports.md) 