---
title: Azure プランへの顧客の移行 | パートナー センター
ms.topic: article
ms.date: 11/25/2019
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 顧客を Azure プランに簡単に移動する方法について説明します。
author: LauraBrenner
ms.author: labrenne
Keywords: ''
robots: ''
ms.localizationpriority: high
ms.openlocfilehash: 0420966e13f0ee7151dd9474d597b8253a1ecfff
ms.sourcegitcommit: c793c1b61f50fc0b0a12c95cedd9f57b31703093
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/03/2019
ms.locfileid: "74722289"
---
# <a name="transition-your-customers-to-azure-plan"></a>顧客の Azure プランへの移行

**適切なロール**

- 管理エージェント
- 課金の管理
- 全体管理者
- ヘルプデスク エージェント
- 販売代理店
- ユーザー管理者

間接プロバイダーおよび直接請求パートナーは、Azure 向け CSP プログラムで利用可能な新しいコマース エクスペリエンスに移行できます。 (間接リセラーは、間接プロバイダーを通じて行う必要があります)。パートナーからの購入、マイクロソフト販売者からの購入、または Web 上での直接購入にかかわらず、クラウド サービスを簡単に購入するための最新の方法が顧客に提供されます。

移行機能は、新しい Azure 向けコマース エクスペリエンスに移行する顧客で、Microsoft 顧客契約に署名している顧客のみを対象としています。Office 365 や Dynamics 365 などの CSP の他のプランは対象外です。

## <a name="transition-existing-csp-offers-to-an-azure-plan"></a>既存の CSP プランの Azure プランへの移行

パートナー センターで、既存の CSP Azure プランから CSP プログラムの新しいコマース エクスペリエンスである Azure プランで管理される Azure サービスに顧客を移行させることができます。 この移行には、次のもののみが必要です。

- パートナーとエンドカスタマーの間にパートナー センターを通じて再販業者関係が確立されている必要であり、顧客が Microsoft 顧客契約に署名している必要があります。

### <a name="select-transition-to-azure-plan"></a>Azure プランへの移行を選択する

1. 顧客向けの Azure プランを選択します。

2. **[請求を Azure プランに移行する]** を選択します。

![移行](images/azure/transition1.png)

3. **[続行]** を選択します。

![移行](images/azure/transition2.png)

これにより、移行が発生する Azure portal に移動します。 顧客は、他の操作を行うことなく、Azure プランに移行されます。 

**移行ワークフローによって、前提条件となる手順が自動化されます**。 

- Azure プランの購入 
- ダイレクト CSP での顧客ごとに 1 つのプラン シナリオ  
- リセラーごとに 1 つのプラン  

例として、パートナーが 2つの Microsoft Azure プランを購入し、その購入の中に 2 つの異なる POR が含まれているとします。 この場合、移行ワークフローでは、2 つの Azure プラン (リセラーごとに 1 つ) が購入され、各 Azure サブスクリプションが Azure プランに自動的にマップされます。  

**Azure サブスクリプションの Azure プランへのマッピング**

Azure プランを購入すると、システムによって既存の Azure サブスクリプションが Azure プランにマップされます。 進行状況は、パートナー センターだけでなく Azure portal でも確認できます。 

4. 顧客のパートナー センターの **[サブスクリプション]** ページに戻り、顧客の現地通貨を使用して予算制限を更新します。 

![移行](images/azure/transition3.png)

>[!NOTE]
>パートナー センターで設定した予算は、Azure portal には引き継がれません。 Azure portal で、予算とアラートも設定する必要があります。

Azure プランに移行すると、この顧客用の Azure サブスクリプションを購入することはできなくなります。 サブスクリプションは、Azure portal で Azure プランの中に作成します。

>[!NOTE]
> Azure プランで RBAC を通して購入されたすべての Azure サブスクリプションに対し、現地通貨で請求および課金されます。 為替レートは使用されません。

### <a name="track-your-transition-details"></a>移行の詳細を追跡する

パートナー センターだけでなく、Azure portal でも移行の進行状況を確認してください。

![詳細の表示](images/azure/details1.png)

**パートナーに対する請求の影響**

既存の CSP Azure プランから顧客を移行する場合、次のような請求の影響が発生します。

- 元の CSP Azure サブスクリプションの終了時点までのすべての使用量については、既存の CSP 請求書で請求されます。

- 既存の CSP サブスクリプションに対する管理者アクセス権を持っている場合は、そのサブスクリプションが移行されたときに引き続きアクセス権を所有します。

ダイレクト エンタープライズ契約を CSP に移行し、サーバーとクラウドの登録を Azure サービスに移行するには、[Microsoft パートナー契約での Azure サブスクリプションの課金所有権の取得](https://docs.microsoft.com/azure/billing/mpa-request-ownership)に関する記事を参照してください。

**監査ログ**:

請求を調整するには、 **[サブスクリプション]** ページで "Microsoft Azure" (0145P) サブスクリプションの履歴を確認します。 

"Microsoft Azure" (0145P) サブスクリプションは、次の 2 つの部分で構成されます。
1. コマース サブスクリプション 
2. Azure サブスクリプション (権利)

移行が完了すると、Azure サブスクリプションは新しい Azure プランの下に移動され、コマース サブスクリプションはこれ以上の使用が報告されないように停止されます。  

>[注]\:CSP で Microsoft Azure (0145P) サブスクリプションを 購入した場合、コマース サブスクリプションと Azure サブスクリプション (権利) の価格は同じになります。 これは、課金所有権の変更または譲渡で価格が異なる場合にのみ発生します。 

**移行に関する問題**

移行中に問題が発生することは想定されていません。 発生した場合は、移行ワークフロー自体の中で更新が実行されます。 Azure の使用に障害が発生することはありません。  

**次の手順**

- [Azure プランのサブスクリプションとリソースを管理する](azure-plan-manage.md)

- [パートナー獲得クレジット - 概要](partner-earned-credit.md)



