---
title: 顧客を現在の Azure プランから Azure プランに移行する
ms.topic: how-to
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: CSP パートナーが、パートナー センターを使用して顧客を既存の CSP Azure プランから、Azure プランで管理される Azure サービスに移行する方法について説明します。
author: mowree
ms.author: mowrim
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.date: 06/16/2020
ms.openlocfilehash: bcc6534995a7550f0f09d1da2d52cbf676b66c40
ms.sourcegitcommit: 7e19c211b1d5f2db2a4c56a743b14c8485decd99
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/03/2020
ms.locfileid: "87527508"
---
# <a name="transition-customers-to-azure-plan-from-existing-csp-azure-offers"></a>顧客を既存の CSP Azure プランから Azure プランに移行する

**適切なロール**

- 管理エージェント
- 課金管理者
- グローバル管理者
- ヘルプデスク エージェント
- 販売代理店
- ユーザー管理の管理者

間接プロバイダーおよび直接請求パートナーは、Azure 向け Microsoft クラウド サービス プロバイダー (CSP) プログラムで利用可能な新しいコマース エクスペリエンスに移行できます。 (間接リセラーは、間接プロバイダーを通じて行う必要があります)。パートナーからの購入、マイクロソフト販売者からの購入、または Web 上での直接購入にかかわらず、クラウド サービスを簡単に購入するための最新の方法が顧客に提供されます。

移行機能は、新しい Azure 向けコマース エクスペリエンスに移行する顧客で、Microsoft 顧客契約に署名している顧客のみを対象としています。Office 365 や Dynamics 365 などの CSP の他のプランは対象外です。

## <a name="transition-existing-csp-offers-to-an-azure-plan"></a>既存の CSP プランの Azure プランへの移行

パートナー センターで、既存の CSP Azure プランから CSP プログラムの新しいコマース エクスペリエンスである Azure プランで管理される Azure サービスに顧客を移行させることができます。 これを行うには、パートナーと顧客の間にパートナー センターを通じて再販業者関係が確立されている必要があり、顧客が Microsoft 顧客契約に署名している必要があります。

### <a name="select-transition-to-azure-plan"></a>Azure プランへの移行を選択する

1. 顧客向けの Azure プランを選択します。

2. **[請求を Azure プランに移行する]** を選択します。

   :::image type="content" source="images/azure/transition1.png" alt-text="使用状況に基づいたサブスクリプションのレポート情報を示すスクリーンショット。選択可能な次のオプションが表示されています:[Azure サブスクリプション請求を Azure プランに移行する]。":::

3. **[続行]** を選択します。

   :::image type="content" source="images/azure/transition2.png" alt-text="[Transition to Azure plan]\(Azure プランへの移行\) というタイトルのダイアログ ボックス。移行についての説明と、[続行] および [キャンセル] という選択可能な 2 つのオプションが表示されています。":::

   顧客は、Azure プランに移行されます。

   **移行ワークフローによって、前提条件となる手順が自動化されます**。

   - Azure プランの購入
   - ダイレクト CSP での顧客ごとに 1 つのプラン シナリオ  
   - リセラーごとに 1 つのプラン  

   例として、パートナーが 2 つの Microsoft Azure プランを購入し、その購入の中に 2 つの異なる POR が含まれているとします。 この場合、移行ワークフローでは、2 つの Azure プラン (リセラーごとに 1 つ) が購入され、各 Azure サブスクリプションが Azure プランに自動的にマップされます。  

   **Azure サブスクリプションの Azure プランへのマッピング**

   Azure プランを購入すると、システムによって既存の Azure サブスクリプションが Azure プランにマップされます。 進行状況は、パートナー センターだけでなく Azure portal でも確認できます。

4. 顧客のパートナー センターの **[サブスクリプション]** ページに戻り、顧客の現地通貨を使用して予算制限を更新します。

   :::image type="content" source="images/azure/transition3.png" alt-text="パートナー センターの [サブスクリプション] ページの一部分。請求期間の予算制限が現地の通貨で設定されています。":::

   >[!NOTE]
   >パートナー センターで設定した予算は、Azure portal には引き継がれません。 Azure portal で、予算とアラートも設定する必要があります。

   Azure プランに移行すると、この顧客用の Azure サブスクリプションを購入することはできなくなります。 サブスクリプションは、Azure portal で Azure プランの中に作成します。

   >[!NOTE]
   > Azure プランで RBAC を通して購入されたすべての Azure サブスクリプションに対し、現地通貨で請求および課金されます。 為替レートは使用されません。

### <a name="track-your-transition-details"></a>移行の詳細を追跡する

パートナー センターだけでなく、Azure portal でも移行の進行状況を確認してください。

:::image type="content" source="images/azure/details1.png" alt-text="サブスクリプションごとに移行の詳細リストが表示されている表のスクリーンショット。サブスクリプション ID、移行日、移行の状態が含まれています。":::

### <a name="billing-impact-to-partners"></a>パートナーに対する請求の影響

既存の CSP Azure プランから顧客を移行する場合、次のような請求の影響が発生します。

- 元の CSP Azure サブスクリプションの終了時点までのすべての使用量については、既存の CSP 請求書で請求されます。

- 既存の CSP サブスクリプションに対する管理者アクセス権を持っている場合は、そのサブスクリプションが移行されたときに引き続きアクセス権を所有します。

ダイレクト エンタープライズ契約を CSP に移行し、サーバーとクラウドの登録を Azure サービスに移行するには、[Microsoft パートナー契約での Azure サブスクリプションの課金所有権の取得](https://docs.microsoft.com/azure/billing/mpa-request-ownership)に関する記事を参照してください。

### <a name="audit-log"></a>監査ログ

請求を調整するには、 **[サブスクリプション]** ページで "Microsoft Azure" (0145P) サブスクリプションの履歴を表示します。

"Microsoft Azure" (0145P) サブスクリプションは、次の 2 つの部分で構成されます。

1. コマース サブスクリプション
2. Azure サブスクリプション (権利)

移行が完了すると、Azure サブスクリプションは新しい Azure プランの下に移動され、コマース サブスクリプションはこれ以上の使用が報告されないように停止されます。  

>[!NOTE]
>CSP で Microsoft Azure (0145P) サブスクリプションを 購入した場合、コマース サブスクリプションと Azure サブスクリプション (権利) の価格は同じになります。 これは、課金所有権の変更または譲渡で価格が異なる場合にのみ発生します。

### <a name="transition-issues"></a>移行に関する問題

移行中に問題が発生することは想定されていません。 発生した場合は、移行ワークフロー自体の中で更新が実行されます。 Azure の使用に障害が発生することはありません。  

## <a name="next-steps"></a>次の手順

- [Azure プランのサブスクリプションとリソースを管理する](azure-plan-manage.md)

- [パートナー獲得クレジット - 概要](partner-earned-credit.md)
