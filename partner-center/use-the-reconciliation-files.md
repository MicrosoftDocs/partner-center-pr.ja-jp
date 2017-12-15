---
title: "調整ファイルの使用 | パートナー センター"
description: "請求サイクルの各料金の詳しい行項目ビューについては、パートナー センターのダッシュボードから調整ファイルをダウンロードします。"
ms.assetid: FA6A6FCB-2597-44E7-93F8-8D1DD35D52EA
author: KPacquer
ms.openlocfilehash: 892204ebcdfe1e1318985f2d50df8af2238bd4c1
ms.sourcegitcommit: 2436cb77fbefc41cc9cb3e62e8a616b6326c557f
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/04/2017
---
# <a name="use-the-reconciliation-files"></a>調整ファイルの使用

**適用対象**

-  パートナー センター
-  米国政府機関向け Microsoft Cloud のパートナー センター
-  Microsoft Cloud ドイツのパートナー センター

請求サイクルの各料金の詳しい行項目ビューについては、パートナー センターのダッシュボードから調整ファイルをダウンロードします。 詳細には、各顧客のサブスクリプションの料金や、詳細なイベント (期間途中でのサブスクリプションへのシートの追加など) が含まれます。

## <a href="" id="itemizebypartner"></a>パートナーごとに明細を示す


インダイレクト モデルのパートナーは、ライセンスベースの調整ファイルと使用量ベースの調整ファイルの両方で、これらの追加フィールドを使用してリセラーごとに明細を記載できます。

<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th>MPN ID</th>
<th>説明</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td>MPN ID</td>
<td><p>CSP パートナー (直接または間接) の Microsoft Partner Network (MPN) IDです。</p></td>
</tr>
<tr class="even">
<td>リセラーの MPN ID</td>
<td><p>インダイレクト モデルのパートナーの調整ファイルにのみ表示されます。</p>
<p>サブスクリプションの登録のあるリセラーの MPN ID。 これは、パートナー センターで特定のサブスクリプションについて示されるリセラー ID に対応します。</p>
<p>リセラーを表示または更新するには、パートナー センター メニューで <strong>[顧客]</strong> を選び、一覧から顧客を選びます。 顧客メニューで <strong>[サブスクリプション]</strong> を選び、一覧からサブスクリプションを選びます。 <strong>[更新]</strong> を選んで、<strong>[再販業者 (MPN ID)]</strong> を変更します。</p>
<p>CSP パートナーがお客様に直接サブスクリプションを販売した場合、パートナーの MPN ID が MPN ID とリセラーの MPN ID として 2 か所に表示されます。</p>
<p>CSP パートナーのリセラーに MPN ID がない場合は、代わりに CSP パートナーの MPN ID がこの値に設定されます。</p>
<p>CSP パートナーがリセラー ID を削除した場合、この値は -1 に設定されます。</p></td>
</tr>
</tbody>
</table>

 

## <a href="" id="licensebasedfiles"></a> ライセンスベースのファイルのフィールド


顧客の注文に対する料金を調整するには、調整ファイルの Syndication\_Partner\_Subscription\_Number とパートナー センターのサブスクリプション ID を比較します。

