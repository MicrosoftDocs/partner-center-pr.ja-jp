---
title: 商用 marketplace 製品の課金
ms.topic: article
ms.date: 05/12/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: パートナーセンター内の商用マーケットプレースから購入した ISV SaaS 製品またはサブスクリプションの課金のしくみについて説明します。
author: LauraBrenner
ms.author: labrenne
keywords: サブスクリプション, 製品, 購入, Marketplace, サードパーティ, ISV, 請求, 請求書, 調整, 偵察ファイル
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 9672850b699a2660f646ede5250e52298f5522cd
ms.sourcegitcommit: 093039319fab2a44ab147159bc4be832f1330d57
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/14/2020
ms.locfileid: "83394154"
---
# <a name="billing-for-commercial-marketplace-products-and-subscriptions-in-partner-center"></a>パートナーセンターでの商用 marketplace 製品とサブスクリプションの課金

**適用対象**

- パートナー センター
- CSP プログラムのパートナー

**適切なロール**

- グローバル管理者
- 課金管理者

CSP プログラムのパートナーとして、パートナーセンターを使用して、商用マーケットプレースの ISV 発行元からライセンスベースの SaaS 製品を購入できます。 その後、これらの種類の購入に関する請求書にアクセスできます。 請求期間はカレンダー月の最初の日から開始され、カレンダー月の最後の日に終了します。 請求書は、次の月の8日に利用可能になります。

