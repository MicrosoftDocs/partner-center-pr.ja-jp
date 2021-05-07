---
title: 2021 年 3 月のお知らせ
description: 2021 年 3 月の Microsoft パートナー センターのお知らせでは、新しい機能、販売促進、オファー、市場、既存のオファーに対する変更を紹介します。
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: brentserbus
ms.author: brserbus
ms.custom: announcement
ms.localizationpriority: high
ms.date: 04/02/2021
ms.openlocfilehash: 17b8082b8a42050892ff434010952d5f91a39431
ms.sourcegitcommit: 6c20c3cc4a226cada70c56df295966696affcec8
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/30/2021
ms.locfileid: "108328068"
---
# <a name="march-2021-announcements"></a>2021 年 3 月のお知らせ

このページでは、2021 年 3 月の Microsoft パートナー センターのお知らせについて説明します。

## <a name="readiness-changes-to-the-cloud-solution-provider-csp-customer-address-validation-api-going-live-in-june-testing-capability-now-available"></a><a name="18"></a>準備状況: クラウド ソリューション プロバイダー (CSP) 顧客アドレス検証 API に対する変更が 6 月に運用開始、現在テスト機能が利用可能

### <a name="categories"></a>Categories

- 日付: 2021 年 4 月 30 日
- 準備

### <a name="summary"></a>まとめ

パートナーと顧客が信頼に基づいてビジネスを遂行できるようにするために、Microsoft はパートナーに対して世界中のすべての国の Validate Address API に対する変更をテストすることをお勧めしています。

### <a name="impacted-audience"></a>対象

顧客の住所の詳細を新規作成または既存のものを更新する、CSP 直接請求パートナーと間接プロバイダー。

### <a name="details"></a>詳細

Microsoft の基盤は信頼です。 Microsoft は、CSP プログラムで顧客サブスクリプションを処理するために、法令に準拠した安全な顧客住所の検証方法の提供に努めています。 2021 年 3 月 31 日の時点で、Validate Address API への変更が発表されています。2021 年 6 月にその変更を含む運用が開始される前にパートナーに対してこれをテストすることをお勧めしていました。

変更は、Validate Address API にのみ影響します。 Create Customer と Update Billing Profile の API には影響がありません。

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

住所が Validate Address API 経由で検証のために送信されると、次の応答スキーマが返されます。

```csharp

// <summary>
/// Object represents the address validation response.
/// </summary>

public class AddressValidationResponse
{
   /// <summary>
   /// Gets or sets the original address
   /// </summary>
   /// <value>
   /// Original Address
   /// </value>
   public Address OriginalAddress { get; set; }

   /// <summary>
   /// Gets or sets the suggested addresses
   /// </summary>
   /// <value>
   /// Suggested Addresses
   /// </value>
   public List<Address> SuggestedAddresses { get; set; }

   /// <summary>
   /// Gets or sets the validation status
   /// </summary>
   /// <value>
   /// Status
   /// </value>
   public string Status { get; set; }

   /// <summary>
   /// Gets or sets the validation message
   /// </summary>
   /// <value>
   /// Validation Message
   /// </value>
   public string ValidationMessage { get; set; }
   ```

サンプルの応答をご覧ください。 米国では、郵便番号に 5 桁の数字のみを入力した場合、応答では郵便番号の行に追加の 4 桁のサフィックスが返されることに注目してください。

```csharp

"suggested_address": {
              "Country": "US",
              "region": "WA",
              "city": "Redmond",
              "address_line1": "1 Microsoft Way",
              "postal_Code": "98052-8300"
},
"original_address": {
              "Country": "US",
              "region": "WA",
              "city": "Redmond",
              "address_line1": "1 Micro Way",
              "postal_Code": "98052"
},
"status":  "InteractionRequired",
"validation_message": "Address field invalid for property: ‘Street’"
}
```

### <a name="next-steps"></a>次のステップ

- テスト フライトに含められるようにサンドボックスのテナント ID を領域の専門家 (Ali Khaki) に知らせます。これにより、更新の準備を開始できます。

- コントロール パネル ベンダー (CPV) ソリューションを使用している場合は、CPV とご相談ください。

### <a name="questions"></a>わからないことがある場合は、

Microsoft との連携でサポートが必要な場合は、パートナー サポートの Yammer グループにお問い合わせください。

### <a name="change-log"></a>変更ログ:

- 2020 年 3 月 31 日: 初版の発行

- 2021 年 4 月 30 日: サンプルの応答と郵便番号の詳細について更新

________________
## <a name="new-exchange-admin-center-eac-experience"></a><a name="17"></a>新しい Exchange 管理センター (EAC) エクスペリエンス

### <a name="categories"></a>Categories

- 日付: 2021 年 3 月 29 日
- 機能

### <a name="summary"></a>まとめ

2021 年 4 月 27 日以降、Exchange 管理センター (EAC) では、ユーザーの日々の効率を向上させる新しいエクスペリエンスがロールアウトされます。

### <a name="impacted-audience"></a>対象

パートナー センター経由で Exchange にアクセスする代理管理者

### <a name="details"></a>説明

2021 年 4 月 27 日以降、パートナー センターを通じて Exchange に移動するパートナーは、新しい EAC にリダイレクトされます。

この新しいエクスペリエンスは現在、プレビューとして提供されており、管理者は従来の EAC で右上隅にあるトグルを選択すれば、このエクスペリエンスをアクティブにできます。 また、すべてのページに表示される [今すぐ試す] バナーを選択して、新しい EAC に移動することもできます。

新しい EAC には次のような利点があります。

- メール フロー関連の問題について、分析情報、レポート、アラートのメカニズムが追加されました。 

- ダッシュボードをカスタマイズして、生産性を向上させることができます。

新しいエクスペリエンスを簡単に確認するには、新しい EAC エクスペリエンスの「**トレーニングとガイド**」セクションでビデオを参照できます。 新しいポータルを最適に使用する方法の概要について理解できます。

>[!NOTE]
>この変更により、従来の EAC エクスペリエンスが非推奨になることはありません。 パートナーには、変更の実施に先立ち、十分前もって通知されます。

### <a name="next-steps"></a>次のステップ

