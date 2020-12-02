---
title: サブスクリプションとライセンスの分析
description: '[サブスクリプションとライセンス分析] ページのメトリックを使用して、注意が必要な成功と領域を特定する方法について説明します。'
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: amitravat
ms.author: amrava
ms.topic: article
ms.localizationpriority: medium
ms.custom: SEOJULY.20
ms.date: 07/08/2020
ms.openlocfilehash: 45a088129d09395abf355efde08c772744b98672
ms.sourcegitcommit: 4043c791402f0acebee6ede160a135e87fe92493
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/01/2020
ms.locfileid: "96474089"
---
# <a name="analyze-subscriptions-and-licenses-to-help-you-drive-business-decisions-and-new-goals"></a>サブスクリプションとライセンスを分析して、ビジネス上の意思決定や新しい目標を促進

**適切なロール**

- グローバル管理者
- ユーザー管理の管理者
- 管理エージェント
- 販売代理店

データはビジネス上の意思決定を促進します。 [ **サブスクリプションとライセンス分析** ] ページのメトリックを使用して、さらに注意が必要な成功と領域を特定します。 新しいビジネス目標を計画するときに、この情報を使用できます。

**CSP TTM 収益 (米国ドル)**: このメトリックは、この csp アカウントが関連付けられているパートナーの場所アカウントとパートナーのグローバルアカウント (PGA) の末尾の12か月 (ttm) に対して請求される、集計された csp を表します。 別の PGA がある他の CSP アカウントがある場合は、それぞれにサインインして、対応する集計された TTM 収益を確認する必要があります。  [Download details] \ (ダウンロードの詳細 \) リンクをクリックすると、MPN ID ごとの TTM 収益 (USD) の内訳が表示されます。

レポートの残りの部分は、次の製品に基づいてピボットできます。

 - **Dynamics 365**: Dynamics 365 のデータ  
 - **EMS**: エンタープライズ管理サービスのデータ  
 - **Microsoft 365**: Microsoft 365 データ  
 - **Office 365**: Office 365 データ  


## <a name="types-of-subscription-and-license-metrics-you-can-view"></a>表示可能なサブスクリプションとライセンスメトリックの種類

次のメトリックを追跡しています。

**まとめ**  
 - **Subscriptions sold** (サブスクリプションの販売数): 指定した期間に作成されたサブスクリプションの数  
  
 - **Licenses sold** (ライセンスの販売数): 指定した期間に販売されたライセンスの数  
  
 - **Subscriptions renewing in 30 days** (30 日以内に更新するサブスクリプション): 指定した期間中に状態がアクティブで、**Autorenew** が true であるサブスクリプションの数
 
 - **Active subscriptions** (アクティブなサブスクリプション): 状態が **Active** であるサブスクリプション  
 
 - **Suspended subscriptions** (中断されたサブスクリプション): 中断されたサブスクリプションの数、日付フィルターなし  

**製品の内訳**
  
 - **Subscription count** (サブスクリプション数): サブスクリプションの販売数で並べ替えた上位 5 つの製品  
 
 - **License count** (ライセンス数): ライセンスの販売数で並べ替えた上位 5 つの製品

**サブスクリプションの維持**

 - **Renewed subscriptions** (更新されたサブスクリプション): 過去 30 日間に更新されたサブスクリプション  

**サブスクリプションのチャーン**  
 - **New subscriptions** (新規サブスクリプション): 期間中の新しいサブスクリプションの数 (試用版プランを除く)  
 
 - **Deprovisioned subscriptions** (プロビジョニング解除されたサブスクリプション数): 日付ごとのプロビジョニング解除または中断されたサブスクリプションの数  

**中断されたサブスクリプション** 
 
 - 状態が **Suspended** (中断) であるすべてのサブスクリプションの一覧 (試用版プランを除く)  
  
**アクティブなサブスクリプション**

 - すべてのアクティブなサブスクリプションの一覧  

**試用版のサブスクリプションの変換**  

 - **Trial conversion** (試用版の変換): 指定した期間中に試用版から有料版への変換が行われたすべての **アクティブ** サブスクリプションの数  

**30 日以内に終了する試用版サブスクリプション**  

 - 開始されたが、終了日が 30 日以内であり、有料版の開始日がサブスクリプションに関連付けられていない試用版の一覧  

## <a name="next-steps"></a>次のステップ

- [間接リセラーのパフォーマンスを分析する](analyze-indirect-resellers.md)