請求書には、パートナーセンターの[ダッシュボード](https://partner.microsoft.com/dashboard/)から、または[パートナーセンター api](https://docs.microsoft.com/partner-center/develop/)を使用してアクセスできます。

CSP プログラムのパートナーは、パートナーセンターまたは Azure portal (お客様が以前に購入した CSP に購入した Azure テナントを使用) から製品を購入した場合に、お客様が購入した ISV 商用 marketplace ソリューションに対して課金されます。

>[!NOTE]
>お客様が独自の Azure AD テナント (CSP プログラムのパートナーから購入したものではない) を使用している場合、お客様は独自の ISV SaaS ソリューションを ([Microsoft AppSource](https://appsource.microsoft.com/)または[Azure Marketplace](https://azuremarketplace.microsoft.com/)) から直接購入することもできます。 その場合は、Microsoft から直接請求書を受け取ります。 同様に、CSP プログラムのパートナーが Azure サブスクリプションまたは新しい Azure プランを顧客に販売し、そのテナントへの[ロールベースのアクセス権](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles)を顧客 (または間接**リセラー) に**付与した場合、その顧客 (または間接リセラー) は、事前の承認または CSP パートナーへの通知を行わずに、商用の marketplace プランを購入できます。 このような場合、マイクロソフトは、顧客が行った購入について、CSP プログラムに直接パートナーに通知しません。 ただし、Microsoft では、Azure サブスクリプションでのアクティビティに関するアラートまたは通知を設定するために使用できるオプションの[Azure Monitor](https://docs.microsoft.com/azure/azure-monitor/platform/alerts-activity-log)メカニズムを提供しています。

## <a name="access-billing-information-for-commercial-marketplace-products"></a>商用 marketplace 製品の課金情報へのアクセス

請求書を表示できる状態になると、会社の全体管理者または請求管理者にはメールが送信されます。 市販の marketplace 製品を購入するための最新の請求書と調整ファイルにアクセスするには、次のようにします。

1. パートナー センター [ダッシュボード](https://partner.microsoft.com/dashboard/)にサインインします。

2. パートナー センター メニューで **[請求]** を選択します。 

    課金ページの上部に2つのタブが表示されます。**定期的**および**定期的な購入と1回限りの購入**です。 各タブでは、さまざまな marketplace 製品の請求書と調整 (recon) ファイルにアクセスできます。

    - [**定期的**なタブ]: Office 365、Microsoft 365、Dynamics 365、Azure Active Directory、PowerBI Pro、および Microsoft Azure に関連するサブスクリプションの請求書と調整ファイルを表示します。

    - [**定期的および1回限りの購入**] タブ: azure プラン、azure 予約、ソフトウェア、および商用 marketplace 製品の請求書と調整ファイルが表示されます。
  
3. [**定期的な購入と1回限りの購入**] タブを選択します。異なる通貨で顧客のサブスクリプションを購入した場合は、通貨ごとにタブが表示されます。 このページでは、次のような操作を行うことができます。

    - 最新の請求書と調整ファイルを表示するには、[**請求書**] または [**調整ファイル**] を選択します。 (必要に応じて、[パートナーセンター api](https://docs.microsoft.com/partner-center/develop/)を使用して、最新の請求書にアクセスし、ファイルデータにアクセスすることもできます。

    - 以前の請求書とファイルを表示するには、下の [**請求履歴**] 行を展開します。

    - 最新のアカウント活動に基づいて、いつでもアカウントの残高や請求金額を確認するには、[**推定**] 見出しの下のリンクを選択します。  

    >[!NOTE]
    > 月の8日目に請求書を投稿すると、税金とその他の適用可能な料金およびクレジットが含まれます。 これは、請求期間中に発生した最終的な金額と異なる場合があることを意味します。

## <a name="more-about-invoices-and-recon-files-for-commercial-marketplace-products"></a>請求書と、商用 marketplace 製品のファイルに関する詳細

このセクションでは、サードパーティの ISV 発行元の顧客向けに購入した商用 marketplace SaaS サブスクリプションの請求書と調整ファイルの詳細について説明します。

[パートナーセンター] メニューの [**課金**] オプションから [**定期的かつ1回限りの購入**] を選択すると、Microsoft (ファーストパーティ) と ISV (サードパーティ) の購入に関連する請求書と調整ファイルにアクセスできるようになります。 これらの購入には、次のものが関連付けられます。

- SaaS サブスクリプション (Microsoft または ISV 発行元のいずれか)

- Azure プラン

- Azure Reservations

- その他のサブスクリプションベースのソフトウェア (Microsoft または ISV 発行元のいずれか)

これらの購入の例には、SUSE Linux ソフトウェア (ソフトウェアサブスクリプション) や Azure ISV SaaS 製品サブスクリプションなどがあります。

>[!NOTE]
> 請求書とファイルへの登録方法の詳細については、「[課金の概要](billing.md)」も参照してください。

### <a name="tips-on-reading-your-invoice"></a>請求書の読み取りに関するヒント

サードパーティの ISV 発行元からライセンスベースの SaaS 製品を購入した場合は、請求書の料金のみが表示されます。 これは、ISV の SaaS 製品が基になる Azure インフラストラクチャリソースを使用 (または消費) する場合にも当てはまります。 これは、ISV の SaaS 製品に対するお客様の Azure インフラストラクチャの使用料金は、ISV に直接請求されるためです。 (Isv には、関連付けられている Azure 従量課金料金が、Azure の使用量に関する毎日評価される請求書調整ファイルとして表示されます)。

請求書にはいくつかのページが含まれます。

- **請求書のページ 1:** CSP プログラムパートナーの請求の詳細について概要を説明します。 これには、請求期間、請求書番号、支払い条件 (Net 60 日)、請求書による支払い方法 (ネットワークまたはチェックによる支払い) の料金の概要が含まれます。

- **請求書のページ 2 (およびそれ以降のページ):** ファーストパーティの Microsoft 購入とサードパーティの ISV (ライセンスベース) の購入の両方について、商用 marketplace からの料金を詳細に説明します。 ISV ライセンスベースの購入は、各製品名の下の**発行元**の行で特定できます。 関連する調整ファイルは、特定の請求書の請求についての詳細な課金を提供します。

- **請求書の最終ページ:** ISV からライセンスベースの marketplace 製品に対して課金された場合、この最終ページには、ISV 発行元の名前とアドレスに関する詳細が表示されます。

### <a name="tips-on-reading-your-reconciliation-file"></a>調整ファイルの読み取りに関するヒント

**定期的および1回限りの購入**調整ファイルには、請求書の料金に対応する追加の詳細を含むいくつかの列が含まれています。 **Publishername**列には、Microsoft またはサードパーティの ISV 発行元からの購入であるかどうかが表示されます。

調整ファイルの料金には、$0 という料金が表示される場合があります。 これは、ISV の "無料試用版" プラン (通常は30日または60日) または「ライセンスの持ち込み」プランが原因である可能性があります。

無料試用版 ISV の場合は、次のようになります。

- 無料試用期間は、その期間における ISV のライセンスベースの SaaS 製品のコストを対象としています。 また、関連付けられている Azure インフラストラクチャによるその SaaS 製品の使用に対して課金されることもありません。  ただし、使用量ベースの ISV プランを使用している場合、無料試用版には、基になる Azure インフラストラクチャの使用コストは含まれません。 この場合、Azure インフラストラクチャの使用量の料金は、別の Azure 調整ファイルに表示されます。

- お客様に対して ISV の無料試用対象製品を購入して展開すると、お客様は ISV 発行元によって無料試用版に自動的に登録されます。 無料試用期間は、ISV 発行者によって定義された期間が過ぎると自動的に終了します。 期間が終了すると、顧客には課金されます。 つまり、調整ファイルには試用対象製品の2つの行が表示されることがあります。1つは試用期間を追跡するもの、もう1つは有料プランを追跡するもの (試用期間が終了するまでに $0 のコストが表示されます) です。 試用期間が終了すると、有料プランを示す行には料金が表示されます。 

各列が表す内容の詳細については、「[調整ファイルの使用](use-the-reconciliation-files.md)」を参照してください。 「[パートナーセンターでの課金の種類](billing-different-types.md)」も参照してください。

## <a name="next-steps"></a>次のステップ

- [顧客向けの商用 marketplace 製品を管理する](csp-commercial-marketplace-manage.md)
- [商用 marketplace 製品のサポートについて説明します](csp-commercial-marketplace-support.md)
