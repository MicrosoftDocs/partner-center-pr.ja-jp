---
title: パートナー センター Insights Microsoft Learn分析
ms.topic: article
ms.date: 08/13/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 個々のトレーニング、完了したモジュール、完了したラーニング パスなどについてのデータを活用して、会社の学習者を追跡します。
author: shganesh-dev
ms.author: shganesh
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 132583352e1697a2f9dfa624eb9532692be6d734
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/19/2021
ms.locfileid: "110152632"
---
# <a name="the-microsoft-learn-analytics-report-shows-the-status-of-learners-in-your-company"></a>Microsoft Learn 分析レポートに社内の学習者の状態が表示されます

**適切なロール**: グローバル管理者|MPN パートナー管理者

このMicrosoft Learnレポートには、完了したモジュールや学習パスなど、会社の学習者に関する情報が表示されます。 レポートには、個々の学習者の状態が表示されます。 会社のグローバル管理者と MPN 管理者は、データを表示できます。

## <a name="how-to-read-the-report"></a>レポートを読み取る方法

### <a name="summary-charts"></a>概要グラフ

これらのグラフは、トレーニングされた個人、モジュールの完了、ラーニング パスの数と毎月の累積傾向をまとめたものです。


**トレーニングされた個人数**: 選択した日付範囲内に少なくとも 1 つのモジュールを完了した、すべての個別の学習者の数 

**トレーニングされた個人の傾向のミニ グラフ**: アクティブな学習者の月累計数 

**モジュールの入力完了数**: 選択した日付範囲内のパートナーの会社の学習者によるモジュール入力完了の数。
たとえば、"モジュール 1" が 15 人の個人によって完了し、"モジュール 2" が同じ 15 人の個人によって完了した場合、モジュールの完了数は 30 です。 モジュールの完了日は、選択した日付範囲に入る必要があります。

**モジュールの完了傾向のミニ グラフ**: モジュール完了の月累計数 

**ラーニング パスの入力完了数**: 選択した日付範囲内のパートナーの会社の学習者によるラーニング パス入力の数。
たとえば、ラーニング パス "パス 1" が 20 人の個人によって完了し、ラーニング パス "パス 2" が同じ 20 人の個人によって完了した場合、ラーニング パスの完了数は 40 です。 ラーニング パスの完了日は、選択した日付範囲内に入る必要があります。

**ラーニング パスの完了傾向のミニ グラフ**: ラーニング パスの完了の月累計数 

### <a name="trained-individuals-monthly-trend"></a>トレーニングされた個人の月次傾向

このデータは、その月に最初にモジュールを完了した会社のユーザーの傾向です。 

**X 軸** は、選択された時間フィルターの月です。 

**Y 軸** は、その月の間に (モジュールの初回完了を) 登録したアクティブな学習器の数です。 これは累積的ではありません。

### <a name="module-completions-monthly-trend"></a>モジュール入力候補の月単位の傾向

このデータは、その月のすべての会社のユーザーによって完了したモジュールの傾向を示します。 (累積ではない) 

**X 軸** は、選択された時間フィルターの月です。 

**Y 軸** は、その月のモジュールの完了のカウントです。 これは累積的ではありません。

### <a name="learning-path-completions-monthly-trend"></a>ラーニングパス入力候補の月単位の傾向

このデータは、その月に会社のユーザーが行ったラーニングパスの傾向を示しています。 (累積ではない) 

**X 軸** は、選択された時間フィルターの月です。 

**Y 軸** は、その月のモジュールの完了数です。 これは累積的ではありません。

### <a name="learning-path-completion-tabs"></a>ラーニングパスの入力候補タブ 

**[モジュール] タブ**

このタブには、会社で完了したモジュール名の上位5つの内訳が表示されます。モジュールが関連付けられている製品。モジュールに関連するユーザーロール。  

- モジュール入力候補ドーナツグラフ: モジュール名によってモジュールの完了 (概要セクションに表示されるカウント) の内訳。

グラフの中央に表示される数値は、完了したモジュールの合計です

- ロール別の完了: モジュールのロール別のモジュール完了の内訳。 モジュールが複数のロールに関連付けられている場合は、各ロールがモジュール完了の数に追加されます。

