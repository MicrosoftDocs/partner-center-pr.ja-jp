---
title: 制限付きの直接請求機能
ms.topic: article
ms.date: 10/09/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: CSP の直接請求パートナーの要件と、機能が制限されるのを回避するために行う方法について説明します。 機能が制限されていないか確認します。
author: billLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: b3b1f3e1593f7e35bd3b9ed6c56ea28683bff95a
ms.sourcegitcommit: 7a6836bd962d5b426a8cb34a9132a87cbbbf39f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/13/2021
ms.locfileid: "109855490"
---
# <a name="restricted-direct-bill-capabilities-and-the-requirements-needed-for-csp-direct-bill-partners"></a>CSP 直接請求パートナーに必要な制限付き直接請求機能と要件

**適切なロール**: グローバル管理者

## <a name="overview"></a>概要

直接請求パートナーは、CSP [直接請求パートナー](direct-partner-new-requirements.md) プログラムに残す新しい要件を満たす必要があります。 そうしないと、直接請求機能へのアクセス権が最終的に制限され、特定のタスク (その顧客についての新しい購入の実行など) を実行できなくなります。

> [!Note]
> CSP 直接請求パートナー プログラムの新しい要件を満たしていない直接請求パートナーは、直接請求機能が制限される場合に Microsoft から通知されます。 これは、直接請求パートナーから間接リセラーへの移行を選択した場合でも、すべての直接請求パートナー [に](transition-direct-to-indirect.md) 適用されます。  

## <a name="how-to-tell-if-your-direct-bill-capabilities-has-been-restricted"></a>直接請求機能が制限された場合の確認方法

直接請求パートナー テナントから直接請求機能へのアクセスが制限されているかどうかを確認するには、次の手順に従います。

1. [パートナー センター ダッシュボード](https://partner.microsoft.com/dashboard)にサインインします。

2. [アカウント設定 **] [法的プロファイル**  ->  **] に移動します**。

3. [ **プログラム情報] で**、状態 **Microsoft クラウド ソリューション プロバイダー探します**。

4. プログラムの状態に **値が制限** されている場合は、直接請求パートナー テナントの直接請求機能へのアクセスが制限されています。

## <a name="affected-direct-bill-capabilities"></a>影響を受ける直接請求機能

直接請求機能が制限されている場合は、顧客に対して新しい購入を行パートナー センター。 この制限には次が含まれます。

- Azure サブスクリプション

- ライセンスベースのサブスクリプション

- 既存のライセンス ベースのサブスクリプションに新しいアドオンを追加します。

- ソフトウェアおよび予約製品 (ソフトウェア サブスクリプション、永続的ソフトウェア、Azure 予約仮想マシン インスタンスなど) を 1 回購入します。

また、CSP プログラムで [Azure パートナー共有](shared-services.md) サービス オファーを使用して、独自に使用するために新しい Azure サブスクリプションを購入することはできません。

既存の直接請求サブスクリプションは影響を受けません。 それらは有効なまま残り、自動的に更新されます。 取り消されるまで、引き続き Microsoft から直接請求されます。 既存のサブスクリプションは、引き続き次の方法で管理できます。

- 既存のサブスクリプションを中断します

- 既存のライセンス ベースのサブスクリプションのライセンス数を調整する

- サブスクリプションに対する既存のアドオンのライセンス数を調整します。 

    >[!Note]
    >新しいアドオンは新規購入として扱われるため、既存のサブスクリプションに追加することはできません。

- 新しい Azure リソースのデプロイと、既存の Azure リソースの管理は、既存の Azure サブスクリプションの下で行います。 これには、Azure Marketplace と Visual Studio サブスクリプションで利用可能なリソースが含まれます。

新規購入だけでなく、パートナー センターで次の直接請求機能にアクセスすることもできません。

- 新しい顧客テナントを作成することはできません。 パートナーセンターの [**顧客**] ページにある [**顧客の作成**] オプションは使用できません。

- 直接再販業者の関係を要求している顧客への招待を生成することはできません。 パートナーセンターの [**顧客**] ページにある [**再販業者の関係を要求する**] オプションは使用できません。

    >[!NOTE]
    >直接請求パートナーから間接リセラーへの移行の一環として、直接請求パートナーテナントを間接リセラーとして既に登録している場合は、代わりに間接再販業者の関係を要求する顧客への招待を生成できます。

- 新しいサンドボックステナントを作成することはできません。 各ダイレクト請求パートナーテナントは、直接請求 API 統合用に1つのサンドボックステナントを作成できます。 以前に作成したことがない場合は、直接請求先パートナーの機能が制限された後でその操作を行うことはできません。  

## <a name="next-steps"></a>次の手順

- [間接リセラーになることについての追加情報](https://assetsprod.microsoft.com/csp-directbill-to-indirect-transition.pdf)

- [CSP の直接パートナーの新しい要件](direct-partner-new-requirements.md)
