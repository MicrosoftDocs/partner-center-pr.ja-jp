---
title: 2021 年 1 月のお知らせ
description: 2021 年 1 月の Microsoft パートナー センターのお知らせでは、新しい機能、販売促進、オファー、市場、既存のオファーに対する変更を紹介します。
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: brentserbus
ms.author: brserbus
ms.custom: announcement
ms.localizationpriority: high
ms.date: 01/15/2021
ms.openlocfilehash: 9b972354fb21dbdfa4780717cee54bac14acdb0e
ms.sourcegitcommit: 9bcccaf8864d8ee3c93e67691f773463f162b5f0
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/19/2021
ms.locfileid: "98571671"
---
# <a name="january-2021-announcements"></a>2021 年 1 月のお知らせ

このページでは、2021 年 1 月の Microsoft パートナー センターのお知らせについて詳しく説明します。

2021 年のお知らせ1 月

2020 年のお知らせ:[5 月](2020-may.md) | [6 月](2020-june.md) | [7 月](2020-july.md) | [8 月](2020-august.md) | [9 月](2020-september.md) | [10 月](2020-October.md) | [11 月](2020-november.md) | [12 月](2020-december.md)  

________________
## <a name="perpetual-software-now-generally-available-for-the-cloud-solution-provider-program"></a><a name="11"></a> クラウド ソリューション プロバイダー プログラムで永続的ソフトウェアが一般提供されるようになりました

### <a name="categories"></a>Categories

- 日付:2021 年 1 月 19 日
- ビジネスの拡大

### <a name="impacted-audience"></a>対象

すべての CSP パートナー

### <a name="details"></a>詳細

