---
title: パートナー獲得クレジットの計算方法
ms.topic: article
ms.date: 06/15/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Azure プランのパートナー獲得クレジット (PEC) の側面を計算する方法について説明します。 これには、パートナーと間接プロバイダーの資格要件が含まれます。
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.custom: SEOJUNE.20
ms.openlocfilehash: 437d1bbd6a5ef3a18d149df2b533fdd2d0ed735d
ms.sourcegitcommit: 1796d3d0ec2e06a3792852377ff81127b4d22fe0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/17/2020
ms.locfileid: "84908900"
---
# <a name="how-partner-earned-credit-pec-is-calculated-for-partners-in-the-cloud-solution-provider-program"></a>クラウドソリューションプロバイダープログラムのパートナーに対してパートナーの獲得クレジット (PEC) を計算する方法

**適切なロール**

- グローバル管理者
- 課金管理者

Microsoft 365 年中無休の IT 運用管理、または CSP における顧客の Azure 環境全体を所有するパートナーは、PEC を利用できます。 PEC は、Microsoft との直接の課金関係を持つパートナーに請求書の一部として提供されます。 クレジットは日単位で計算され、月次請求書に反映されます。 CSP の既定では、顧客のサブスクリプションに対する必要なアクセス権がパートナーに付与されます。これにより、サブスクリプションのリソースを24時間365日体制で管理し、制御することができます。 次のセクションでは、お客様が取引先へのアクセスをプロビジョニングするためのその他の方法について説明します。


## <a name="important-eligibility-and-calculation-requirements"></a>重要な資格と計算の要件:

- パートナーには、active MPN agreement と有効なルールベースのアカウント制御 (RBAC) の役割があります。これにより、管理対象の azure 資産の獲得クレジットを受け取ることができます。 [有効な RBAC ロール] の詳細情報

- 間接プロバイダーは、お客様または間接リセラーか、またはその両方が、CSP 内の顧客の Azure リソースを24時間365日体制で管理および管理している場合に、PEC の対象となります。

- PEC は、パートナーによって管理される CSP 内の顧客の Azure 資産に対して課金される (請求可能な) 消費量に関連付けられます。 

- PEC は、Microsoft によって請求される CSP のパートナー (間接プロバイダーおよびダイレクト請求パートナー) にのみご利用いただけます。

- 対象サービス: パートナーの獲得クレジットは、価格表に記載されているすべての Azure 1PP Azure の使用量に適用されます。 3PP や Azure Reservations に限定されない例外もあります。

- PEC は毎日計算され、毎日偵察ファイルで表示できます。 パートナー (プロバイダーを通じて) は、PEC を確実に取得するために、一日中 (24 時間365日) のアクセス権を持っている必要があります。

- PEC は、Azure リソース レベルで獲得されます。 パートナーがサブスクリプションまたはリソースグループレベルで有効なアクセス権を持っている場合は、上位のエンティティにロールがある各リソースが PEC を獲得します。 

- PEC は、パートナーの月次請求書に記載されます。 請求書の料金は正味です。 詳細は、請求書の偵察ファイルに表示されます。

Azure サブスクリプションを管理するためのアクセス権を取得する方法と、MPN ID を RBAC ロールにリンクする方法については、「 [azure プランでのサブスクリプションとリソースの管理」](azure-plan-manage.md)を参照してください。

詳細情報

- [Azure プラン-課金](azure-plan-billing.md)

- [CSP の新しいコマース エクスペリエンスの価格表](azure-plan-price-list.md)