グラフの中央に表示される数値は、モジュールの完了に対する個別のロールの数です。 

- 製品別の完了: モジュールがマップされている製品別のモジュール完了の内訳。 モジュールが複数の製品に関連付けられている場合は、各製品がモジュール完了の数に追加されます。    

グラフの中央に表示される数値は、モジュールの完了に対する個別の製品の数です。  

**[ラーニング パス] タブ**   

このタブには、上位 5 つのモジュール名で会社で完了したラーニング パスの内訳が含まれます。ラーニング パスがマップされている製品。このラーニング パスに関連する役割。  

- ラーニング パスの入力補完ドーナツ グラフ: 名前別のラーニング パスの入力完了数 (概要セクションに表示されるカウント) の内訳。

- [ロール別の完了] *: ロール別のラーニング パスの完了の内訳。 モジュールが複数のロールに関連付けられている場合は、各ロールがモジュール完了の数に追加されます。

- 製品別の完了: ラーニング パスがマップされている製品別のラーニング パスの完了の内訳。 モジュールが複数の製品に関連付けられている場合は、各製品がモジュール完了の数に追加されます。

### <a name="completions-by-learning-individuals"></a>個人の学習による完了

これにより、会社のトレーニング済みユーザーと、完了したモジュールとラーニング パスの詳細が一覧表示されます。

Microsoft Learnユーザー オブジェクト ID を持つ学習者を識別します。 [モジュール **] タブでは**、すべての学習器が完了したモジュールで並べ替えされます。 ユーザー名、オブジェクト ID、Microsoft Learn数を指定して表示されます。 ユーザー名を使用して検索できます。 

[ **ラーニングパス] タブ** の下に、ラーニングパスの完了によって並べ替えられたすべての学習器が、学習者の表示名、オブジェクト ID、およびモジュール数と共に表示されます。

ユーザーオブジェクト ID を使用して学習器の詳細を取得するには、次のようにします。 

1. [Graph Explorer](https://developer.microsoft.com/graph/graph-explorer )にサインインします。 (会社の Azure AD テナントのグローバル管理者である必要があります)。

2. Graph Explorer で [強調表示](https://graph.microsoft.com/v1.0/users/a9633ad7-c8dc-4587-b119-0bc286b0711f) されている領域にユーザーオブジェクト ID をコピーします。 

## <a name="faq"></a>よく寄せられる質問

1. 会社の学習の詳細が表示されません。

このレポートは、パートナーセンターでアカウントを所有しているパートナーが利用できます。 パートナーメンバーシップセンターにまだ参加していない場合は、このレポートを表示することはできません。

2.  社内のだれがこのレポートを表示できますか。 

全体管理者と MPN 管理者は、レポートを表示できます。

3. すべてのユーザー Microsoft Learn アカウントをパートナーセンターアカウントに関連付けるにはどうすればよいですか。

全体管理者が新しいユーザーを追加した後、そのユーザーは **自分のプロファイル** にアクセスして Microsoft Learn アカウントを関連付ける必要があります。

- ダッシュボードの右上隅にある **自分のアカウント** アイコンを選択し、[ **マイプロファイル**] を選択します。 

-  **ラーニング** では、ユーザーは自分の Microsoft learning アカウントに関連付けて、パートナーの大学に Microsoft アカウントを接続することができます。

3. このレポートで MSA アカウントを使用して Microsoft Learn にサインインしているすべての会社のユーザーを表示できますか。

現時点で最適な方法は、これらのユーザーを Azure AD テナントに追加し、パートナーセンターに追加して、パートナーセンターで **自分のプロファイル** を使用して Microsoft Learn アカウントを関連付けることができるようにすることです。 

MSA アカウントのみをトレーニングに使用するユーザーについては、Microsoft Learn チームが、仕事用の電子メールを Microsoft Learn プロファイルに関連付けることができるようになります。 

## <a name="next-steps"></a>次のステップ

詳細なレポートについては、「 [Partner Center Insights](partner-center-insights.md)」を参照してください。

>[!NOTE] 
> このレポートを作成する生データは、Insights ダッシュボードの [レポートのダウンロード] セクションからダウンロードできます。 [詳細情報](pci-download-reports.md) 