- [このトピックに関するリソース](https://partner.microsoft.com/resources/collection/new-exchange-admin-center-experience#/)を参照して、新しいエクスペリエンスのスクリーンショットを確認することができます。

- この情報を組織内の適切な関係者に共有してください。 

### <a name="questions"></a>疑問がある場合

これらの変更についてさらにご質問がある場合は、関連する Yammer コミュニティをご確認ください。

________________
## <a name="microsoft-operations-introducing-the-product-launch-calendar"></a><a name="16"></a>Microsoft Operations: 製品発表予定表の概要

### <a name="categories"></a>Categories

- 日付: 2021 年 3 月 25 日
- 製品サービス | モダン ワークプレース

### <a name="summary"></a>まとめ

パートナーからのフィードバックにお応えして、Microsoft Operations では製品発表に関するコミュニケーションを合理化します。

### <a name="impacted-audience"></a>対象

クラウド ソリューション プロバイダー (CSP) パートナー様

### <a name="details"></a>詳細

Microsoft では、パートナー エクスペリエンスの継続的な改善に取り組んでいます。 Microsoft からの情報が多すぎるというフィードバックが寄せられています。これには、製品の発表に関する重複したお知らせも含まれます。

Microsoft では、皆様からのフィードバックにお応えして、新規および既存のオファーについて製品発表の準備エクスペリエンスを合理化しました。

現在では、月に 1 回の製品発表ビューを Operations Readiness リソース ギャラリーに提供するようになりました。 この月単位の[製品発表予定表ビュー](https://partner.microsoft.com/resources/collection/product-launch-calendar-collection#/)は、Operations Readiness リソース ギャラリーとパートナー センターのお知らせに含まれる個別の製品発表情報に置き換わるものとなります。

また、[コミュニティ コレクション](https://partner.microsoft.com/resources/collection/product-launch-calendar-collection#/)、[予定表ビュー](https://partner.microsoft.com/resources/assets#/?type=collection&search=Calendar&sort=updated)、[CSP ニュースレター](https://partner.microsoft.com/resources/collection/csp-monthly-update#/)から、この[製品発表予定表](https://partner.microsoft.com/resources/collection/product-launch-calendar-collection#/)にアクセスすることもできます。 各月の製品発表予定表が公開されたら、Operations Readiness リソース ギャラリーのお知らせで皆様に通知します。

新規および既存のオファーに関する情報は、今後も、価格一覧のプレビューと価格一覧の変更ログ、製品のブログ、ライセンス ガイド、製品マーケティング ページで確認できます。

この変更は、次の製品に関する発表に適用されます。

- オンプレミスの Dynamics
- Microsoft 365
- Microsoft Dynamics 365
- Windows
- サーバー  
- ツール
- Teams と Telco

Operations Readiness の詳細を必要とする製品の発表については、引き続き特定のお知らせをお送りします。

### <a name="next-steps"></a>次のステップ

このトピックに関するリソースを確認し、この情報を組織内の該当する関係者と共有してください。

### <a name="questions"></a>わからないことがある場合は、

これらのオファーについてさらにご質問がある場合は、関連する Yammer コミュニティをご確認ください。

________________
## <a name="changes-to-csp-customer-onboarding-requirements"></a><a name="15"></a>CSP のお客様のオンボード要件の変更

### <a name="categories"></a>Categories

- 日付: 2021 年 3 月 25 日
- 機能

### <a name="summary"></a>まとめ

パートナーと顧客が信頼に基づいて取引できるように支援する責任の一環として、Microsoft では 2021 年 3 月 25 日から、追加の顧客情報を要求いたします。

### <a name="impacted-audience"></a>対象

次のセクションに記載されている国に新規または既存の顧客がいるクラウド ソリューション プロバイダー (CSP) 直接請求パートナーおよび間接プロバイダー

### <a name="details"></a>詳細

Microsoft の基盤は信頼です。 Microsoft は、CSP プログラムでの顧客サブスクリプションの取引について、顧客検証のための法令に準拠した安全な手段の提供に努めています。 2021 年 3 月 25 日に、パートナー センター API とユーザー インターフェイス (UI) の拡張機能を導入する予定です。これは、以下の条件の両方を満たすパートナーに影響します。

1. Microsoft の間に直接請求関係があるパートナー (つまり、直接請求パートナーまたは間接プロバイダーのいずれかであるパートナー)

2. パートナーは、次の国の新規または既存の顧客と取引があります:

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

条件を満たすパートナーは、新しい顧客をオンボードするとき、または既存の顧客の詳細を変更するときに、顧客の **会社登録 ID** (顧客の **組織 INN** とも呼ばれます) と **電話番号** を提出する必要があります。 また、これらのパートナーは、必要に応じて、顧客の **ミドル ネーム** を入力することができます。

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

その他の地域の顧客と提携しているパートナーは、2021 年 3 月 25 日に、顧客の **会社登録 ID**、**電話番号**、**ミドル ネーム** を詳細情報として必要に応じて入力できるようになります。

### <a name="next-steps"></a>次のステップ

- 詳細なガイダンスについては、[専用のパートナー コレクション](https://partner.microsoft.com/resources/collection/additionalfields-csp-customers-selected-geos#/)でテクニカル ドキュメントとよく寄せられる質問を参照してください。

- Partner Center API と Web ユーザー エクスペリエンスを使用して、変更を組み込む準備をしてください。 API または SDK はテストに使用できます。

- 新しい顧客をオンボードする場合や、既存の顧客の詳細情報を変更する場合は、必ず追加データを提出してください。

- コントロール パネル ベンダー (CPV) ソリューションを使用している場合は、CPV とご相談ください。

### <a name="questions"></a>わからないことがある場合は、

有効な識別子 (INN または TIN とも呼ばれます) に関するご質問がある場合は、税務顧問または現地の税務署にお問い合わせください。 Microsoft では、税務に関するガイダンスを提供できません。

Microsoft との連携でサポートが必要な場合は、[サービス要求を開いてください](https://partner.microsoft.com/dashboard/support/servicerequests/create?stage=2&topicid=aa679372-d996-73df-e244-cb28bbbf28e8)。

________________
## <a name="corrections-made-to-march-1-2021-perpetual-software-price-list"></a><a name="14"></a>2021 年 3 月 1 日に永続的ソフトウェアの価格表に加えられた修正

### <a name="categories"></a>Categories

- 日付: 2021 年 3 月 23 日
- 製品サービス/市場

### <a name="impacted-audience"></a>対象

クラウド ソリューション プロバイダー プログラムで永続的なソフトウェアの取引を行っている間接プロバイダーおよび直接請求パートナー 

### <a name="details"></a>詳細

2021 年 3 月 1 日に公開された永続的ソフトウェアの価格表には、掲載されるべきではなかった市場が含まれていました。 修正内容を含めた永続的ソフトウェアの価格表が、2021 年 3 月 17 日に更新されました。 これらの修正は、次の場合にのみ適用されます。

- 製品 ID: DF77X4D43RKT 
- 製品名: Microsoft 365 Business の Windows 10 Home から Pro へのアップグレード
- 削除された、またはサポートされていない市場: AE、AF、AL、AM、AO、BA、BB、BD、BH、BM、BN、BO、BR、BS、BW、BY、BZ、CI、CL、CM、CO、CR、CW、DO、DZ、EC、EG、ET、FJ、FO、GE、GH、GT、HN、IL、IN、IQ、JM、JO、KE、KG、KN、KW、KY、KZ、LB、LK、LY、MA、MC、MD、ME、MN、MO、MU、NA、NG、NI、NP、OM、PA、PE、PH、PK、PR、PY、QA、RS、RU、RW、SG、SN、SV、TH、TJ、TM、TN、TT、TZ、UA、UG、UY、UZ、VE、VN、YE、ZM、ZW

これらの変更は、上記の製品にのみ適用されます。 他の製品には修正がありませんでした。 

### <a name="next-steps-and-resources"></a>次の手順とリソース

- 永続的ソフトウェアの取引を行うパートナーは、最新の永続的ソフトウェアの価格表をダウンロードする必要があります。
- 国を指す 2 文字の省略形のわかりやすいマッピングについては、[地域と国のコード](https://docs.microsoft.com/azure/marketplace/commercial-marketplace-co-sell-countries)を参照してください。
________________
## <a name="sdk-release-on-net-standard-v1170"></a><a name="13">.NET Standard (v1.17.0) の SDK リリース</a>

### <a name="categories"></a>Categories

- 日付: 2021 年 3 月 23 日

- 機能
 
### <a name="impacted-audience"></a>対象

パートナー センターの .NET SDK を使用している、CSP プログラムに参加している直接請求パートナーと間接プロバイダー。

### <a name="details"></a>詳細

2020 年 3 月 23 日より、パートナーは、更新されたパートナー センター SDK [GitHub の一般向けサンプル](https://github.com/Microsoft/Partner-Center-DotNet-Samples)と共に、[MicrosoftPartnerCenter.NETSDK (NuGet ギャラリー | Microsoft.Store.PartnerCenter 1.17.0)](https://www.nuget.org/packages/Microsoft.Store.PartnerCenter/1.17.0) バージョンのダウンロードを開始できます。 このバージョンには、以下のメソッドに対する更新が含まれています。

#### <a name="audit-updated-new-operation-types"></a>更新された監査: 新しい操作の種類

顧客が DAP を承認および終了した日時を把握するための、新しい[操作の種類](https://docs.microsoft.com/partner-center/develop/auditing-resources)が追加されました。

- DapAdminRelationshipApproved

- DapAdminRelationshipTerminated

#### <a name="audit-updated-new-resource-and-operation-types"></a>更新された監査: 新しいリソースと操作の種類

顧客ディレクトリ ロールのシナリオをサポートするための、新しい[リソースと操作の種類](https://docs.microsoft.com/partner-center/develop/auditing-resources)が追加されました。

- 新しいリソースの種類 "CustomerDirectoryRole"

- 操作の種類 "AddUserMember" と "RemoveUserMember"

#### <a name="sdk-updates-to-customer-accounts"></a>顧客アカウントに対する SDK の更新

- GET のサポート /customers/{customer-tenant-id}/directSignedMicrosoftCustomerAgreementStatus

- GET /customers/{customer-tenant-id}/qualifications

- POST /customers/{customer_id}/qualifications?code={validationCode}

#### <a name="additional-changes"></a>追加の変更

新しいコマースの一部として導入された次の変更は、現在、M365 または D365 の新しいコマース エクスペリエンスのテクニカル プレビューに含まれているパートナーのみが、招待に基づいて利用できます。 新しいコマースのテクニカル プレビューに含まれていないパートナーは、影響を受けないようにして、下位互換性を確保する必要があります。

- カタログの変更:

  - GET /products/{product-id}/skus/{sku-id}

- 購入および管理:
  - GET /customers/{customerId}/subscriptions
  - GET /customers/{customerId}/subscriptions/{subscriptionId}
  - PATCH /customers/{customerId}/subscriptions/{subscriptionId}
  - GET /customers/{customerId}/subscriptions/{subscriptionId}/transitioneligibilities
  - GET /customers/{customerId}/subscriptions/{subscriptionId}/transitions
  - POST /customers/{customerId}/subscriptions/{subscriptionId}/transitions

### <a name="next-steps"></a>次の手順

- 最新バージョン [MicrosoftPartnerCenter.NETSDK (NuGet ギャラリー | Microsoft.Store.PartnerCenter 1.17.0)](https://www.nuget.org/packages/Microsoft.Store.PartnerCenter/1.17.0) をダウンロードする
- [GitHub サンプル](https://github.com/Microsoft/Partner-Center-DotNet-Samples)をダウンロードして確認する

________________
## <a name="csp-commercial-marketplace-offer-and-fy21-csp-incentives-for-eligible-offers"></a><a name="12"></a>CSP コマーシャル マーケットプレース プランと、対象となるプランの FY21 CSP インセンティブ

### <a name="categories"></a>Categories

- 日付: 2021 年 3 月 18 日
- 機能

### <a name="impacted-audience"></a>対象

クラウド ソリューション プロバイダー プログラムにおける間接プロバイダーと直接請求パートナー 

### <a name="details"></a>詳細

クラウド ソリューション プロバイダー プログラムにおける間接プロバイダーおよび直接請求パートナーは、サードパーティのプランを販売できます。また、パートナー センターまたは Azure portal でトランザクションが実行された、対象となるサードパーティのプランごとにリベート インセンティブを獲得することができます。 インセンティブは、対象となるプランの請求済み売上に対するリベートの形式であり、**2021 年 6 月 30 日まで利用可能** です。  

この CSP コマーシャル マーケットプレース プランのインセンティブについて、以下で引き続き学習してください。顧客に今すぐ連絡して、継続的な成功とデジタル変革を実現するための適切なプランを特定してください。

Microsoft では、独立系ソフトウェア ベンダー (ISV) と提携して、Microsoft 顧客向けの最新の IaaS および SaaS ソリューションを市場に投入しています。 ISV 発行者は、Microsoft パートナー チャネルを通じたプランの販売を有効にすることができます。 インセンティブの対象となるプランは、次の 2 つのカテゴリに分類されます。

- Azure IP 共同販売インセンティブ対象ステータスを持つ、SaaS と IaaS のサードパーティ プランを選択する。 

- Teams、または少なくとも 2 つの Microsoft 365 生産性向上アプリ (PowerPoint、Word、Excel、Outlook、SharePoint など) で統合された SaaS アプリケーション。

### <a name="next-steps-and-resources"></a>次の手順とリソース

- 対象となるマーケットプレース アプリやインセンティブ対象アプリを販売する場合の[パートナー インセンティブ](https://partner.microsoft.com/membership/partner-incentives)の獲得について確認してください。 新しいプランは毎月追加されます。  
- [クラウド ソリューション プロバイダーの直接請求パートナー インセンティブ リソース](https://partner.microsoft.com/asset/collection/cloud-solution-provider-direct-partner-incentive-resources#/)
- [クラウド ソリューション プロバイダーの間接プロバイダー インセンティブ リソース](https://partner.microsoft.com/asset/collection/cloud-solution-provider-indirect-provider-incentive-resources#/)
- この[プレゼンテーション](https://partner.microsoft.com/resources/detail/partner-center-cm-for-csp-overview-pdf)を確認して、コマーシャル マーケットプレース アプリの販売に関する詳細を確認してください。 その他のリソースについては、[こちら](https://partner.microsoft.com/resources/collection/partner-center-cm-for-csp-collection#/)を参照してください。 
- [パートナー センター](https://docs.microsoft.com/partner-center/csp-commercial-marketplace-discover)または [Azure portal](https://ms.portal.azure.com/#home) でコマーシャル マーケットプレース カタログを探索する
- [API](https://docs.microsoft.com/partner-center/develop/create-subscription-azure-marketplace-products#get-a-list-of-offers-for-a-market) 使用して、会社のマーケットプレースにアプリを統合する
- 取引を行いたい ISV に連絡する
- 間接プロバイダーは API を使用して統合し、販売するアプリについてリセラーに指示する必要があります

### <a name="questions"></a>疑問がある場合  

パートナー センターのコマーシャル マーケットプレースの概要については、[この記事](https://docs.microsoft.com/partner-center/csp-commercial-marketplace-overview)を参照してください。

さらにサポートが必要な場合は、パートナー センターでサポート リクエストを作成できます。 詳細については、[https://aka.ms/IncentivesSupport](https://partner.microsoft.com/dashboard/support/servicerequests/create?stage=1) をご覧ください。

________________
## <a name="power-bi-premium-offer-naming-and-prerequisite-update"></a><a name="11"></a>Power BI Premium プランの名前と前提条件の更新

### <a name="categories"></a>Categories

- 日付: 2021 年 3 月 18 日
- 機能

### <a name="summary"></a>まとめ

2021 年 4 月 1 日の最終的な価格表は、Power BI Premium Per User の名前や前提条件の情報を明確にするために更新されます。

### <a name="impacted-audience"></a>対象

クラウド ソリューション プロバイダー (CSP) の直接および間接のパートナー

### <a name="details"></a>詳細

2021 年 4 月 1 日の最終的な価格表は、Power BI Premium Per User の名前や前提条件の情報を明確にするために更新されます。

最終的な価格表が更新されるまで、このセクションの情報を使用して、正しい製品が注文されていることを確認してください。

次の詳細は、影響を受ける SKU と前提条件の詳細を示しています。

| 3 月 1 日の価格表プレビューでのプラン表示名 |  4 月 1 日の最終的な価格表での更新されたプラン表示名| プラン ID |
| ------ | ----------- | ----------- |
| Power BI Premium Per User アドオン (非営利団体職員向けの価格)  |  Power BI Premium Per User アドオン **(Office)** (非営利団体職員向けの価格)   | 31c03289-47ab-4ab0-8df1-03742c127ac6   |

このプランを購入するには、次のいずれかの前提条件が満たされている必要があります。

| プラン表示名 | プラン ID |
| ------ | ----------- |
| Microsoft 365 E5 (非営利団体職員向けの価格)  |  31bedf01-9e57-4ece-a53a-d3656a563931   |
|   オーディオ会議なしの Microsoft 365 E5 (非営利団体職員向けの価格)|  b456810a-c414-4e07-98fc-ef74e8175a09|
|   Office 365 E5 (非営利団体職員向けの価格)| ce139fe5-8bd5-47ed-a5be-07c286f8b9e    |
|   Office 365 E5 (非営利団体職員向けの価格) 試用版|  2f192efe-608a-4c9c-9d19-2b0b70b0962e|
|   オーディオ会議なしの Office 365 E5 (非営利団体職員向けの価格)|  c3897426-9f49-4eaf-9b4d-7d9a1c72aef7|

次の Power BI Premium プランには、購入に必要な前提条件があります。

| プラン表示名 | プラン ID |
| ------ | ----------- |
|   Power BI Premium Per User アドオン (非営利団体職員向けの価格)|  ef0b895b-681b-4026-a5b1-dda182a57d40 |

このプランを購入するには、この前提条件が必要です。

| プラン表示名 | プラン ID |
| ------ |----------|
| Power BI Pro (非営利団体職員向けの価格)  |   cabdfc93-5786-4224-bfd3-35d58f833b35 |

### <a name="next-steps"></a>次のステップ

このトピックに関するリソースを確認し、この情報を組織内の該当する関係者と共有してください。  

### <a name="questions"></a>疑問がある場合

これらのプランについてさらにご質問がある場合は、関連する Yammer コミュニティをご確認ください。 

## <a name="march-price-updates-for-microsoft-365-f3"></a><a name="10"></a>Microsoft 365 F3 の 3 月の価格更新

### <a name="categories"></a>Categories

- 日付: 2021 年 3 月 16 日
- 製品サービス/市場

### <a name="summary"></a>まとめ

Microsoft 365 F3 のイギリス ポンド (GBP) とユーロ (EUR) では、2021 年 3 月の正しくない価格が修正されました。

### <a name="impacted-audience"></a>対象

クラウド ソリューション プロバイダー (CSP) プログラムを通して、2021 年 3 月 1 日から 3 月 17 日までの間に Microsoft 365 F3 を GBP または EUR で購入したパートナー。

### <a name="details"></a>詳細

Microsoft は Microsoft 365 F3 の価格が正しくなかった問題を解決しました。 GBP と EUR の価格が正しくありませんでした。2021 年 3 月 1 日から 3 月 17 日の間に購入したプランのみが対象となります。 影響を受けるプランと通貨は次のとおりです。 

| プラン名 | Currency | プラン ID | マテリアル ID |
| ------ |----------- |----------- |----------- |
| Microsoft 365 F3 (非営利団体) | GBP | 57b722c2-c435-4bfb-9bc8-80509213a13a | AAD-11626 |
| Microsoft 365 F3 (商用) | EUR| 3451a3b0-8cda-44a7-bad7-c30be81c4aaa | AAA-89898 |
 
3 月および 4 月のプレビューのライセンスベースの価格表は、3 月 16 日午後 5 時 (太平洋標準時) に更新されました。

### <a name="next-steps"></a>次のステップ

- パートナーは、3 月と 4 月のプレビューの両方の現在のライセンスベースの価格表をもう一度ダウンロードし、該当する場合はこれらの価格を修正する必要があります。  
- Microsoft は、今後数週間にわたって影響を受けたパートナーにメールで連絡し、影響を受けるトランザクションの修正に関連する今後の手順について通知します。

### <a name="questions"></a>わからないことがある場合は、

さらにご質問がある場合は、関連する CSP Yammer コミュニティをご確認ください。

________________

## <a name="update-a-legal-company-name-through-partner-center"></a><a name="9"></a>パートナー センターでの会社正式名称の更新

### <a name="categories"></a>Categories

- 日付: 2021 年 3 月 16 日
- 効率とスケールの向上

### <a name="summary"></a>まとめ

2021 年 3 月から、Microsoft Partner Network (MPN) パートナーとクラウド ソリューション プロバイダー (CSP) 間接リセラーは、パートナー センターで会社の正式名称を更新できます。

### <a name="impacted-audience"></a>対象

MPN パートナーと CSP 間接リセラー (CSP 直接請求パートナーは対象外です)

### <a name="details"></a>詳細

2021 年 3 月から MPN パートナーと CSP 間接リセラーは、パートナー センターで、規則に従って、セルフ サービス方式で、会社の正式名称を更新できます。 この新機能により、パートナーは社名を更新するためにパートナー センター サポート チケットを提出する必要がなくなります。 これにより、パートナーはこれらの操作を行う際の時間をかなり節約することができます。 

詳細については、「[法的ビジネスプロファイルを更新する](../update-your-partner-profile.md#update-your-legal-business-profile)」を参照してください。

>[!NOTE]
>企業の公式プロファイルの社名に誤字や略式表記がないこと、会社の正式な登録情報と完全に一致していることを確認してください。 組織プロファイル更新の詳細は[組織プロファイルの有効性を確認する](../update-your-partner-profile.md#update-your-legal-business-profile)に関するページを参照してください。

### <a name="next-steps"></a>次の手順

担当チームが手続きの見直し、更新を実施できるよう、この情報を組織で共有してください。

### <a name="questions"></a>ご質問がある場合は、

さらにご質問がある場合は、関連する CSP Yammer コミュニティをご確認ください。

________________
## <a name="update-to-cloud-solution-provider-csp-program-evolution-and-open-license-program-changes"></a><a name="8"></a>クラウド ソリューション プロバイダー (CSP) プログラムの進歩とオープン ライセンス プログラムの変更に関する最新情報

### <a name="categories"></a>Categories

- 日付: 2021 年 3 月 15 日
- 機能

### <a name="summary"></a>まとめ

オープン ライセンス プログラムの変更に伴い、商用および公的機関向けの新しい永続ライセンス ソフトウェア商品を、クラウド ソリューション プロバイダー (CSP) プログラムに追加します。

### <a name="impacted-audience"></a>対象

オープン ライセンス プログラムを通じて販売を行っている商業ディストリビューターと管理下のリセラー、および、永続ライセンス ソフトウェアの取引を行っているすべての CSP パートナー

### <a name="details"></a>詳細

2020 年 9 月、Microsoft はデジタル化推進の一環として、CSP プログラムのパートナーにビジネス機会を提供するための一連の方策を[発表しました](https://blogs.partner.microsoft.com/mpn/expanding-opportunities-for-partners-in-the-cloud-solution-provider-program/)。一例として、パートナーはオンプレミスのソフトウェアを使用できるようになりました。 これらの変更により、パートナーは CSP のソフトウェア ライセンスを利用してビジネスを成長させ、リーチを広げることができ、クラウド ファーストである現環境での成功を期待できます。 これはまた、顧客のクラウド移行をサポートし、顧客のハイブリッド クラウド環境の運用に求められる柔軟性をパートナーに与えます。

こうしてデジタル化を推し進める中で、Microsoft は次の変更を発表しました。

- 2021 年 7 月 1 日: 新たな SKU、製品、販促物をオープン ライセンス プログラムの価格表に追加することを中止します。

- 2021 年 7 月 7 日: Get Genuine Windows と Visual Studio Professional の 2 商品、および公的機関 (政府、教育機関、NPO。[発表](./2020-december.md#9)をご確認ください) 向けオファーを CSP 永続ライセンス ソフトウェアの価格表に追加します。  価格表はパートナー センターの [[Sell]\(販売\) > [Pricing & Offers]\(価格とオファー\)](https://partnercenter.microsoft.com/pcv/sales) ページの [ソフトウェア] セクションで閲覧できます。この価格表はこの日に改定する予定です。

CSP プログラムの進歩とオープン ライセンス プログラムの変更の詳細は、下の「**次のステップ**」をご覧ください。

### <a name="next-steps"></a>次のステップ:

- CSP プログラムの進歩: 準備資料[クラウド ソリューション プロバイダー プログラムの永続ライセンス ソフトウェア](https://partner.microsoft.com/resources/collection/software-in-csp#/)をご確認ください。 こちらの[レディネス マップ](https://partner.microsoft.com/resources/detail/software-in-csp-readiness-map-pdf)を利用すると、ロールに適した情報をすばやく見つけることができます。

- オープン ライセンス プログラムの変更: 準備資料[ CSP プログラムの進歩とオープン ライセンス プログラムの変更](https://partner.microsoft.com/resources/collection/csp-open-evolution-to-a-better-experience#/)をご確認ください。 こちらの[レディネス マップ](https://partner.microsoft.com/resources/detail/csp-open-evolution-to-a-better-experience-readiness-map-pdf)を利用すると、ロールに適した情報をすばやく見つけることができます。

### <a name="questions"></a>質問

さらにご質問がある場合は、関連する CSP Yammer コミュニティをご確認ください。

_______________
## <a name="update-to-a-previous-announcement-premium-assessments-an-add-on-to-compliance-manager"></a><a name="7"></a>以前の発表に関する最新情報: Compliance Manager のプレミアム評価アドオン

### <a name="categories"></a>Categories

- 日付: 2021 年 3 月 15 日
- ビジネスを拡大する

### <a name="summary"></a>まとめ

オファーの試用版は価格表に掲載しないことになっており、今後削除する予定です。

### <a name="impacted-audience"></a>対象

クラウド ソリューション プロバイダー プログラムで取引を行うパートナー

### <a name="details"></a>詳細

オファーの試用版は価格表に掲載しないことになっています。 これらは 2021 年 5 月 1 日の価格表から削除します。

元の発表は[こちら](./2021-february.md#4)でご覧いただけます。

### <a name="additional-resources"></a>その他のリソース

- [Microsoft 365 E5 のセキュリティとコンプライアンス](https://www.microsoft.com/licensing/product-licensing/microsoft-365-enterprise?activetab=m365-enterprise:primaryr5)

- [Microsoft コンプライアンス マネージャーでの評価の作成と管理 - Microsoft 365 コンプライアンス](/microsoft-365/compliance/compliance-manager-assessments)

### <a name="next-steps"></a>次のステップ

このトピックに関するリソースを確認し、この情報を組織内の該当する関係者と共有してください。

### <a name="questions"></a>疑問がある場合

これらのオファーに関するご質問については、Yammer の関連コミュニティをご確認ください。

________________
## <a name="migrate-your-solutions-from-one-commercial-partner-ocp-go-to-market-gtm-to-the-microsoft-commercial-marketplace"></a><a name="6"></a> One Commercial Partner (OCP) Go-to-Market (GTM) から Microsoft コマーシャル マーケットプレースにソリューションを移動する

### <a name="categories"></a>Categories

- 日付: 2021 年 3 月 12 日
- 機能

### <a name="summary"></a>まとめ

2021 年 3 月 29 日から One Commercial Partner (OCP) Go-to-Market (GTM) の機能を制限します。 パートナー センターのコマーシャル マーケットプレースにソリューションを移動することを推奨します。

### <a name="impacted-audience"></a>対象

OCP GTM のソリューションを使用して共同販売を行っている組織

### <a name="details"></a>詳細

Microsoft は 2020 年 12 月に、Microsoft OCP GTM ツールからパートナー センターの Microsoft コマーシャル マーケットプレースへの移行を開始しました。 この移行によってコマーシャル マーケットプレースの機能を拡張します。これは、皆様のソリューションを何百万もの顧客に紹介し、Microsoft や他のパートナー販売者と相互にビジネス機会を共有し、革新的なソリューションを共同販売できるプラットフォームです。

移行の次のステップは 2021 年 3 月 29 日に実施します。 そのときに、OCP GTM の機能の制限を開始し、一部のサービスは閲覧しかできなくなります。 現在 OCP GTM のソリューションを使用して共同販売を行っている場合、ソリューションをコマーシャル マーケットプレースに移動することを推奨します。それによって、この機能を利用できるようになり、公開作業も単純化できます。 

コマーシャル マーケットプレースに移行すると、共同販売する商品は主としてパートナー センターで公開することになります。 そこでは、Microsoft が採用している共通の販路と製品内部の仕組みを通じて皆様のソリューションを共通の顧客に紹介することで、引き続きビジネスを成長させることができます。 [コマーシャル マーケットプレースの詳細](https://blogs.partner.microsoft.com/mpn/getting-started-with-the-microsoft-commercial-marketplace/)。

### <a name="next-steps"></a>次の手順

- まだソリューションを移動させていない場合、[移行ガイド](/azure/marketplace/co-sell-solution-migration)に詳述された手順に従うか、[ステップ バイ ステップの動画チュートリアル](https://partner.microsoft.com/asset/detail/ocp-gtm-to-the-microsoft-commercial-marketplace-mp4)を見て移動作業を完了し、コマーシャル マーケットプレースでソリューションの公開を始めてください。

- OCP GTM の機能の制限に関するご質問については [Microsoft コマーシャル マーケットプレース共同販売公開要件 FAQ](https://partner.microsoft.com/resources/detail/co-sell-requirements-publish-commercial-marketplace-faq-pdf) に関するページをご覧ください。 (2021 年 3 月 29 日に始まる OCP GTM の機能の制限に関するセクションをお読みください。)

### <a name="questions"></a>疑問がある場合

ご質問がある場合、詳しく知りたい場合は[サポート](https://partner.microsoft.com/support/?stage=1)にお問い合わせください。

________________
## <a name="expanding-the-new-commerce-experience-in-the-cloud-solution-provider-csp-program-for-azure-to-russia"></a><a name="5"></a>クラウド ソリューション プロバイダー (CSP) プログラムの Azure 取引新サービスをロシアに拡大

### <a name="categories"></a>Categories

- 日付: 2021 年 3 月 10 日
- 機能

### <a name="impacted-audience"></a>対象

クラウド ソリューション プロバイダー (CSP) プログラムを通じてロシアで取引を行うすべてのパートナー。

### <a name="details"></a>詳細

2021 年 3 月 10 日から **CSP の Azure 取引新サービスをロシアで利用** できるようになります。 このサービスにより、顧客が Azure のサービスを購入、使用する方法を効率化し、改善します。 また、CSP プログラムのパートナーは、さまざまな販売状況を通じて Azure の料金を安定的に見通し、国際的目安として米ドルでの料金を把握し、請求日をそろえ、Azure Cost Management にアクセスできるようになります。

### <a name="next-steps"></a>次の手順

Azure の新しい取引サービスを紹介し、追加的な情報を提供する資料をいくつか用意しています。 最新の FAQ、プレゼン資料、動画、その他の資料を [CSP プログラム最新情報資料ギャラリー](https://partner.microsoft.com/resources/collection/new-azure-experience-in-csp#/)で見付けてください。

________________
## <a name="partner-center-software-license-key-and-download-fulfillment"></a><a name="4"></a>パートナー センター ソフトウェア ライセンス キーとダウンロード フルフィルメント

### <a name="categories"></a>Categories

- 日付: 2021 年 3 月 4 日
- 機能

### <a name="summary"></a>まとめ

パートナー センターのソフトウェア ダウンロードおよびライセンス キー フルフィルメント機能が復元されました。

### <a name="impacted-audience"></a>対象

パートナー センターを通じて永続的およびサーバーのサブスクリプション ソフトウェアの注文を処理しているすべてのクラウド ソリューション プロバイダー (CSP) パートナー

### <a name="details"></a>詳細

パートナーからのフィードバックに応えて、永続的およびサーバーのサブスクリプション ソフトウェアの注文に対してソフトウェアとライセンス キーを取得するパートナー センターのフルフィルメント機能を復元しています。 2021 年 1 月 19 日に削除される前の状態に復元されます。 ([お知らせ](2020-september.md#17)を参照してください。)

ソフトウェア ライセンス キーとダウンロード リンクは、価値ある重要な知財資産であることに注意してください。 リークが生じると、それらのライセンス認証制限がすぐに枯渇し、顧客エクスペリエンスやパートナー エクスペリエンスに悪影響を及ぼす恐れがあります。

### <a name="next-steps"></a>次のステップ

ソフトウェアキーの配布に関する使用方法と重要なガイダンスについては、次のリソースを参照してください。

- [CSP プログラムによるオンプレミス ソフトウェアの販売](../csp-on-premise-software.md)
- [Partner Center New Commerce Operations Guide](https://partner.microsoft.com/resources/detail/partner-center-new-commerce-operations-guide-pdf) (**ソフトウェア キーの配布に関するガイダンス** に関するセクションを参照してください)。

### <a name="questions"></a>わからないことがある場合は、

この通知についてさらにご質問がある場合は、関連する Yammer コミュニティをご確認ください。

________________
## <a name="migrate-your-deals-from-partner-sales-connect-psc-to-partner-center"></a><a name="3"></a>Partner Sales Connect (PSC) からパートナー センターに取引を移行

### <a name="categories"></a>Categories

- 日付: 2021 年 3 月 4 日
- 機能

### <a name="summary"></a>まとめ

Partner Sales Connect (PSC) は、2021 年 3 月 31 日から読み取り専用アクセスに移行するので、PSC からパートナー センターに取引を移行し始めることをお勧めします。

### <a name="impacted-audience"></a>対象

PSC での取引があるパートナー

### <a name="details"></a>詳細

成長に対する共有コミットメントの一環として、**Microsoft との共同販売** は、お客様が **認識され、専門知識を提供し、顧客フットプリントを拡大して**、良好な顧客アウトカムを得るための手段です。 パートナー センターで共同販売エクスペリエンスを管理すれば、平均的な処理が通常より **3.5 倍高速** になり、顧客への直接販売や、パートナー、Microsoft の販売者チャネルなどに対する販売ができ、1 か所でパイプライン全体を管理できます。

**PSC** は **2021 年 3 月 31 日** から **読み取り専用アクセス** に移行するため、パートナー センターへの移行を開始し、以下のような機能改善にアクセスすることをお勧めします。 

- お客様が必要とするサポートの種類に基づいて、Microsoft と共有する取引を適切な販売者に **ルーティングする際の正確さの向上**。
- インセンティブの対象となるソリューションに対する適格性があるか、および ISV コネクト プログラムの基準を満たしているかについての **前払い取引の検証**。このため、承認プロセスと最終的な実行証明 (POE) の立証が簡略化されます。
- すべての共同販売機会とセールス見込み客を 1 か所で管理するための **シームレスなユーザー エクスペリエンス**。

また、お客様の移行を支援するために、最近パートナー センターに次のような新しい機能が追加されました。

- [共同販売機会の一括操作](../bulk-operations.md)
- [取引移行機能](../psc-to-pc.md) (**PSC 取引の移行** に関するセクションを参照してください)。

パートナー センターの共同販売エクスペリエンスを利用することで、販売チームは、見込み客や機会の促進、契約の締結、顧客との長期的な関係の形成に集中する時間が増えます。

### <a name="next-steps"></a>次のステップ

パートナー センターへの[移行ガイド](../psc-to-pc.md)を使用して、PSC からパートナー センターに取引を移行する手順について説明します。

### <a name="questions"></a>わからないことがある場合は、

その他の質問については、[サポート](https://partner.microsoft.com/support/?stage=1)にお問い合わせください。

________________
## <a name="new-microsoft-dynamics-365-products-and-offers-available-on-april-1-2021"></a><a name="2"></a>新しい Microsoft Dynamics 365 製品およびオファーが 2021 年 4 月 1 日に利用できるようになります

### <a name="categories"></a>Categories

- 日付: 2021 年 3 月 4 日
- 機能

### <a name="summary"></a>まとめ

2021 年 4 月 1 日、Microsoft は、クラウド ソリューション プロバイダー (CSP) プログラム用のいくつかの新しい製品およびプランを開始します。

### <a name="impacted-audience"></a>対象

クラウド ソリューション プロバイダー (CSP) プログラムを通じて取引を行う、すべてのパートナー様

### <a name="details"></a>詳細

2021 年 4 月 1 日に、Microsoft は、次のような新しい製品およびプランを開始します。

- Power BI Premium Per User
- Customer Voice および Marketing USL の地域およびセグメントの拡張

**Power BI Premium Per User**

Microsoft は、最初のユーザーごとの Power BI Premium プランを導入します。 Power BI Premium は現在、容量構成でのみ販売されています。 Power BI Premium Per User は、ユーザーごとに、エンタープライズ ビジネス インテリジェンス (BI) および分析機能へのアクセスを提供します。 その柔軟な個別のシート ライセンスで、中小規模の企業の要求に応えます。

このプランについて詳しくは、[Power BI リリースの詳細](/power-platform-release-plan/2020wave2/power-bi/planned-features)に関するページを参照してください。


**特典の詳細**

プラン名は、価格表プレビューとは若干異なることに注意してください。

| プラン名 | プラン ID |
| ------ |----------- |
| Power BI Premium Per User | 9c810018-9356-4903-95ab-eeb956289290 | 
| 教職員用 Power BI Premium Per User | 3affc44f-f372-4ad5-8657-aadd9574fce0 | 
| 学生用 Power BI Premium Per User | 657eea87-d0b0-4c89-8c8e-9b04395bd940 | 
| Power BI Premium Per User (非営利団体職員向けの価格) | 7a0a856c-059f-45dd-9d26-ae27992e706a | 
| Power BI Premium Per User アドオン | 244ff87e-5925-44a0-bf31-cea189719b58 | 
| 教職員用 Power BI Premium Per User アドオン | 5da849bd-b8f7-4340-b4f4-3a9eaeb8987e | 
| 学生用 Power BI Premium Per User アドオン | cf62d70d-5af5-422a-bda8-97936402ac8e | 
| Power BI Premium Per User アドオン (非営利団体職員向けの価格) | 31c03289-47ab-4ab0-8df1-03742c127ac6 | 

**Customer Voice および Marketing USL の地域およびセグメントの拡張**

2020 年 12 月の発売後のフォローアップとして、Dynamics 365 Customer Voice および Marketing USL プランは、新しい国やより多くの非営利団体および教育機関向けの SKU を追加するように変更されてきました。

| プラン名 | プラン ID |
| ------ |----------- |
| Dynamics 365 Customer Voice USL (非営利団体職員向けの価格) | 7a8642a5-481e-4906-a642-b56dbeeb62a0 |
| 教職員用 Dynamics 365 Customer Voice USL | 85162d70-9676-4cf6-a4bc-a0d6672f2657 |

これらのプランについて詳しくは、次のページを参照してください。

- [Dynamics 365 Customer Service Voice ホーム ページ](https://dynamics.microsoft.com/customer-voice/overview/)
- [Dynamics 365 Marketing ホーム ページ](https://dynamics.microsoft.com/customer-voice/overview/)

### <a name="next-steps"></a>次のステップ

このトピックに関するリソースを確認し、この情報を組織内の該当する関係者と共有します。  

### <a name="questions"></a>わからないことがある場合は、

これらのプランについてさらにご質問がある場合は、関連する Yammer コミュニティをご確認ください。 

________________
## <a name="microsoft-universal-print-now-available-in-some-suites"></a><a name="1"></a>Microsoft Universal Print が一部のスイートで利用できるようになりました

### <a name="categories"></a>Categories

- 日付: 2021 年 3 月 3 日
- 機能

### <a name="summary"></a>まとめ

Microsoft Universal Print は、2021 年 3 月 1 日から、選択された Microsoft 365 スイート内での取引に利用したり、スタンドアロン アドオンとして利用したりできるようになります。

### <a name="impacted-audience"></a>対象

クラウド ソリューション プロバイダー (CSP) プログラムを通じて取引を行う、すべてのパートナー様

### <a name="details"></a>詳細

[Universal Print](https://aka.ms/universalprint) は、オンプレミスのプリント サーバーを不要にし、Windows デバイスから Azure 登録済みプリンターに出力できるようにする Microsoft 365 プリント サービスです。 2021 年 3 月 1 日から取引に利用できるようになります。

ワーカーは、ドライバー不要の印刷、合理化されたロケーションベースのプリンター検出、学習曲線不要の直感的な印刷操作などの利点が得られます。 Azure Active Directory (Azure AD) に参加しているデバイスは、既存の Azure AD 資格情報を使用して安全に印刷します。 管理者は Azure portal を使用して印刷を管理し、Universal Print のネイティブ サポートを使用してプリンターを簡単に接続できます。 Universal Print は、Universal Print コネクタ ソフトウェアを使用して、互換性のないプリンターで展開できます。

Universal Print はサービス開始時に、Windows E3、A3、E5、A5 と Microsoft 365 BP、F3、E3、A3、E5、A5 に追加されます。  

**特典の詳細**

プラン名は、価格表プレビューとは若干異なることに注意してください。

| プラン名 | プラン ID | マテリアル ID |
| ------ |----------- |----------- |  
| Universal Print ボリューム アドオン (500 ジョブ) - Microsoft 365  | cb131356-45ee-4ae2-8537-873b706c8e75     | 9BI-00004   |
| 教職員用 Universal Print ボリューム アドオン (500 ジョブ) - Microsoft 365   | 477bee81-9872-43d6-91d3-c72390bfcf49   | 9BK-00004   |
| Universal Print ボリューム アドオン (500 ジョブ) - Windows    | d3ddc493-5741-4e0d-a02d-07edbb0bb72e   | 9BI-00002   |
| 教職員用 Universal Print ボリューム アドオン (500 ジョブ) - Windows   |  d0862f05-80f5-4fd4-8432-fe72dd893cc7  | 9BK-00002   |

### <a name="next-steps"></a>次のステップ

価格表と [Universal Print の概要](/universal-print/fundamentals/universal-print-whatis)についてご確認ください。 この情報を組織内の適切なすべての担当者に共有してください。

### <a name="questions"></a>ご質問がある場合は、

これらのプランについてさらにご質問がある場合は、関連する Yammer コミュニティをご確認ください。
