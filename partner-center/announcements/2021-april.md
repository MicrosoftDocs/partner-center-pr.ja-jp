---
title: 2021 年 4 月のお知らせ
description: 2021 年 4 月の Microsoft パートナー センターのお知らせでは、新しい機能、販売促進、オファー、市場、既存のオファーに対する変更を紹介します。
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: brentserbus
ms.author: brserbus
ms.custom:
- announcement
- references_regions
ms.localizationpriority: high
ms.date: 04/29/2021
ms.openlocfilehash: 798dcb1570a0f6dfc94c7b45fc3c2e152f55cbe5
ms.sourcegitcommit: 22e257d5b334ca8d3fc072f59010a508e1022694
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/06/2021
ms.locfileid: "108702826"
---
# <a name="april-2021-announcements"></a>2021 年 4 月のお知らせ

このページでは、2021 年 4 月の Microsoft パートナー センターのお知らせについて説明します。

## <a name="readiness-updated-csp-customer-address-validation-api-going-live-in-june-testing-capability-now-available"></a><a name="10"></a>準備状況: 更新された CSP 顧客アドレス検証 API が 6 月に運用開始、テスト機能が現在利用可能

### <a name="categories"></a>Categories

- 日付: 2021 年 4 月 30 日
- 準備

### <a name="summary"></a>まとめ

パートナーと顧客が信頼に基づいてビジネスを遂行できるようにするために、Microsoft はパートナーに対して世界中のすべての国の Validate Address API に対する変更をテストすることをお勧めしています。

### <a name="impacted-audience"></a>対象

顧客の住所の詳細を新規作成または既存のものを更新する、CSP 直接請求パートナーと間接プロバイダー

### <a name="details"></a>詳細

Microsoft の基盤は信頼です。 Microsoft は、CSP プログラムで顧客サブスクリプションを処理するために、法令に準拠した安全な顧客住所の検証方法の提供に努めています。 2021 年 3 月 31 日の時点で、Validate Address API に対する変更が発表されています。 2021 年 6 月末の運用開始前にパートナーはこの API をテストすることをお勧めします。 

これらの変更は、Validate Address API にのみ影響を与えることに注意してください。 Create Customer と Update Billing Profile の API には影響がありません。 提案された住所は現在、Create Customer API で使用する必要はありませんが、そうすることを強くお勧めします。

応答では、次のいずれかのステータス メッセージが返されます。

| 状態     | 説明 |    返される住所候補の数 |
|-------|---------------|-------------------|
|Verified shippable (検証済み出荷可能) | 住所が確認され、出荷可能です。 | Single |
|Verified | 住所が確認されました。 | Single |
|Interaction required (対話式操作が必要) | 提案された住所は大幅に変更されており、ユーザーの確認が必要です。 | Single |
|Street partial (番地が不完全) | 住所の番地が部分的であるため、さらに情報が必要です。 | 複数 (最大 3) |
|Premises partial (建物が不完全) | 指定された建物 (ビル番号、部屋番号、その他) が不完全であるため、さらに情報が必要です。 | 複数 (最大 3) |
|複数 | 住所の複数のフィールドが不完全です (street partial と premises partial も含む可能性があります)。 | 複数 (最大 3) |
|なし | 住所が正しくありません。 | なし |
|検証なし | 住所は、検証プロセスを通じて送信できませんでした。 | なし |

米国の郵便番号は、ハイフン付きでさらに 4 桁が返されます (例: 12345-6789)。

### <a name="next-steps"></a>次のステップ

