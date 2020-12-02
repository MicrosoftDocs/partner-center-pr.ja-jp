---
title: 間接リセラーのパフォーマンス分析
description: 分析を使用して、間接リセラーがどのように実行されているかを確認します。成功と領域の両方で、さらに注意が必要になる場合があります。
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: shganesh
ms.author: shganesh
ms.topic: article
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.date: 05/13/2020
ms.openlocfilehash: b7158f0ba52cece8b143cbaf592f3b0c4667fe27
ms.sourcegitcommit: 4043c791402f0acebee6ede160a135e87fe92493
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/01/2020
ms.locfileid: "96474055"
---
# <a name="use-analytics-to-analyze-the-performance-of-your-indirect-resellers"></a>分析を使用して間接リセラーのパフォーマンスを分析する

**適切なロール**

- グローバル管理者
- ユーザー管理の管理者


データはビジネス上の意思決定を促進します。 **リセラー分析** のページのメトリックを使用して、パートナーの成功度、間接リセラーの成功度、注意が必要な分野を把握します。 新しいビジネス目標を計画するときに、この情報を使用できます。

> [!NOTE]
> 間接リセラー分析は、クラウドソリューションプロバイダープログラムの間接プロバイダーに対してのみ使用できます。

## <a name="types-of-reseller-analytics-metrics-you-can-view"></a>表示可能なリセラー分析メトリックの種類

次のメトリックを追跡しています。

**まとめ**  
 - **Total resellers** (リセラーの合計数): サブスクリプションの最終日にアクティブなリセラーの数  
 - **New resellers** (新規リセラー数): 指定した期間の新規間接リセラーの数  
 - **Active resellers** (アクティブなリセラー数): MPNID に 1 つ以上のサブスクリプションがあり、サブスクリプションの状態がプロビジョニング解除ではない間接リセラーの数  
 - **Transacting resellers** (取引のあるリセラー数): 指定した期間に販売したサブスクリプションがある間接リセラーの数  

**市場別のリセラー数**  
 - 地域別の合計リセラー数  

**サブスクリプションの販売数による上位リセラー**
 - リセラーのサブスクリプション販売数で並べ替えられたリセラーの一覧  

**サブスクリプション数による上位製品**  
 - **Dynamics 365**: サブスクリプションの販売数で並べ替えられた Dynamics 365 製品  
 - **EMS**: エンタープライズ管理サービス サブスクリプションの販売数  
 - **Microsoft 365**: Microsoft 365 サブスクリプションの販売数  
 - **Office 365**: サブスクリプションの販売数で並べ替えられた Office 365 製品  

**新しいサブスクリプション**  
 - 日付ごとの追加された新規サブスクリプションの数  

**サブスクリプションのチャーン**  
 - **New subscriptions** (新規サブスクリプション数): 日付ごとの追加された新規サブスクリプションの数  
 - **Deprovisioned subscriptions** (プロビジョニング解除されたサブスクリプション数): 日付ごとのプロビジョニング解除または中断されたサブスクリプションの数  

**新規リセラーの詳細**  
 - **Reseller name** (リセラー名): 間接リセラーの名前  
 - **Location** (場所): 間接リセラーが営業している市場  
 - **Subscriptions** (サブスクリプション数): リセラーが販売したサブスクリプションの数  
 - **Licenses** (ライセンス数): すべてのサブスクリプションを合わせてリセラーが販売したライセンスの合計数  

**MPA の署名された状態**

このセクションでは、CSP 間接リセラーの MPA の署名された状態について説明します。

 - **再販業者名**: CSP 間接リセラーの名前
 - **MPN id**: 間接リセラーの MPN id
 - **リージョン**: 間接リセラーが運用するリージョン
 - **MPN 審査 status**: 間接リセラーの審査の状態
 - **Mpa の署名済みステータス**: 間接リセラーの mpa 署名状態

グラフのダウンロードアイコンをクリックして、追加のディメンションを含む MPA 署名済み状態データをダウンロードします
  
## <a name="next-steps"></a>次のステップ

- [サブスクリプションとライセンスを分析して、ビジネス上の意思決定を促進する](analyze-subscriptions-licenses.md)