本日[お知らせ](https://blogs.partner.microsoft.com/mpn/general-availability-of-perpetual-software-licenses-in-the-cloud-solution-provider-program/)したように、CSP パートナーが販売する商用永続的ソフトウェア ライセンスが一般提供されるようになりました。 パートナー センターで CSP 永続的ソフトウェアの価格表が再公開され、追加の製品と地域が含まれるようになりました。

さらに、本日をもってパートナー センターのソフトウェアおよびライセンス キー フルフィルメント機能は廃止され、今後、パートナーと顧客は、この目的では Microsoft 365 管理センターを使用する必要があることにご注意ください。
詳細と次の手順については、以下を参照してください。

### <a name="next-steps"></a>次の手順

- パートナー センターの [[料金とプラン]](https://partnercenter.microsoft.com/en-us/pcv/sales) ページの **[ソフトウェア]** セクションにある **CSP の永続的ソフトウェア** の価格表をダウンロードします。 新しく追加された製品と地域の一覧については、[こちら](https://partner.microsoft.com/resources/detail/software-in-csp-new-products-geos-pdf)を参照してください。
- [Microsoft 365 管理センターの永続的ソフトウェアと製品ライセンス キーのダウンロードに関するハウツー記事](https://go.microsoft.com/fwlink/p/?linkid=2152525)を参照し、顧客がソフトウェアとライセンス キーをダウンロードする準備ができたときに顧客と共有してください。
- [クラウド ソリューション プロバイダー プログラムの永続的ソフトウェア](https://partner.microsoft.com/resources/collection/software-in-csp#/)準備資料を参照してください。 こちらの[レディネス マップ](https://partner.microsoft.com/resources/detail/software-in-csp-readiness-map-pdf)を利用すると、ロールに適した情報をすばやく見つけることができます。

### <a name="questions"></a>わからないことがある場合は、

さらにご質問がある場合は、関連する CSP Yammer コミュニティをご確認ください。

_____________
## <a name="reminder-introducingapithrottlingtopartners-calling-partner-centerapis"></a><a name="10"></a> リマインダー:パートナー センター API を呼び出すパートナーに対する API スロットリングの導入 

### <a name="categories"></a>Categories

- 日付:2021 年 1 月 19 日
- ビジネスの拡大

### <a name="summary"></a>まとめ

Microsoft は、パートナー センター API を呼び出すパートナーの特定の期間のパフォーマンスをさらに安定させることができるように、API スロットリングを導入します。

### <a name="impacted-audience"></a>対象

クラウド ソリューション プロバイダー (CSP) プログラムを通じて取引を行うすべてのパートナー  

### <a name="details"></a>詳細

2021 年 2 月、Microsoft は、パートナー センター API を呼び出すパートナーの特定の期間のパフォーマンスをさらに安定させることができるように、API スロットリングを導入します。 リソースの過剰な使用を防ぐため、スロットリングにより、ある期間におけるサービスの要求の数が制限されます。 スロットリングしきい値を超えた場合、パートナー センターにより、そのクライアントからのそれ以上の要求が一定期間制限されます。
  
**パートナー側のメリット:** パートナー センターは大量の要求を処理するように設計されていますが、少数のパートナーによって膨大な数の要求が行われた場合、すべてのパートナーに最適なパフォーマンスと信頼性を維持するために調整が役立ちます。  

- スロットリングによって、ダウンタイムが最小限に抑えられます。
- スロットリングによって大量の要求の数が削減され、すべてのパートナーに対して一貫したパフォーマンスが確保されるようになります。

**スロットリング対象の API:**

| 操作 | パートナー センターに関するドキュメント |
| ------ | ------- |
|{baseURL}/v1/customers/{customer_id}/subscriptions  | [顧客のすべてのサブスクリプションを取得する](/partner-center/develop/get-all-of-a-customer-s-subscriptions&data) |
|{baseURL}/v1/customers/{customer_id}/subscriptions/{subscription_id}  | [ID でサブスクリプションを取得する](/partner-center/develop/get-a-subscription-by-id) |
|{baseURL}/v1/customers/{customer_id}/orders  | [すべての顧客の注文を取得する](/partner-center/develop/get-all-of-a-customer-s-orders) |
|{baseURL}/v1/customers/{customer_id}/orders/{order_id}  | [ID ごとに注文を取得する](/partner-center/develop/get-an-order-by-id) |
|{baseURL}/v1/customers/{customer_id}/orders/{order_id}/provisioningstatus  | [サブスクリプションのプロビジョニング状態を取得する](/partner-center/develop/get-subscription-provisioning-status) |
|{baseURL}/v1/customers/{customer_id}/subscriptions/{subscription_id}  | [注文とサブスクリプションを管理する](/partner-center/develop/manage-orders#manage-a-subscription) |
|{baseURL}/v1/customers/{customer_id}/subscriptions/{subscription_id}/addons  | [サブスクリプションのアドオンの一覧を取得する](/partner-center/develop/get-a-list-of-add-ons-for-a-subscription) |
|{baseURL}/v1/customers/{customer_id}/subscriptions/{subscription_id}/azureEntitlements | [サブスクリプションの Azure エンタイトルメントの一覧を取得する](/partner-center/develop/get-a-list-of-azure-entitlements-for-subscription) |
|{baseURL}/v1/customers/{customer_id}/subscriptions/{subscription_id}/registrationstatus  | [サブスクリプションの登録状態を取得する](/partner-center/develop/get-subscription-registration-status) |
|{baseURL}/v1/customers/{customer-tenant-id}/transfers  | [顧客の譲渡をすべて取得する](/partner-center/develop/get-all-of-a-customer-s-transfers) |
|{baseURL}/v1/productUpgrades/{upgrade-id}/status  | [製品のアップグレード状態を取得する](/partner-center/develop/get-product-upgrade-status) |
|{baseURL}/v1/customers/{customer-id}/subscriptions/{subscription-id}/conversions   | [試用版の変換プランの一覧を取得する](/partner-center/develop/get-a-list-of-trial-conversion-offers) |
 
パートナーには、スロットリングされることがないように、アクティビティ ログ API を使用して効率化を検討することを強くお勧めします。 この機能の詳細については、 [こちら](/partner-center/develop/api-throttling-guidance)を参照してください。  

### <a name="next-steps"></a>次の手順

このトピックの [リソース](/partner-center/develop/api-throttling-guidance) を確認し、必要な手順を実行します。  

_____________

## <a name="security-compliance-and-identity-sci-launches-coming-on-february-1-2021"></a><a name="9"></a>2021 年 2 月 1 日、セキュリティ、コンプライアンス、および ID (SCI) を提供開始 

### <a name="categories"></a>Categories

- 日付:2021 年 1 月 15 日
- 製品サービス/市場

### <a name="summary"></a>まとめ

1 月の価格表のプレビューには Microsoft 365 のさまざまなサービスの開始が含まれ、2021 年 2 月 1 日から利用可能になります。

### <a name="impacted-audience"></a>対象

クラウド ソリューション プロバイダー (CSP) プログラムを通じて取引を行う、すべてのパートナー様

### <a name="details"></a>詳細

#### <a name="microsoft-365-g5-compliance-component-skus-for-government"></a>[行政機関向け Microsoft 365 G5 コンプライアンス コンポーネント SKU](/office365/servicedescriptions/microsoft-365-service-descriptions/microsoft-365-tenantlevel-services-licensing-guidance/microsoft-365-security-compliance-licensing-guidance)

Government Community Cloud (GCC) と GCC High の顧客向けに、3 つの新しいコンポーネント サービスの提供が開始され、2021 年 2 月 1 日から利用可能になります。 これらの SKU は、現在商用で利用可能な Microsoft 365 E5 Information Protection and Governance、M365 E5 Insider Risk Management、および Microsoft 365 E5 eDiscovery & Audit に相当します。 

   |**プラン名**|**プラン ID**|**マテリアル ID**|
   |-------------------|:------|:------|
   |Microsoft 365 E5 Information Protection and Governance for GCC|9e5397ab-f309-4d90-97f3-6fb5d53074d6|8QL-00002|
   |Microsoft 365 E5 eDiscovery and Audit for GCC|5c9ef884-6307-47e7-a914-f5092feae51e|8RI-00002|
   |Microsoft 365 E5 Insider Risk Management for GCC|11ccfdb3-80cb-4c80-8146-c9775045df17|8RF-00002|
   |GCC 向け Microsoft 365 E5 Information Protection and DLP (アドオン)|911d3177-53a9-42ec-a0e9-3b73fce527f0|8QY-00002|

#### <a name="10-year-audit-log-retention-add-on"></a>[監査ログを 10 年間保持するアドオン](/microsoft-365/compliance/)

Microsoft 365 E5 の必須ソフトウェアで利用可能なアドオンによって、顧客は、10 年間データを保持することができます。 

   |**プラン名**|**プラン ID**|**マテリアル ID**|
   |-------------------|:------|:------|
   |EDU 向けの監査ログを 10 年間保持するアドオン|879b5e1a-eaa2-4ea9-a628-0b429b2e8732|8LC-00002|
   |監査ログを 10 年間保持するアドオン|e14ce8d1-09f4-42d2-9b5e-ee85f32e7be4|8LB-00003|
   
#### <a name="frontline-worker-add-ons"></a>フロントライン ワーカーのためのアドオン

2021 年 2 月 1 日以降、顧客は、[Microsoft 365 F1 および F3 SKU](https://www.microsoft.com/microsoft-365/firstline-workers) のアドオンとして、フロントライン ワーカーのための 3 つの新しいセキュリティおよびコンプライアンス プログラム プランを購入できます。

これらのプログラム プランは、**2021 年 2 月 28 日** に終了する現在の[セキュリティおよびコンプライアンス](https://microsoft.sharepoint.com/teams/M365LicensingNews/SitePages/Security-and-Compliance-Promotion-for-Firstline-Workers-Update.aspx) プロモーションの後継となります。 現在のプロモーションとは異なり、これらの F5 アドオンによって、顧客は、最前線の従業員が増加するときの予測の予測可能性を高めることができます。

   
   |**プラン名**|**プラン ID**|**マテリアル ID**|
   |-------------------|:------|:------|
   |Microsoft 365 F5 Security|a8fba59e-1fc2-4658-8684-5f3d0c71c490|8RQ-00003|
   |Microsoft 365 F5 Compliance|6dc6cb1d-7bcb-4234-80cc-9c7a9cded044|8RL-00003|
   |Microsoft 365 F5 Security & Compliance|ad396924-ee4e-4059-b779-efe43dfa24d2|8RU-00003|
   
### <a name="next-steps"></a>次の手順

価格表のプレビューを確認し、組織の適切な関係者と共有してください。 詳細については、「[Microsoft のセキュリティとコンプライアンス - Microsoft Tech Community](https://techcommunity.microsoft.com/t5/microsoft-security-and/ct-p/MicrosoftSecurityandCompliance)」を参照してください。

### <a name="questions"></a>疑問がある場合

これらのオファーについてさらにご質問がある場合は、関連する Yammer コミュニティをご確認ください。 

_____________ 

## <a name="docusign-migration-to-adobe-sign-for-partners-under-microsoft-partner-agreements-mpas"></a><a name="8"></a>Microsoft Partner Agreement (MPA) に基づいたパートナー向けの Adobe Sign への DocuSign 移行 

### <a name="categories"></a>Categories

- 日付:2021 年 1 月 15 日
- 機能

### <a name="summary"></a>まとめ

Microsoft は、すべての電子署名処理を DocuSign から Adobe Sign に移行します。

### <a name="impacted-audience"></a>対象

MPA 下の既存の直接および間接のクラウド ソリューション プロバイダー (CSP) パートナー。 ウクライナ、ロシア、およびカザフスタンのパートナーは、毎年、物理的または電子的に Rider に再署名する必要があります。

### <a name="details"></a>詳細

2021 年 2 月、Microsoft は、CSP パートナーに対するすべての電子署名処理の DocuSign から Adobe Sign への移行を開始します。 

スムーズな移行が必要になります。 移行後は、電子署名が必要になるたびに、DocuSign ではなく adobesign@adobesign.com から電子メールが届きます。 この電子メールに、署名する必要がある Adobe Sign Web ページへのリンクが記載されています。 Microsoft パートナーは、既存の契約に再署名する必要はありません。今後のチャネル契約に限定されます。 

[リソース ギャラリー](https://partner.microsoft.com/resources/detail/adobe-sign-signature-request-email-pdf)で、Adobe Sign 署名要求電子メールの例を確認できます。 

**最適なエクスペリエンスを実現するために、次のことを必ず行ってください。**

1. このアカウントからの電子メールが迷惑メール フォルダーに直接送られないようにするために、差出人セーフ リストに adobesign@adobesign.com を追加します。
2. IT 部門と協力して、以下を実行します。
   - adobesign@adobesign.com 電子メール アドレスを差出人セーフ リストに追加して、事前設定されるフィッシング規則に含まれないようにします。
   - 既存のセキュリティ ポリシーを更新して、必要なすべての受信者が Adobe Sign エンタープライズ ライセンス下でドキュメントに署名できるようにします。

Adobe Sign は Microsoft の優先電子署名ソリューション (ESS) です。 Adobe Sign への移行により、安全で効率的な電子署名エクスペリエンスが保証され、お客様とパートナーにより大きな価値がもたらされます。

ドキュメントに電子的に署名する方法と電子署名の委任の詳細については、次の **チュートリアル** を参照してください。 
- [ドキュメントに電子的に署名する | Adobe Sign チュートリアル](https://helpx.adobe.com/sign/how-to/adobe-for-signers.html?playlist=/ccx/v1/collection/product/sign/segment/designer/explevel/beginner/applaunch/continuinged/collection.ccx.js&ref=helpx.adobe.com)
- [ドキュメントへの署名を委任する | Adobe Sign チュートリアル](https://helpx.adobe.com/sign/how-to/use-the-delegator-role.html?playlist=/ccx/v1/collection/product/sign/segment/designer/explevel/beginner/applaunch/orientation/collection.ccx.js&ref=helpx.adobe.com)

### <a name="next-steps"></a>次のステップ

この情報を組織内の適切な関係者に共有してください。

### <a name="questions"></a>疑問がある場合

質問がある場合は、[Call Logging Tool (CLT)](https://clt.partners.extranet.microsoft.com/CLT) を使用するか、[Explore MS](https://www.explore.ms/) で地域のオペレーション センターにお問い合わせください。 ご質問をできるだけ速やかに解決できるように、標準の CLT プロセスに注意深く従ってください。

_____________ 

## <a name="commercial-pricing-update-for-norwegian-krone"></a><a name="7">ノルウェー クローネでの商用価格の更新</a> 

### <a name="categories"></a>Categories

- 日付:2021 年 1 月 14 日
- 製品サービス/市場

### <a name="impacted-audience"></a>対象

ノルウェー クローネを使用するクラウド ソリューション プロバイダー パートナー。

### <a name="details"></a>詳細

2021 年 3 月 1 日以降、商用のオンプレミス ソフトウェアとオンライン サービスのノルウェー クローネ価格は、地域の市場価格と足並みを揃えるように変更されます。
完全なお知らせは、Microsoft パートナーのみご利用いただけます。 [完全なお知らせにアクセスするには、サインインしてください](https://partner.microsoft.com/resources/detail/pricing-update-norway-partners-pdf)。

_____________ 

## <a name="commercial-pricing-update-for-the-indian-rupee"></a><a name="6"></a>インド ルピーについて、商用顧客向け価格の更新 

### <a name="categories"></a>Categories

- 日付:2021 年 1 月 8 日
- 製品サービス/市場

### <a name="impacted-audience"></a>対象

インドで活動中の CSP パートナー。

### <a name="details"></a>詳細 

Microsoft は、インドおよびアジア地域における商用ソフトウェアとオンライン サービスの価格に合わせて、インド ルピーの価格表の変更を行っています。

完全なお知らせは、Microsoft パートナーのみご利用いただけます。 [完全なお知らせにアクセスするには、ログインしてください](https://partner.microsoft.com/resources/detail/price-update-indian-rupee.pdf)。

________________

## <a name="calling-plan-and-phone-system-updates-for-february-1-20201"></a><a name="5"></a>2021 年 2 月 1 日の通話プランおよび電話システムの更新

### <a name="categories"></a>Categories

- 日付:2021 年 1 月 8 日
- 製品サービス/市場

### <a name="summary"></a>まとめ

Microsoft 365 のアドオン プラン (電話システムと国内通話プラン、およびスタンドアロン国内通話プランが含まれます) が、近日中に一部の国向けに提供される予定です。

### <a name="impacted-audience"></a>対象

クラウド ソリューション プロバイダー (CSP) プログラムを通じて取引を行う、すべてのパートナー様。

### <a name="details"></a>詳細情報 

Microsoft 365 E1、E3、E5 プラン向けのアドオン バンドル プランには、電話システムと国内通話プランが含まれています。 さらに、E5 についてのみ、新しいスタンドアロン国内通話プランを使用できるようになります。 新しいプランは、米国、プエルトリコ、カナダのお客様にのみ提供されます。他のすべての国と地域については、既存のグローバル スタンドアロン SKU と価格のまま変わりません。 

これらのプランは、米国、プエルトリコ、カナダの商用、学生、教職員、Government Community Cloud (GCC)、および非営利団体のお客様が利用できます。 通話プランは、米国の他の準州では利用できません。

   |**プラン名**|**プラン ID**|**マテリアル ID**|
   |-------------------|:------|:------|
   |米国およびカナダ向け Microsoft Teams Calling Essentials|1ee81de6-4d8b-4cf1-b926-2fd2a774a4ca|8N2-00010|
   |米国およびカナダ向け Microsoft Teams Calling Essentials (非営利団体スタッフの価格)|0c2ece0d-39b7-40ec-8c08-87c2b6c75d62|8N2-00011|
   |米国およびカナダの教職員向け Microsoft Teams Calling Essentials|b8baa3b8-8cc2-4f26-a212-7fbeb28e7895|8N3-00003|
   |米国およびカナダの学生向け Microsoft Teams Calling Essentials|26956da8-eeb5-44e3-aa79-d36e0e42b930|8N3-00004|
   |米国およびカナダの GCC 向け Microsoft Teams Calling Essentials|7a2e2d5a-41b5-4b20-a0d1-0d06d34b5fe1|8N4-00002|
   |米国およびカナダ向け Microsoft 365 Domestic Calling Plan|60d2919e-427a-46c9-bd03-89cbad27d53f|TK2-00050|
   |米国およびカナダの教職員向け Microsoft 365 国内通話プラン|602e7548-375b-4e01-bf79-a9a8b8ff16d4|LM7-00006|
   |米国およびカナダの学生向け Microsoft 365 国内通話プラン|1f4b4375-3185-40cf-b044-117fe3b102c6|LM7-00007|
   |米国およびカナダの GCC 向け Microsoft 365 国内通話プラン|594ed84e-ddf8-4e40-9726-76c04bd29e3b|LM9-00023|

### <a name="next-steps"></a>次のステップ

- 組織内の関係者とこの情報を共有し、アップセルとクロスセルの機会を理解します。 
- [Teams パートナー ガイド](https://aka.ms/teamscallingmeetingsguide)のリソースに関するセクションを参照してください。

_____________ 

## <a name="license-base-price-list-updates-for-january-2021"></a><a name="4"></a>2021 年 1 月のライセンスベースの価格表の更新 

### <a name="categories"></a>Categories

- 日付:2021 年 1 月 8 日
- 製品サービス/市場

### <a name="summary"></a>まとめ

1 月と 2 月のライセンスベース プランの価格表が更新され、一部の誤った定価が修正されました。

### <a name="impacted-audience"></a>対象

クラウド ソリューション プロバイダー (CSP) プログラムを通じて取引を行う、すべてのパートナー様。

### <a name="details"></a>詳細情報 

2021 年 1 月と 2021 年 2 月のライセンスベースの価格表に、正しくない定価がいくつか含まれていました。 影響を受けるプランと通貨は次のとおりです。 正しい価格は、2021 年 1 月 7 日午後 2 時 PST (太平洋標準時) に更新されて、利用可能になりました。 

   |**プラン名**|**プラン ID**|**マテリアル ID**|
   |-------------------|:------|:------|
   |Microsoft 365 E3|2b3b8d2d-10aa-4be4-b5fd-7f2feb0c3091|AAA-35638| 
   |Microsoft 365 Business Basic|bd938f12-058f-4927-bba3-ae36b1d2501c|AAA-10624|

影響を受ける通貨: 

- Microsoft 365 E3 の価格の問題は、次の通貨のみに限られていました: JPY (日本円)、GBP (英国ポンド)、EUR (欧州連合)、AUD (オーストラリア ドル)。 
- Microsoft 365 Business Basic の問題は、USD (米国ドル) のみに限られていました。 

パートナーは、現在利用可能な 1 月と 2 月のプレビュー価格表で、正しい価格を参照する必要があります。 

### <a name="next-steps"></a>次のステップ

- パートナーは、パートナー センターから最新の価格表ファイルをダウンロードして、1 月と 2 月の修正された価格を入手する必要があります。 
- 影響を受けるテナントの、1 月 1 日から 1 月 6 日までの間にサブスクリプションを購入したグローバル管理者には、1 月末までに、パートナー センターからメールで詳細が通知されます。 

_____________ 

## <a name="euefta-change-of-partner-billing-currency-for-new-commerce-offers"></a><a name="3"></a> EU および EFTA での新しいコマース プランに関するパートナー請求通貨の変更

### <a name="categories"></a>Categories

- 日付:2021 年 1 月 7 日
- 機能

### <a name="impacted-audience"></a>対象

- EU および EFTA 地域のクラウド ソリューション プロバイダー プログラムを通じて取引を行うすべてのパートナー 

### <a name="details"></a>詳細

欧州連合 (EU) および欧州自由貿易協会 (EFTA) の地域では、クラウド ソリューション プロバイダー プログラムにおけるすべての新しいコマース オファーで、顧客の請求場所ではなく、パートナーの請求場所が使用されるようになります。 そのため、Microsoft による請求は、顧客の所在地の通貨ではなく、パートナーの所在地の通貨に基づいて行われれます。 これらの変更は、次の 2 つのフェーズで実行されます。

**フェーズ 1:**

- CSP で新しいコマース プランを購入した新しい顧客

- 既存の顧客による新しいコマース プランの初めての購入 - 2020 年 5 月 11 日より前に作成されたテナント

2021年 1 月 28 日以降、まったく新しい顧客が新しいコマース プランを購入するパートナー、または 2020 年 5 月 11 日より前にテナントを作成した既存の顧客が新しいコマース プランを初めて購入するパートナーには、それらの購入に対する請求がパートナーの場所の通貨で行われます。  

既存の顧客が CSP で新しいコマース プランを既に購入しているパートナーの場合は、このフェーズの間は、引き続き顧客の請求場所の通貨で課金されます。 さらに、テナントを 2020 年 5 月 11 日以降に作成した既存の顧客が、新しいコマース プランを初めて購入した場合、そのパートナーへの請求は引き続き顧客の通貨で行われます。

**フェーズ 2:**

- フェーズ 1 より前に CSP で新しいコマース プランを既に購入していた既存の顧客
- 既存の顧客による新しいコマース プランの初めての購入 - 2020 年 5 月 11 日以降に作成されたテナント

フェーズ 1 の後、2021 年を通して、Microsoft は、フェーズ 1 より前に CSP で新しいコマース プランを購入した既存の顧客、および 2020 年 5 月 11 日以降にテナントを作成した顧客がいるパートナーに対する新しいコマース プランの請求を、顧客の所在地の通貨から、パートナーの所在地の通貨に移行します。 パートナーには、この変更が実施される前に通知されます。

フェーズ 2 の後、EU および EFTA 地域のパートナーに対する、すべての顧客およびすべての CSP の購入についての請求は、パートナーの場所の通貨で行われます。

>[!NOTE]
>この変更による影響があるのはパートナーの請求通貨だけであり、CSP での新しいコマース プランの価格には影響ありません。 この変更の対象となる新しいコマース オファーは次のとおりです。Azure プランの一部である Azure のサブスクリプション、Azure の予約、サーバーのサブスクリプション、永続的なソフトウェア、およびクラウド ソリューション プロバイダー プログラムでの Microsoft コマーシャル マーケットプレースの購入。


### <a name="partner-benefits"></a>パートナーの特典

この更新により、EU/EFTA 地域における、新しいコマース エクスペリエンスでの複数の通貨による請求に関する複雑さとオーバーヘッドが軽減されます。

- パートナーは、1 つの通貨にまとめられた請求書を受け取るようになり、顧客の所在地の通貨ごとに請求書を受け取ることはなくなります
- インセンティブの支払いは、パートナーの請求書の通貨と同じ通貨で行われます
- パートナーは、複数の通貨での請求に伴う複雑さが軽減されるため、現在はアカウントの調整に取られている時間とリソースが解放されます
- 新しいコマース プランをまだ採用していないパートナーの場合、この変更により以前のパートナー請求モデルと一致するようになり、パートナーは CSP の新しいコマース エクスペリエンスにいっそう簡単に移行できます

### <a name="next-steps"></a>次のステップ

このトピックについての情報は、Microsoft パートナー Web サイトの[オペレーション ギャラリー](https://partner.microsoft.com/resources/collection/eu-efta-changes-collection#/) (サインインが必要) で確認してください。  

### <a name="questions"></a>わからないことがある場合は、

このお知らせに関する質問は、[パートナー センター サポート](https://partner.microsoft.com/dashboard/support/referrals/servicerequests?category=referrals) (サインインが必要) にお問い合わせください。

### <a name="change-log"></a>ログの変更

- 2020 年 11 月 17 日:初版の発行日
- 2021 年 1 月 7 日:フェーズ 1 およびフェーズ 2 に含まれる追加のシナリオ


________________
## <a name="deprecation-and-retirement-of-existing-get-and-put-qualification-apis-for-the-education-customer-validation-process-by-the-end-of-february-2021"></a><a name="2"></a>教育機関の顧客の検証プロセス用の、既存の GET および PUT Qualifications API が 2021 年 2 月末までに非推奨化および廃止

### <a name="impacted-audience"></a>対象

パートナー センター API を使用してクラウド ソリューション プロバイダー プログラムを通じてアカデミック向けオファーを販売しているパートナー様

### <a name="details"></a>詳細 

これは、2020 年 12 月にリリースされた API の機能強化に関する補足情報です。 2020 年 12 月に、新しい GET および POST Qualifications API がリリースされました。その結果、前の GET および PUT Qualifications API は、2021 年 2 月末までに廃止されます。 教育機関向け特価プランを購入できるようにするには、その時点で、新しい GET および POST パートナー センター API を使用する必要があります。 

### <a name="next-steps"></a>次のステップ

- これをまだ行っていない場合は、適切かつタイムリーに移行できるように、新しい API に更新してください。
- 以下をご確認ください: 新しいパートナー センター API の変更内容、および[ ガイド (オペレーション レディネス リソース:パートナー センターの教育機関顧客検証プロセスの機能強化)](https://partner.microsoft.com/resources/collection/partner-center-edu-validation-enhancements#/)。
- この情報を組織内の該当するチームやリセラーと共有し、これらの変更内容に対して準備できるようにします。

_____________

## <a name="dynamics-365-offers-for-february-2021"></a><a name="1"></a>2021 年 2 月の Dynamics 365 オファー

### <a name="categories"></a>Categories

- 日付:2021-01-04
- オファー

### <a name="summary"></a>まとめ

新しい Dynamics 365 オファーの変更が 2021 年 2 月に公開されます。

### <a name="impacted-audience"></a>対象

クラウド ソリューション プロバイダー (CSP) ダイレクト請求パートナー、間接プロバイダー、間接リセラー インセンティブ プログラムに参加しているパートナー

### <a name="details"></a>詳細

Microsoft では、2021 年 2 月に公開される新しい Dynamics 365 オファーの変更内容を発表します。

- Dynamics 365 Customer Voice Additional Response
- Dynamics 365 Customer Service Insights の有効期間終了
- Dynamics 365 Cloud AX 移行オファー ID の変更

**Dynamics 365 Customer Voice Additional Response**

2021 年 2 月 1 日に、Microsoft では 1-K の回答の権利を含む新しい "Additional Response" プランが作成されます。2-K の Survey Responses を含む既存のプランはそれと置き換えられ、2021 年 2 月 1 日に販売終了となる予定です。

SKU の詳細については、[Dynamics CSP オファー - 2021 年 2 月の Excel ドキュメント](https://partner.microsoft.com/resources/detail/dynamics-csp-offers-february-2021-xls)の [Customer Voice Addl Resp] タブをご覧ください。 詳細については、[Microsoft Dynamics 365 Customer Voice のホーム ページ](https://dynamics.microsoft.com/en-us/customer-voice/overview/)をご覧ください。

**Dynamics 365 Customer Service Insights の有効期間終了**

2021 年 2 月 1 日に、次の製品が有効期間終了に変更されます。

- Dynamics 365 Customer Service Insights ("Additional Cases" を含む)
- カスタマー サービス向け Dynamics 365 Virtual Agent

"Customer Service Insights" のスタンドアロン エクスペリエンスは "Dynamics 365 Customer Service" に移行し、顧客はそこでカスタマー サービス エクスペリエンスに完全に組み込まれている同じ機能を見つけることができます。  

SKU の詳細については、[Dynamics CSP オファー - 2021 年 2 月の Excel ドキュメント](https://partner.microsoft.com/resources/detail/dynamics-csp-offers-february-2021-xls)の [Customer Service Insights] タブをご覧ください。 詳細については、[Microsoft Dynamics Customer Service のホーム ページ](https://dynamics.microsoft.com/customer-service/overview/)にアクセスしてください。

**Dynamics 365 Cloud AX 移行オファー ID**

これらの SKU は、2021 年 1 月 1 日以降、最終的な価格表から削除されており、現時点では注文できません。 

   |**プラン名**|**プラン ID**|
   |-------------------|:------|
   |Dynamics 365 Finance for AX Migration Program|7fbd1115-a4c1-4cf9-b881-40c4187ca581|
   |Dynamics 365 Supply Chain Management for AX Migration Program|a3c62c0e-4f8a-4fc9-a47e-dec3310529d0|
   |Dynamics 365 Commerce for AX Migration Program|97e98de6-24a8-4282-bad6-9d1a874e90a4|
   |Dynamics 365 Finance Attach to Qualifying Dynamics 365 Base Offer for AX Migration Program|69d789e8-1e93-4dee-86b2-3ddfb03c08b9|
   |Dynamics 365 Supply Chain Management Attach to Qualifying Dynamics 365 Base Offer for AX Migration Program|c897adce-2964-4d24-abc3-7f7ad4b6a80d|
   |Dynamics 365 Commerce Attach to Qualifying Dynamics 365 Base Offer for AX Migration Program|ba1fe561-cfda-405a-a25d-ecda3bd3cba7|
   |Dynamics 365 Operations – Activity for AX Migration Program|177e954e-1fff-4941-8967-55a47e36e1ce|
   |Dynamics 365 Operations – Device for AX Migration Program|8c8b7c8f-cb3a-4737-8319-1752938c7be3|
   |Dynamics 365 Team Members for AX Migration Program|1eb3ad0b-9de3-419d-8bfe-0d61bdd945b2|

### <a name="next-steps"></a>次のステップ

このトピックに関するリソースを確認し、組織内の該当する関係者と共有してください。 

### <a name="questions"></a>疑問がある場合

これらのオファーについてさらにご質問がある場合は、関連する Yammer コミュニティをご確認ください。

________________