- 詳細なガイダンスについては、[専用のパートナー コレクション](https://partner.microsoft.com/resources/collection/additionalfields-csp-customers-selected-geos#/)でテクニカル ドキュメントとよく寄せられる質問を参照してください。
- Partner Center API と Web ユーザー エクスペリエンスを使用して、変更を組み込む準備をしてください。 
- テスト フライトに含められるようにサンドボックスのテナント ID を領域の専門家 (Ali Khaki) に知らせます。これにより、更新の準備を開始できます。 
- コントロール パネル ベンダー (CPV) ソリューションを使用している場合は、CPV とご相談ください。

### <a name="questions"></a>わからないことがある場合は、

Microsoft との連携でサポートが必要な場合は、パートナー サポートの Yammer グループに問い合わせるか、[サービス要求](https://partner.microsoft.com/dashboard/support/servicerequests/create?stage=2&topicid=aa679372-d996-73df-e244-cb28bbbf28e8)を開いてください。

_______________
## <a name="new-location-for-partner-center-api-swagger-documentation"></a><a name="9"></a>パートナー センター API の Swagger ドキュメントの新しい場所

### <a name="categories"></a>Categories

- 日付: 2021 年 4 月 26 日
- 機能

### <a name="summary"></a>まとめ

パートナー センター API の Swagger ドキュメントは、[前の Swagger ドキュメント サイト](https://apidocs.microsoft.com/services/partnercenter)から[新しい Swagger ドキュメント サイト](https://docs.microsoft.com/rest/api/partner-center-rest/)に移行されました。

### <a name="impacted-audience"></a>対象

パートナー センター API を使用し、クラウド ソリューション プロバイダー (CSP) プログラムに参加している直接請求パートナーと間接プロバイダー

### <a name="details"></a>詳細

2021 年 4 月 26 日の時点で、パートナー センター API の Swagger ドキュメント (Rest API コンテンツを含む) は[新しいサイト](https://docs.microsoft.com/rest/api/partner-center-rest/)に配置されています。 古いサイトは数週間後にアクセスできなくなります。

### <a name="benefits"></a>メリット

パートナー センター API の Swagger ドキュメントには、**Try It** (試用) 機能があります。 この機能を使用するには、ベアラー トークンが必要です。これは、[パートナー センターの認証](https://docs.microsoft.com/partner-center/develop/partner-center-authentication#app--user-authentication)に関する記事に記載されている手順に従って生成できます。

### <a name="next-steps"></a>次の手順

担当チームが手続きの見直し、更新を実施できるよう、この情報を組織で共有してください。

### <a name="questions"></a>疑問がある場合

これらのオファーに関するご質問については、Yammer の関連コミュニティをご確認ください。

________________
## <a name="cloud-solution-provider-csp-software-return-period-policy-and-download-link-expiry-notice"></a><a name="8"></a>クラウド ソリューション プロバイダー (CSP) ソフトウェア返品期間ポリシーとダウンロード リンクの有効期限に関する通知

### <a name="categories"></a>Categories

- 日付: 2021-04-21
- 機能

### <a name="summary"></a>まとめ

CSP ソフトウェア返品期間ポリシーとダウンロード リンクの有効期限に変更点があります。

### <a name="impacted-audience"></a>対象

CSP で永続的ソフトウェアまたはソフトウェア サブスクリプション プランの取引を行っているパートナー

### <a name="details"></a>詳細

パートナー センターを介した永続的ソフトウェアまたはソフトウェア サブスクリプションの購入に関して次の重要な通知にご注意ください。

#### <a name="software-return-period-policy"></a>ソフトウェアの返品期間ポリシー

2021 年 6 月 1 日から、Microsoft Partner Agreement (MPA) に記載されているように、CSP のソフトウェア プランの返品期間が、注文日から 60 日間から 30 日間に変更されます。

ソフトウェア プランの注文が送信されると、パートナーは注文日から 30 日以内であれば、そのような注文への変更を送信できます。

- 30 日間の返品期間内に返されたすべての永続的なソフトウェア ライセンスには、支払済み購入価格のフル クレジットが付与されます。

- 30 日間の返品期間内に返されたすべてのソフトウェア サブスクリプション製品には、支払済み購入価格の日割り計算のクレジットが付与されます。

このメッセージは、2020 年 12 月と 2021 年 4 月に、返品期間や MPS へのその他の更新に関してすべての CSP パートナーに送信された電子メール通信の補足情報です。 MPA に影響する変更に関する詳細については、これらの通知を参照してください。

#### <a name="software-download-link-expiry"></a>ソフトウェアのダウンロード リンクの有効期限

2021 年 6 月 3 日以降、パートナー センターを通じた永続的ソフトウェアおよびソフトウェア サブスクリプション製品の購入におけるソフトウェアのダウンロード リンクについて、最初のダウンロードから 5 日間の有効期限が設けられます。 有効期限は、2021 年 6 月 3 日より前と 2021 年 6 月 3 日以降のすべての購入に適用されます。

### <a name="next-steps"></a>次のステップ

[CSP の返品期間とダウンロード リンクの有効期限に関する FAQ](https://partner.microsoft.com/resources/detail/csp-software-return-period-download-expiry-faq-pdf) を確認し、これらの変更を組織内のすべての適切なチームに通知しましょう。

### <a name="questions"></a>疑問がある場合

これらのオファーに関するご質問については、Yammer の関連コミュニティをご確認ください。

________________
## <a name="open-licensing-program-transitioning-resellers-to-the-cloud-solution-provider-csp-program"></a><a name="7"></a>オープン ライセンス プログラム: クラウド ソリューション プロバイダー (CSP) プログラムへのリセラーの移行

### <a name="categories"></a>Categories

- 日付 : 2021 年 4 月 19 日
- ビジネスの拡大

### <a name="summary"></a>まとめ

この通信では、オープン ライセンス プログラムに近日行われる変更に備える方法を記載しています。

### <a name="impacted-audience"></a>対象

CSP と Open License パートナー

### <a name="details"></a>詳細

2020 年、Microsoft は、クラウド ソリューション プロバイダー (CSP) プログラムを通じてパートナーとお客様が永続的ソフトウェア ライセンスを幅広くご利用いただけるようになることを[発表](https://blogs.partner.microsoft.com/mpn/general-availability-of-perpetual-software-licenses-in-the-cloud-solution-provider-program/)しました。 最初のマイルストーンには、商用の永続的ソフトウェア プランが利用可能になった 2021 年 1 月時点で到達しました。 次の主要なマイルストーンは、[公的機関](https://aka.ms/openlicensepublicsector)のプランが利用可能になる 2021 年 7 月に発生します。 2022 年 1 月 1 日より、Open License プログラムを通じてソフトウェア アシュアランスまたはオンライン サービスの新しいソフトウェア ライセンスの購入または更新を行えなくなる旨も[お伝えしました](https://blogs.partner.microsoft.com/mpn/expanding-opportunities-for-partners-in-the-cloud-solution-provider-program/)。

新しいコマース エクスペリエンスで永続的ソフトウェアを CSP プログラムに移行することで、パートナーはさまざまなソリューションやマネージド サービスを提供する機会を広げることができます。 これにより、お客様のクラウドへの移行も促進されます。  パートナーとお客様両方の円滑な移行を実現するために、こうした調整を行い、このデジタル変革を促進するための資料をご用意しました。

#### <a name="april-2021"></a>2021 年 4 月

[提供中](https://partner.microsoft.com/resources/collection/reseller-open-license-to-csp-transition-materials#/): リセラー向けの Open License から CSP への移行に関する資料

#### <a name="july-2021"></a>2021 年 7 月

##### <a name="csp"></a>CSP

- 7 月 1 日: 永続的ソフトウェア ライセンスを公的機関のお客様が利用可能に

- 7 月 7 日: Visual Studio Pro および Get Genuine Windows Agreement の永続的なソフトウェア ライセンスがすべてのセグメントで利用可能に

##### <a name="open-value"></a>オープン バリュー

- 7 月 1 日: 追加の SKU が教育および非営利向けの Open Value プログラムで利用可能に。Open License プログラムに似たプランを提供します。

##### <a name="open-license"></a>オープン ライセンス

- 7 月 1 日: Microsoft による Open License プログラムでの新しいプランの発表はなくなります。

#### <a name="january-2022"></a>2022 年 1 月

- 1 月 1 日: Open License プログラムで新しい購入や更新を行うことはできなくなります。

### <a name="next-steps"></a>次のステップ

#### <a name="csp-indirect-providers"></a>CSP 間接プロバイダー

今後数か月間で、パートナー コミュニティのイベントに参加し、リセラー向けの Open License から CSP への移行に関する資料を使用して、Open License リセラーの CSP プログラムへの移行を進めます。

- [リセラー向けの Open License から CSP への移行に関する資料](https://partner.microsoft.com/resources/collection/reseller-open-license-to-csp-transition-materials#/)—カスタマイズ可能な概要プレゼンテーション、電子メール テンプレート、CSP 間接リセラー オンボード ガイドなどを利用して、大規模なリセラーの導入を促進することができます。

- Microsoft Business Operations 主催の [CSP パートナー コミュニティ イベント](https://globalpbocomm.eventbuilder.com/GlobalCSP)。  さまざまなセッションに参加して、CSP の基本 (CSP の基礎) を確認したり、最新の情報を入手したり、Software in CSP に関する質問をしたり (Q&A セッション) することができます。

- (近日公開予定) Microsoft Business Operations 主催の CSP 間接リセラー向けトレーニング セッション。

#### <a name="open-license-resellers"></a>Open License リセラー

- 組織が現在 CSP プログラムに登録されていない場合は、開始方法について、ディストリビューターにお問い合わせください。 間接プロバイダーと[こちら](https://partner.microsoft.com/membership/cloud-solution-provider/find-a-provider)から連携できます。

- 組織が既に CSP プログラムに登録されている場合は、CSP の永続的ソフトウェアの詳細について、[こちら](https://partner.microsoft.com/resources/collection/software-in-csp)をご覧ください。

### <a name="questions"></a>疑問がある場合

これらのオファーについてさらにご質問がある場合は、関連する Yammer コミュニティをご確認ください。

________________
## <a name="now-live-global-promo-readiness-guide"></a><a name="6"></a>公開中: グローバル プロモーション準備ガイド

### <a name="categories"></a>Categories

- 日付: 2021 年 4 月 16 日
- 機能

### <a name="summary"></a>まとめ

Launch Readiness が、Operations Readiness リソース ギャラリーに[グローバル プロモーション準備ガイド](https://partner.microsoft.com/resources/detail/operations-promo-guide-pdf)を公開しました。 このガイドは、すべてのアクティブな[グローバル販売促進](https://partner.microsoft.com/resources/collection/global-promo-readiness-guide-collection#/)を統合的に表示します。

### <a name="impacted-audience"></a>対象

すべてのボリューム ライセンス (VL)、Dynamics Price List (DPL)、およびクラウド ソリューション プロバイダー (CSP) パートナー

### <a name="details"></a>詳細

Microsoft パートナーから、すべてのグローバル プロモーションとその詳細について統合されたビューを提供してほしいという要望がありました。 この統合ガイドを使用すると、利用可能なすべての情報に一元的かつ便利な場所で簡単にアクセスできるという安心感の中、プロモーションを利用できます。

2021 年 4 月から、Microsoft はこのガイドを毎月更新し、ガイドは Operations Readiness リソース ギャラリーの専用グローバル プロモーション準備ガイド コレクションで利用できるようになります。

このガイドへのリンクは、次のコレクションにも含まれます。

- [製品発表予定表コレクション](https://partner.microsoft.com/resources/collection/csp-announcement-calendar#/)。今後の変更や発表を一元的に表示できます。

- [コミュニティ コレクション](https://partner.microsoft.com/resources/collection/april-2021-csp-partner-community-content#/)。月次パートナー コールのサポート資料が含まれ、今後の変更や、運用上興味深いタイムリーなトピックを中心に扱います。

- [パートナー ニュースレター](https://partner.microsoft.com/resources/collection/csp-monthly-update#/)。CSP の月ごとの更新ニュースレター

毎月のリマインダーとして、グローバル プロモーション準備ガイドの最新刊と共に、パートナー センターのお知らせも公開されます。

### <a name="next-steps"></a>次のステップ

各月の開始時に、[Operations Readiness リソースギャラリー](https://partner.microsoft.com/resources)に最新の[グローバル プロモーション準備ガイド](https://partner.microsoft.com/resources/detail/operations-promo-guide-pdf)が掲載されます。

この情報を組織内の適切な担当者と共有し、各ページの最後の「このページは役に立ちましたか?」 ボタンを押して、ガイドがどのくらい役立ったかをお聞かせください。

________________
## <a name="april-cloud-solution-provider-csp-community-update-and-reminders"></a><a name="5"></a>4 月のクラウド ソリューション プロバイダー (CSP) コミュニティの更新とリマインダー

### <a name="categories"></a>Categories

- 日付: 2021 年 4 月 16 日
- コミュニティ | 招待とリマインダー

### <a name="summary"></a>まとめ

オンデマンドで利用できる CSP コミュニティ リソースは毎月更新されるため、常に最新情報を入手し、CSP プログラムの変更に備えることができます。

### <a name="impacted-audience"></a>対象

CSP 直接請求パートナーおよび間接プロバイダー

### <a name="details"></a>詳細

今月、リソースには、次の主要なトピックが含まれています。

- [CSP プログラムの進化の更新と Open License プログラムの変更](https://partner.microsoft.com/resources/collection/csp-open-evolution-to-a-better-experience#/)

- [特定の地域での CSP のお客様のオンボード要件の変更](https://partner.microsoft.com/resources/collection/additionalfields-csp-customers-selected-geos#/)

- [CSP プログラムでの新しいコマース PDF 請求書の新しい形式](https://partner.microsoft.com/resources/collection/introducing-new-format-for-the-new-commerce-invoice-in-csp#/)

[CSP コミュニティ コレクション](https://partner.microsoft.com/resources/collection/april-2021-csp-partner-community-content#/)には、以下が見つかります。

- ダウンロード可能な [CSP の月ごとの更新ニュースレター](https://partner.microsoft.com/resources/detail/csp-monthly-update-april-2021-global)。最近の CSP のお知らせ、更新プログラム、イベント、リマインダーを、読みやすいドキュメントに集計します。

- [CSP のお知らせカレンダー](https://partner.microsoft.com/resources/detail/csp-announcement-calendar-april-2021)。プログラムに影響を与える今後の変更のタイムライン ビューを提供します。

- 新しい[製品の発売予定表](https://partner.microsoft.com/resources/detail/product-launch-calendar-april-pdf)。今後の製品の発表とプランをご覧いただけます。

- [CSP 製品発表更新リソース](https://partner.microsoft.com/resources/collection/april-2021-csp-launch-topics-collection#/)には、主要な運用上の変更に関する簡単に使用できるコンテンツが含まれています。

- 関心や質問を受け付ける CSP の主要なトピックに関する[リフレッシャーとリマインダー](https://partner.microsoft.com/resources/detail/csp-april-2021-refreshers-and-reminders-pdf)。

#### <a name="csp-community-call-qas"></a>CSP コミュニティ コールに関する Q&A

コミュニティ コールの Q&A は、今後の変更に関する質問がある場合に役立ちます。 4 月、5 月、6 月に開催される CSP コミュニティ コールの Q&A に今すぐ登録しましょう。 ここでは、最新の発表、重要なリフレッシャー、リマインダーにフォーカスが置かれます。

[こちらからご登録ください](https://globalpbocomm.eventbuilder.com/GlobalCSP)。

### <a name="next-steps"></a>次のステップ

コミュニティのリソースを確認し、コミュニティ コールの Q&A に登録しましょう。

コミュニティ コールの Q&A を最大限に活用するには、オンデマンド コミュニティ コンテンツを確認し、電話の少なくとも 48 時間前までに質問をお送りください。

### <a name="questions"></a>わからないことがある場合は、

月次の CSP コミュニティ コール Q&A は、CSP プログラムの変更に関する質問がある場合に最適です。 毎月、お客様にとって最も重要なトピックにセッションを費やせるよう、資料を確認し、事前に質問をお送りください。

詳細については、[サポート](https://partner.microsoft.com/dashboard/support/csp/servicerequests/create?category=csp)にお問い合わせください。

________________
## <a name="final-reminder-deprecation-of-get-qualification-on-may-6-2021"></a><a name="4"></a>最後のリマインダー: 2021 年 5 月 6 日に GET 認定が非推奨化

### <a name="categories"></a>Categories

- 日付: 2021 年 5 月 4 日

- 機能

### <a name="impacted-audience"></a>対象

パートナー センター API を使用してクラウド ソリューション プロバイダー プログラムを通じて教育、非営利、Government Community Cloud (GCC) 向けのプランを販売しているパートナー様

### <a name="details"></a>詳細

この発表は、[12 月にリリースされたパートナー センター の機能強化](https://docs.microsoft.com/partner-center/announcements/2020-december#1)に関する補足です。 そのリリースの一部として、新しい GET および POST 認定 API が展開されました。その結果、**既存の GET 認定は 2021 年 5 月 6 日に廃止される予定です**。 その時点までに、新しい POST パートナー センター API を使用するように移行しておく必要があります。 新しい POST API を使用すると、教育機関向けプランを購入できます。一方、新しい GET API を使用すると、事前に資格要件が確認された非営利および GCC 向けプランを購入できます。

### <a name="next-steps"></a>次のステップ

- 適切かつタイムリーに移行できるよう、**新しい API に更新** してください。

- オペレーション レディネス リソースで、**新しいパートナー センター API に関する変更点とガイド** を確認してください: [パートナー センターの教育機関顧客検証プロセスの機能強化](https://partner.microsoft.com/resources/collection/partner-center-edu-validation-enhancements#/)。

- この情報を組織内の該当するチームと、およびリセラーと共有し、彼らがこれらの変更内容に対して準備できるようにしてください。

### <a name="questions"></a>わからないことがある場合は、

このお知らせに関してご質問がある場合は、[パートナー センター サポート](https://partner.microsoft.com/dashboard/support/referrals/servicerequests?category=referrals)にお問い合わせください。

### <a name="change-log"></a>ログの変更

- 2021 年 5 月 4 日: GET 認定の予定されている非推奨に関する最後のご案内

- 2021 年 4 月 9 日: GET 認定の予定されている非推奨に関するご案内 

- 2 月: GET と PUT の認定の非推奨に関するタイムラインを更新しました

- 1 月: GET と PUT の認定の予定されている非推奨に関するご案内

________________
## <a name="new-format-for-the-new-commerce-pdf-invoice-in-csp"></a><a name="3"></a>CSP での新しいコマース PDF 請求書の新しい形式

### <a name="categories"></a>Categories

- 日付: 2021 年 4 月 5 日
- 機能

### <a name="summary"></a>まとめ

Microsoft では、クラウド ソリューション プロバイダー (CSP) プログラムに新しいコマース PDF 請求書の新しい形式を導入中であり、SKU の説明ではなく製品の詳細ごとに請求の詳細を表示するようになります。

### <a name="impacted-audience"></a>対象

CSP プログラム経由で取引のあるパートナー様

### <a name="details"></a>詳細

2021 年 5 月以降、Microsoft では、CSP プログラムに新しいコマース PDF 請求書の新しい形式を導入し、SKU の説明ではなく製品の詳細ごとに請求の詳細を表示するようになります。 この新しい更新により、製品の種類ごとに品目が集計され、すべての製品が個別の行に表示されます。

パートナー様は、2021 年 4 月 1 日から 2021 年 4 月 30 日までの請求期間に対する 5 月の請求書でこの変更を目にすることになります。 影響を受けるオファーは、Microsoft Azure 予約インスタンス、Azure サブスクリプション (Azure プラン)、Marketplace です。

請求書の形式が更新された後に行われるクレジット再請求の要求は、新しい形式で生成されます。

#### <a name="partner-benefits"></a>パートナーの特典

この更新では、パートナー様への請求エクスペリエンスに関して次の点が改善されます。

- 重要なデータを保持したまま、請求書のサイズが削減されます

- 簡潔でユーザー フレンドリな請求書の業界標準の形式に従います 

次の要素は影響を受けません。

- 請求書 PDF の請求の概要ページ

- 既存の請求 API

- 調整ファイル (調整ファイルは詳細データを取得するために使用できます) 

- 使用量とライセンス ベースの料金の請求書

### <a name="next-steps"></a>次のステップ

このトピックの情報について、Microsoft パートナー Web サイトの [Operations Readiness リソース ギャラリー](https://partner.microsoft.com/resources/collection/introducing-new-format-for-the-new-commerce-invoice-in-csp#/)を参照してください。 請求リソース、請求書、CSP 請求、税金など、請求と税金のトピックに関する詳細は、パートナー センターの[請求セクション](https://docs.microsoft.com/partner-center/billing)を参照してください。

________________
## <a name="changes-to-the-cloud-solution-provider-csp-customer-onboarding-requirements"></a><a name="2"></a>クラウド ソリューション プロバイダー (CSP) のお客様のオンボード要件の変更

### <a name="categories"></a>Categories

- 日付: 2021 年 4 月 2 日
- 製品サービス/市場

### <a name="summary"></a>まとめ

パートナーと顧客が信頼に基づいて取引できるように支援する責任の一環として、Microsoft では 2021 年 3 月 25 日から、追加の顧客情報を要求いたします。

### <a name="impacted-audience"></a>対象

次のセクションに記載されている国に新規または既存の顧客がいる CSP 直接請求パートナーおよび間接プロバイダー

### <a name="details"></a>詳細

Microsoft の基盤は信頼です。 Microsoft は、CSP プログラムでの顧客サブスクリプションの取引について、顧客検証のための法令に準拠した安全な手段の提供に努めています。 2021 年 3 月 25 日に、パートナー センター API とユーザー インターフェイス (UI) の拡張機能を導入する予定です。これは、以下の条件の両方を満たすパートナーに影響します。

- Microsoft の間に直接請求関係があるパートナー (つまり、直接請求パートナーまたは間接プロバイダーのいずれかであるパートナー)

- パートナーは、次の国の新規または既存の顧客と取引があります:

    - タイ
    - ベトナム
    - トルコ
    - ポーランド
    - 南アフリカ
    - インド
    - ブラジル
    - イラク
    - ミャンマー
    - 南スーダン
    - サウジアラビア
    - アラブ首長国連邦
    - ベネズエラ

条件を満たすパートナーは、次にその顧客のサブスクリプションを更新または作成するときに、顧客の会社登録 ID (顧客の組織 INN とも呼ばれます) と電話番号を提出する必要があります。 また、これらのパートナーは、必要に応じて、顧客のミドル ネームを入力することができます。

会社登録 ID を追加する場合は、顧客の個人 ID ではなく、業務用の税 ID を使用する必要があることに注意してください。

以下の国で新規または既存の顧客との取引を行っているパートナーは、先行する 2020 年 11 月のリリースで既にオンボードされています。

- アルメニア
- アゼルバイジャン
- ベラルーシ
- ハンガリー
- カザフスタン
- キルギスタン
- モルドバ
- ロシア
- タジキスタン
- ウクライナ
- ウズベキスタン

その他の地域の顧客と提携しているパートナーは、2021 年 3 月の終わりに、顧客の会社登録 ID、電話番号、ミドル ネームを詳細情報として必要に応じて入力できるようになります。

### <a name="next-steps"></a>次のステップ

- 詳細なガイダンスについては、専用の[パートナー コレクション](https://partner.microsoft.com/resources/collection/additionalfields-csp-customers-selected-geos#/)でテクニカル ドキュメントとよく寄せられる質問を参照してください。
- パートナー センター API と Web ユーザー エクスペリエンスを使用して、変更を組み込む準備をしてください。 API または SDK はテストに使用できます。
- 新しい顧客をオンボードする場合や、既存の顧客の詳細情報を変更する場合は、必ず追加データを提出してください。
- コントロール パネル ベンダー (CPV) ソリューションを使用している場合は、CPV とご相談ください。

### <a name="questions"></a>わからないことがある場合は、

会社登録 ID (INN または TIN とも呼ばれます) に関するご質問がある場合は、税務顧問または現地の税務署にお問い合わせください。 Microsoft では、税務に関するガイダンスを提供できません。

Microsoft との連携でサポートが必要な場合は、[サービス要求](https://partner.microsoft.com/dashboard/support/servicerequests/create?stage=2&topicid=aa679372-d996-73df-e244-cb28bbbf28e8)を開いてください。

## <a name="view-this-months-product-launches-and-offers"></a><a name="1"></a>今月の製品の発表とオファーを見る

### <a name="categories"></a>Categories

- 日付: 2021 年 4 月 1 日
- 機能
 
### <a name="summary"></a>まとめ

2021 年 4 月の製品発表予定表が公開されました。

### <a name="impacted-audience"></a>対象

クラウド ソリューション プロバイダー (CSP) プログラムを通じて取引を行う、すべてのパートナー様

### <a name="details"></a>詳細

2021 年 4 月の[製品発表予定表](https://partner.microsoft.com/resources/collection/product-launch-calendar-collection#/) が、Operations Readiness リソース ギャラリーで入手できるようになりました。 こちらで今後予定されている製品の発表とオファーをご覧ください。

### <a name="next-steps"></a>次のステップ

[製品発表予定表](https://partner.microsoft.com/resources/collection/product-launch-calendar-collection#/)を確認し、この情報を組織内の該当する関係者と共有します。  

### <a name="questions"></a>わからないことがある場合は、

これらのオファーについてさらにご質問がある場合は、関連する Yammer コミュニティをご確認ください。
