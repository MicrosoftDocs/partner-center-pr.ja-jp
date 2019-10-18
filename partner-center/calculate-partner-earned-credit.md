---
title: パートナーの獲得クレジットの計算方法 |パートナーセンター
ms.topic: article
ms.date: 09/17/2019
description: Azure プランのパートナー獲得クレジットの比率を計算する方法
ms.assetid: ''
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.openlocfilehash: eb0dd5ef22632a85ca0227cc9e988a88263e9ddf
ms.sourcegitcommit: 0195355f4526362f4d89f59ea643a5e422b6a9b2
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/27/2019
ms.locfileid: "71318777"
---
# <a name="how-the-partner-earned-credit-pec-is-calculated"></a>パートナーの獲得クレジット (PEC) の計算方法


Microsoft 365 年中無休の IT 運用管理、または CSP における顧客の Azure 環境全体を所有するパートナーは、PEC を利用できます。 PEC は、Microsoft との直接の課金関係を持つパートナーに請求書の一部として提供されます。 クレジットは日単位で計算され、月次請求書に反映されます。 CSP の既定では、顧客のサブスクリプションに対する必要なアクセス権がパートナーに付与されます。これにより、サブスクリプションのリソースを24時間365日体制で管理し、制御することができます。 次のセクションでは、お客様が取引先へのアクセスをプロビジョニングするためのその他の方法について説明します。   


## <a name="important-eligibility-and-calculation-requirements"></a>重要な資格と計算の要件:

- パートナーは、管理対象の azure 資産の獲得クレジットを受け取るために、active MPN agreement と有効なルールベースのアカウント C (RBAC) の役割を持っている必要があります。 [有効な RBAC ロール] の詳細情報

- 間接プロバイダーは、お客様または間接リセラーか、またはその両方が、CSP 内の顧客の Azure リソースを24時間365日体制で管理および管理している場合に、PEC の対象となります。

- PEC は、パートナーによって管理される CSP におけるお客様の Azure 資産の請求 (課金) に関連付けられています。 

- PEC は、Microsoft によって請求される CSP のパートナー (間接プロバイダーおよびダイレクト請求パートナー) にのみご利用いただけます。

- 対象サービス: パートナーの獲得クレジットは、価格表に記載されているすべての Azure 1PP Azure の使用量に適用されます。 3PP や Azure Reservations に限定されない例外もあります。

- PEC は毎日計算され、毎日偵察ファイルで表示できます。 パートナー (プロバイダーを通じて) は、PEC を確実に取得するために、一日中 (24 時間365日) のアクセス権を持っている必要があります。

- Azure リソースレベルまで、PEC が獲得されます。 パートナーがサブスクリプションまたはリソースグループレベルで有効なアクセス権を持っている場合は、上位のエンティティにロールがある各リソースが PEC を獲得します。 

- PEC は、パートナーの月次請求書に記載されます。 請求書の料金は正味です。 詳細は、請求書の偵察ファイルに表示されます。

Azure サブスクリプションを管理するためのアクセス権を取得する方法と、MPN ID を RBAC ロールにリンクする方法については、「 [azure プランでのサブスクリプションとリソースの管理」](azure-plan-manage.md)を参照してください。

詳細情報

- [Azure プラン-課金](azure-plan-billing.md)

- [CSP の新しいコマースエクスペリエンスの価格表](azure-plan-price-list.md)