<table>
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<tbody>
<tr class="odd">
<td><strong>列</strong></td>
<td><strong>説明</strong></td>
<td><strong>サンプル値</strong></td>
</tr>
<tr class="even">
<td>PartnerId</td>
<td><p>特定の課金エンティティの一意の識別子 (GUID 形式)。 調整には必要ありませんが、有用な情報である場合があります。 すべての行で同じです。</p></td>
<td>8ddd03642-test-test-test-46b58d356b4e</td>
</tr>
<tr class="odd">
<td>CustomerID</td>
<td><p>顧客を識別するために使用される、GUID 形式の一意の Microsoft ID。</p></td>
<td>12ABCD34-001A-BCD2-987C-3210ABCD5678</td>
</tr>
<tr class="even">
<td>OrderID</td>
<td><p>Microsoft 課金プラットフォームでの注文の一意の識別子。 サポートに問い合わせる際に、注文の識別に有効な場合がありますが、調整には有用ではありません。</p></td>
<td>566890604832738111</td>
</tr>
<tr class="odd">
<td>SubscriptionID</td>
<td><p>Microsoft 課金プラットフォームでのサブスクリプションの一意の識別子。 サポートに問い合わせる際に、サブスクリプションの識別に有効な場合がありますが、調整には有用ではありません。</p>
<p>これは、パートナー管理コンソールのサブスクリプション ID と同じではありません。 「Syndication_Partner_Subscription_Number」をご覧ください。</p></td>
<td>usCBMgAAAAAAAAIA</td>
</tr>
<tr class="even">
<td>SyndicationPartnerSubscriptionNumber</td>
<td><p>サブスクリプションの一意の識別子。 お客様は同じプランで複数のサブスクリプションを持つことができるため、これは調整ファイルの分析で重要です。</p>
<p>このフィールドは、パートナー管理コンソールのサブスクリプション ID にマップされます。</p></td>
<td>fb977ab5-test-test-test-24c8d9591708</td>
</tr>
<tr class="odd">
<td>OfferID</td>
<td><p>一意のプラン ID。 価格表に従った標準のプラン ID。</p>
<p><b>注</b>: この値は、価格表のプラン ID とは一致しません。 以下の DurableOfferID を参照してください。</p></td>
<td>FE616D64-E9A8-40EF-843F-152E9BBEF3D1</td>
</tr>
<tr class="even">
<td>DurableOfferID</td>
<td><p>価格表で定義されている一意の継続的なプラン ID。</p>
<p><b>注</b>: この値は価格表のプラン ID と一致します。</p></td>
<td>1017D7F3-6D7F-4BFA-BDD8-79BC8F104E0C</td>
</tr>
<tr class="odd">
<td>OfferName</td>
<td><p>価格表で定義されている、顧客が購入したサービス プランの名前。</p></td>
<td>Microsoft Office 365 (プラン E3)</td>
</tr>
<tr class="even">
<td>SubscriptionStartDate</td>
<td><p>サブスクリプションの開始日。注文が送信された日に設定されます。 サブスクリプションの開始日を終了日と共に確認することにより、顧客がサブスクリプションの最初の 1 年以内であるか、サブスクリプションが次の 1 年間更新されたかを確認できます。</p>
<p>時刻は常に、その日の始まりの時刻 (0:00) になります。</p></td>
<td>2/1/2015 0:00</td>
</tr>
<tr class="odd">
<td>SubscriptionEndDate</td>
<td><p>サブスクリプション終了日: 開始日から 12 か月 + x 日後 (パートナーの請求日と合わせる) または更新日から 12 か月</p>
<p>更新時に、価格は最新の価格表に更新されます。 自動更新の前に、顧客とのやり取りが必要になる場合があります。</p>
<p>時刻は常に、その日の始まりの時刻 (0:00) になります。</p></td>
<td>2/1/2015 0:00</td>
</tr>
<tr class="even">
<td>ChargeStartDate</td>
<td><p>課金の開始日。</p>
<p>顧客がシート数を変更するときに、この数値を使用して 1 日あたり (日割り) の料金を計算します。</p>
<p>時刻は常に、その日の始まりの時刻 (0:00) になります。</p></td>
<td>2/1/2015 0:00</td>
</tr>
<tr class="odd">
<td>ChargeEndDate</td>
<td><p>課金の終了日。</p>
<p>顧客がシート数を変更するときに、この数値を使用して 1 日あたり (日割り) の料金を計算します。</p>
<p>時刻は常に、その日の終わりの時刻 (23:59) になります。</p></td>
<td>2/28/2015 23:59</td>
</tr>
<tr class="even">
<td>ChargeType</td>
<td><p>課金または調整の種類。 「<a href="#charge_types">請求書と調整ファイルの間の課金のマッピング</a>」を参照してください。</p></td>
<td><p>「<a href="#charge_types">請求書と調整ファイルの間の課金のマッピング</a>」を参照してください。</p></td>
</tr>
<tr class="odd">
<td>UnitPrice</td>
<td><p>シートごとの価格。 調整中に、請求システムに格納された情報と一致することを確認します。</p></td>
<td>6.82</td>
</tr>
<tr class="even">
<td>Quantity</td>
<td><p>シート数。 調整中に、請求システムに格納された情報と一致することを確認します。</p></td>
<td>2</td>
</tr>
<tr class="odd">
<td>Amount</td>
<td><p>数量に対する合計価格。 金額の計算が、この顧客用の計算方法に一致することを確認するために役立ちます。</p></td>
<td>13.32</td>
</tr>
<tr class="even">
<td>TotalOtherDiscount</td>
<td><p>これらの料金に適用される割引額。 インセンティブの対象となる IUR または新しいサブスクリプションの場合も、この列に割引額が含まれます。</p></td>
<td>2.32</td>
</tr>
<tr class="odd">
<td>Subtotal</td>
<td><p>合計額 (税抜)。 割引の場合、小計が、予想される合計と一致することを確認します。</p></td>
<td>11</td>
</tr>
<tr class="even">
<td>Tax</td>
<td><p>市場の税関連の規則や特定の状況に基づく税金の額。</p></td>
<td>0</td>
</tr>
<tr class="odd">
<td>TotalForCustomer</td>
<td><p>合計額 (税込)。 請求書に課税されるかどうかを確認します。</p></td>
<td>11</td>
</tr>
<tr class="even">
<td>Currency</td>
<td><p>通貨の種類。 各課金エンティティの通貨は 1 つのみです。 最初の請求書と一致し、その後で、主要な課金プラットフォームの更新と一致することを確認します。</p></td>
<td>EUR</td>
</tr>
<tr class="odd">
<td>CustomerName</td>
<td><p>パートナー センターで報告される顧客の組織名。 これは、システムの情報を使って請求書を調整するために非常に重要です。</p></td>
<td>Test Customer A</td>
</tr>
<tr class="even">
<td>MPNID</td>
<td><p>CSP パートナーの MPN ID</p></td>
<td>4390934</td>
</tr>
<tr class="odd">
<td>ResellerMPNID</td>
<td><p>サブスクリプションの登録のあるリセラーの MPN ID。 「[パートナーごとに明細を示す](#itemizebypartner)」をご覧ください。</p></td>
<td>4390934</td>
</tr>
<tr class="even">
<td>DomainName</td>
<td><p>顧客のドメイン名。顧客を特定できるようにするために使用されます。</p></td>
<td>example.onmicrosoft.com</td>
</tr>
<tr class="odd">
<td>SubscriptionName</td>
<td><p>サブスクリプションのニックネーム。 ニックネームが指定されていない場合、パートナー センターでは OfferName を使用します。</p></td>
<td>PROJECT ONLINE</td>
</tr>
<tr class="even">
<td>SubscriptionDescription</td>
<td><p>価格表で定義されている、顧客が購入したサービス プランの名前  (これはプラン名と同一のフィールドです)。</p></td>
<td>PROJECT ONLINE PREMIUM WITHOUT PROJECT CLIENT</td>
</tr>
</tbody>
</table>


## <a href="" id="usagebasedfiles"></a>使用量ベースのファイルのフィールド


顧客の使用量に対する料金を調整するには、調整ファイルの ResellerID/ResellerName/ResellerBillableAccount、顧客名、およびパートナー センターのサブスクリプション ID を比較します。

次のフィールドで、どのサービスが使用されるか、およびレートについて説明します。

<table>
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<tbody>
<tr class="odd">
<td><strong>列</strong></td>
<td><strong>説明</strong></td>
<td><strong>サンプル値</strong></td>
</tr>
<tr class="even">
<td>PartnerID</td>
<td><p>GUID 形式のパートナー ID。</p></td>
<td>DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</td>
</tr>
<tr class="odd">
<td>PartnerName</td>
<td><p>パートナー名。</p></td>
<td>Acme Incorporated</td>
</tr>
<tr class="even">
<td>PartnerBillableAccountID</td>
<td><p>パートナーのアカウント ID。</p></td>
<td>1010578050</td>
</tr>
<tr class="odd">
<td>CustomerName</td>
<td><p>パートナー センターで報告される顧客の組織名。 これは、システムの情報を使って請求書を調整するために非常に重要です。</p></td>
<td>Test Customer A</td>
</tr>
<tr class="even">
<td>MPNID</td>
<td><p>CSP パートナーの MPN ID。</p></td>
<td>4390934</td>
</tr>
<tr class="odd">
<td>ResellerMPNID</td>
<td><p>サブスクリプションの登録のあるリセラーの MPN ID。 「[パートナーごとに明細を示す](#itemizebypartner)」をご覧ください。</p></td>
<td>4390934</td>
</tr>
<tr class="even">
<td>InvoiceNumber</td>
<td><p>指定されたトランザクションが含まれる請求書番号。</p></td>
<td>D020001IVK</td>
</tr>
<tr class="odd">
<td>ChargeStartDate</td>
<td><p>前の課金サイクルからの潜在的な未請求の使用状況データの日付を提示するときを除く、課金サイクルの開始日。</p>
<p>時刻は常に、その日の始まりの時刻 (0:00) になります。</p></td>
<td>2/1/2014 0:00</td>
</tr>
<tr class="even">
<td>ChargeEndDate</td>
<td><p>前の課金サイクルからの潜在的な未請求の使用状況データの日付を提示するときを除く、課金サイクルの終了日。</p>
<p>時刻は常に、その日の終わりの時刻 (23:59) になります。</p></td>
<td>2/28/2014 23:59</td>
</tr>
<tr class="odd">
<td>SubscriptionID</td>
<td><p>Microsoft 課金プラットフォームでのサブスクリプションの一意の識別子。 サポートに問い合わせる際に、サブスクリプションの識別に有効な場合がありますが、調整には有用ではありません。</p>
<p>これは、パートナー管理コンソールのサブスクリプション ID と同じではありません。</p></td>
<td>usCBMgAAAAAAAAIA</td>
</tr>
<tr class="even">
<td>SubscriptionName</td>
<td><p>サービス プランのニックネーム。</p></td>
<td>Microsoft Azure</td>
</tr>
<tr class="odd">
<td>SubscriptionDescription</td>
<td><p>サービス プランの基幹業務</p></td>
<td>Microsoft Azure</td>
</tr>
<tr class="even">
<td>OrderID</td>
<td><p>Microsoft 課金プラットフォームでの注文の一意の識別子。 サポートに問い合わせる際に、サブスクリプションの識別に有効な場合がありますが、調整には有用ではありません。</p></td>
<td>566890604832738111</td>
</tr>
<tr class="odd">
<td>ServiceName</td>
<td><p>対象の Azure サービスの名前。</p></td>
<td>VIRTUAL MACHINES</td>
</tr>
<tr class="even">
<td>ServiceType</td>
<td><p>Windows Azure サービスの特定の種類。</p></td>
<td><ul>
<li>Service Bus – Individual or Pack</li>
<li>SQL Azure database – Business or Web Edition</li>
</ul></td>
</tr>
<tr class="odd">
<td>ResourceGUID</td>
<td><p>すべてのサービス データおよび価格設定構造の特定の一意の識別子。</p></td>
<td>DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</td>
</tr>
<tr class="even">
<td>リソース名</td>
<td><p>Azure リソースの名前。</p></td>
<td><ul>
<li>Data Transfer In (GB)</li>
<li>Data Transfer Out (GB)</li>
</ul></td>
</tr>
<tr class="odd">
<td>Region</td>
<td><p>使用量が適用される地域。 料金は地域によって異なるため、主にデータ転送に料金を割り当てるために使われます。</p></td>
<td>Asia Pacific、Europe、Latin America、North America</td>
</tr>
<tr class="even">
<td>SKU</td>
<td><p>プランについての MSFT の一意の識別子</p></td>
<td>7UD 00001</td>
</tr>
<tr class="odd">
<td><p>DetailLineItemId</p></td>
<td><p>特定の課金期間のサービスまたはリソースに対してさまざまなレートの明細を設定するための ID と数量。 Azure の階層化されたレーティングの場合は、一定数量の課金可能単位までは 1 つのレートがあり、その後に別のレートがあることがあります。</p></td>
<td>1</td>
</tr>
<tr class="even">
<td>ConsumedQuantity</td>
<td><p>レポート期間のサービスの使用量 (時間、GB など)。</p>
<p>前のレポート期間から課金していない使用も含まれます。</p></td>
<td>11</td>
</tr>
<tr class="odd">
<td>IncludedQuantity</td>
<td><p>単位数はプランの一部として含まれます。 通常、CSP には含まれません。</p></td>
<td>0</td>
</tr>
<tr class="even">
<td><p>OverageQuantity</p></td>
<td><p>単位数はプランの一部として含まれず、パートナーが支払う必要があります。</p>
<p>ConsumedQuantity - IncludedQuantity と同じです。</p></td>
<td>11</td>
</tr>
<tr class="odd">
<td>ListPrice</td>
<td><p>サブスクリプションの開始日に有効な価格を提供します。</p></td>
<td>$0.0808</td>
</tr>
<tr class="even">
<td>PretaxCharges</td>
<td><p>ListPrist と OverageQuantity を掛けて、最も近いセントに丸めます。</p></td>
<td>$0.085</td>
</tr>
<tr class="odd">
<td>TaxAmount</td>
<td><p>市場の税関連の規則や特定の状況に基づく税金の額。</p></td>
<td>$0.08</td>
</tr>
<tr class="even">
<td>PostTaxTotal</td>
<td><p>税が適用されるときの税引き後の合計額。</p></td>
<td>$0.93</td>
</tr>
<tr class="odd">
<td>Currency</td>
<td><p>通貨の種類。 各課金エンティティの通貨は 1 つのみです。 最初の請求書と一致し、その後で、主要な課金プラットフォームの更新と一致することを確認します。</p></td>
<td>EUR</td>
</tr>
<tr class="even">
<td>PretaxEffectiveRate</td>
<td><p>単位あたりの税込み価格。 PretaxCharges / OverageQuantity と同じで、最も近いセントに丸められます。</p></td>
<td>$0.08</td>
</tr>
<tr class="odd">
<td>PostTaxEffectiveRate</td>
<td><p>単位あたりの税引き後の価格。 PostTaxTotal / OverageQuantity、または PretaxEffectiveRate + 単位額あたりの税率と同じで、最も近いセントに丸められます。</p></td>
<td>$0.08</td>
</tr>
<tr class="even">
<td>ChargeType</td>
<td><p>課金または調整の種類。 「<a href="#charge_types">請求書と調整ファイルの間の課金のマッピング</a>」を参照してください。</p></td>
<td><p>「<a href="#charge_types">請求書と調整ファイルの間の課金のマッピング</a>」を参照してください。</p></td>
</tr>
<tr class="odd">
<td>CustomerBillableAccount</td>
<td><p>MSFT 課金プラットフォームの一意のアカウント ID。</p></td>
<td>1280018095</td>
</tr>
<tr class="even">
<td>UsageDate</td>
<td><p>サービスの展開の日付。</p></td>
<td>2/1/2014 0:00</td>
</tr>
<tr class="odd">
<td>MeteredRegion</td>
<td><p>この列は、これが該当し、設定されている場合に、サービスの領域内でのデータ センターの場所を識別します。</p></td>
<td>East Asia、South East Asia、North Europe、West Europe、North Central US、South Central US</td>
</tr>
<tr class="even">
<td>MeteredService</td>
<td><p>この列は、[Service Name] 列で特に識別されない可能性のある、個別の Microsoft Azure サービスの追跡に利用されます。 たとえば、データ転送は、[Service Name] 列で &quot;Microsoft Azure - All Services&quot; と報告されます。 この [MeteredService] 列は、利用に関連する特定のサービスを示します。</p></td>
<td>AccessControl、CDN、Compute、Database、ServiceBus、Storage</td>
</tr>
<tr class="odd">
<td>MeteredServiceType</td>
<td><p>個々の Microsoft Azure サービスの内容を、MeteredService フィールドで提供されるレベルよりも明確にする小見出し。</p></td>
<td>EXTERNAL</td>
</tr>
<tr class="even">
<td>Project</td>
<td><p>サービス インスタンスの顧客定義の名前</p></td>
<td>ORDDC52E52FDEF405786F0642DD0108BE4</td>
</tr>
<tr class="odd">
<td>ServiceInfo</td>
<td><p>特定の日にプロビジョニングされ、利用された ServiceBus 接続の数。</p></td>
<td>例: 1 か月 30 日間の中に、個別にプロビジョニングされた接続がある場合、Service Info 1 は "1.000000 Connections / 30 days" と表示されます。 プロビジョニングされた ServiceBus 接続が 25 パックあり、その日に 1 つを利用した場合、その日の 1 日の使用量の計算書には、"25 Connections / 30 Days – Used: 1.000000" と表示されます。</td>
</tr>
<tr class="even">
<td>CustomerID</td>
<td><p>顧客を識別するために使用される、GUID 形式の一意の Microsoft ID。</p></td>
<td>ORDDC52E52FDEF405786F0642DD0108BE4</td>
</tr>
<tr class="odd">
<td>DomainName</td>
<td><p>顧客のドメイン名。顧客を特定できるようにするために使用されます。</p></td>
<td>example.onmicrosoft.com</td></tr>
</tr>
<tr class="even">
<td>Unit</td>
<td><p>リソース名の単位</p></td>
<td>GB または HOURS</td>
</tr>
</tbody>
</table>



## <a href="" id="charge_types"></a>請求書と調整ファイルの間の課金のマッピング

請求書は料金の概要を示し、調整ファイルは、課金の種類を含め、行項目のトランザクションの詳細な内訳を示します。

請求書と調整ファイルの間で請求金額を相互参照するには、Microsoft Excel のフィルター オプションを使用して、調整ファイルの課金の種類でフィルター処理し、請求書の課金を調整ファイルの一連の課金の内訳にマップします。

使用量ベースとライセンス ベースの調整ファイルには、使用量関連のトランザクションと料金 (消費された単位量および関連する料金) のみが表示されます。 請求書に “調整” として表示される単発のクレジット、割引、払い戻し金額は、調整ファイルに表示されません。

次の表に、請求書のセクションと、調整ファイルに表示される関連付けられた課金の種類とのマッピングを示します。 

<table>
<tbody>
<tr>
<td>
<p><strong>請求書の課金の説明</strong></p>
</td>
<td>
<p><strong>調整ファイルの課金の説明 (ChargeType 列)</strong></p>
</td>
<td>
<p><strong>この課金の意味</strong></p>
</td>
<td>
<p><strong>これらの ChargeTypes を請求書にマップする方法</strong></p>
</td>
</tr>
<tr>
<td rowspan="8">
<p><strong>当月のサービス利用料金</strong></p>
</td>
<td>
<p>Cancel instance prorate</p>
</td>
<td>
<p>関連付けられているシートが変更されたときに顧客に払い戻される日割り料金</p>
</td>
<td rowspan="8">
<p>ライセンスベースのファイルから、<strong>Amount</strong> 列を合計する</p>
</td>
</tr>
<tr>
<td>
<p>Cycle fee</p>
</td>
<td>
<p>サブスクリプションの定期的な課金</p>
</td>
</tr>
<tr>
<td>
<p>Cycle instance prorate</p>
</td>
<td>
<p>関連付けられているシートが変更されたときに顧客から評価される日割り料金</p>
</td>
</tr>
<tr>
<td>
<p>Prorate fees when cancel</p>
</td>
<td>
<p>取り消し時のサービスの未使用部分に対する日割りの払戻し額</p>
</td>
</tr>
<tr>
<td>
<p>Prorate fees when purchase</p>
</td>
<td>
<p>購入時の日割りの料金</p>
</td>
</tr>
<tr>
<td>
<p>Purchase fee</p>
</td>
<td>
<p>サブスクリプションの最初の課金</p>
</td>
</tr>
<tr>
<td>
<p>Prorate fee when renew</p>
</td>
<td>
<p>サブスクリプションの更新時の日割り料金</p>
</td>
</tr>
<tr>
<td>
<p>Renew fee</p>
</td>
<td>
<p>サブスクリプションの更新時の課金</p>
</td>
</tr>
<tr>
<td>
<p><strong>その他の製品とサービス</strong></p>
</td>
<td>
<p>Prorate fees when activate</p>
</td>
<td>
<p>アクティブ化から課金期間の終了までの日割り料金</p>
</td>
<td>
<p>ライセンスベースのファイルから、<strong>Amount</strong> 列を合計する</p>
</td>
</tr>
<tr>
<td rowspan="2">
<p><strong>利用料金</strong></p>
</td>
<td>
<p>Assess usage fee when cancel</p>
</td>
<td>
<p>現在の課金期間中に未払いの使用を取り消したときのアクセス利用料</p>
</td>
<td rowspan="2">
<p>使用量ベースのファイルから、<strong>PretaxCharges</strong> 列を合計する</p>
</td>
</tr>
<tr>
<td>
<p>Assess usage fee for current cycle</p>
</td>
<td>
<p>現在の課金期間のアクセス利用料</p>
</td>
</tr>
<tr>
<td>
<p><strong>調整額</strong></p>
</td>
<td>
<p>Offset a line item</p>
</td>
<td>
<p>税金を含む、行項目への一部または全部の払戻し</p>
</td>
<td>
<p>ライセンスベースのファイルから、<strong>TotalForCustomer</strong> 列を合計する</p>
<p>使用量ベースのファイルから、<strong>PostTaxTotal</strong> 列を合計する</p>
</td>
</tr>


<tr>
<td rowspan="4">
<p><strong>その他の割引</strong></br>
<em>(使用量ベース)</em></p>
</td>
<td>
<p>Activation discount</p>
</td>
<td>
<p>サブスクリプションがアクティブ化されたときに適用される割引</p>
</td>
<td rowspan="4">
<p>使用量ベースのファイルから、<strong>PretaxCharges</strong> 列を合計する</p>
</td>
</tr>
<tr>
<td>
<p>Cycle discount</p>
</td>
<td>
<p>定期的な課金に適用される割引</p>
</td>
</tr><tr>
<td>
<p>Renew discount</p>
</td>
<td>
<p>サブスクリプションの更新時に適用される割引</p>
</td>
</tr><tr>
<td>
<p>Cancel discount</p>
</td>
<td>
<p>割引が取り消されたときに適用される料金</p>
</td>
</tr>
<tr>
<td>
<p><strong>その他の割引</strong></br>
<em>(ライセンスベース)</em></p>
</td>
<td>
<p><em>複数の種類の料金に適用される場合がある</em></p>
</td>
<td>
<p>&nbsp;</p>
</td>
<td>
<p>ライセンスベースのファイルから、<strong>TotalOtherDiscount</strong> 列を合計する</p>
</td>
</tr>
<tr>
<td>
<p><strong>税</strong>&nbsp;または&nbsp;<strong>VAT</strong></p>
</td>
<td>
<p><em>複数の種類の料金に適用される場合がある</em></p>
<p><em>例外: "Offset a line item" には既に税が含まれます。 前の「調整額」を参照してください。</em></p>
</td>
<td>
<p>税または付加価値税 (VAT)</p>
</td>
<td>
<p>ライセンスベースのファイルから、<strong>Tax</strong> 列を合計する</p>
<p>使用量ベースのファイルから、<strong>TaxAmount</strong> 列を合計する</p>
</td>
</tr>
</tbody>
</table>
<p>&nbsp;</p>
