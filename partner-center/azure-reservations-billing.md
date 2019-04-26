---
title: Azure Reservations の請求 | パートナー センター
ms.topic: article
ms.date: 03/15/2019
Description: Azure 予約の課金について説明します。
author: LauraBrenner
ms.author: v-petand
keywords: Azure RI, Azure 予約インスタンス, 予約, VM, 管理, 請求, 購入
robots: noindex, nofollow
ms.localizationpriority: medium
ms.openlocfilehash: b99cb2a72d69cd33f9267a956f921aa65dedd482
ms.sourcegitcommit: b1ab80345b4e4af649fb8cc51d96d798e0791ade
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/23/2019
ms.locfileid: "62135422"
---
# <a name="microsoft-azure-reserved-vm-instances-billing"></a>Microsoft Azure Reserved VM Instances の請求

**適用対象**

-  パートナー センター
-  Microsoft Azure portal
-  CSP のパートナー

クラウド ソリューション プロバイダー (CSP) プログラムのパートナーは、Microsoft Azure Virtual Machines 上の予約インスタンスを顧客に提供できます。 顧客は、事前に仮想マシンを (1 年または 3 年の期間で) 予約して、Azure の使用料を大きく節約できます。   

顧客は、Azure Reserved VM Instances の支払いを事前に行います。 顧客の代わりに Azure Reserved VM Instances を購入した場合は、このような 1 回限りの料金に対する請求書と調整ファイルが届きます。 

>[!IMPORTANT]
>通貨が異なる市場の顧客用に Azure Reserved VM Instances を購入する場合、既定の請求通貨はパートナーではなく顧客の市場がベースになります。 顧客が複数の市場に存在する場合は、顧客への請求が必要な各通貨について、個別の請求書と調整ファイルが届き、適切な通貨で顧客に請求できます。 

1 回限りの料金の請求書と調整ファイルにアクセスするには、選択**課金**クリックして、パートナー センターから**1 回**します。 

クラウド ソリューション プロバイダー プログラムでの請求について詳しくは、「[課金の基本](billing-basics.md)」をご覧ください。

## <a name="azure-reserved-vm-instance-invoice-file-definitions"></a>Azure Reserved VM Instances の請求書ファイルの定義

**一般的な課金情報**

|**フィールド** |**定義**|
|:----------------|:-----------------------------|
|US FEIN |連邦税の ID 番号。 |
|請求先 |納税目的で使用する、法律上の会社の住所。 この住所を変更するには、[アカウント設定] > [パートナー課金プロファイル] に移動します。 |
|請求額 |現在のすべての請求額。 |
|クレジット |当初の購入以降に発生した払い戻しアクティビティに対するクレジット。 |
|割引 |顧客注文内の Azure 予約またはその他の項目に適用される割引。 |
|税 |請求書の 2 ページ目で始まる明細セクションの、現在の合計料金に対する税金の合計。 |
|当月の請求額合計 |支払い期限ごとの、請求期間の請求通貨での支払い額。 |
|支払い方法 |地域に基づいて、請求書に対する支払いのタイミングと方法を説明します。 支払いを行うときには、常に請求書番号を含めます。 |
|請求書番号 |請求書の番号。 |
|請求書作成日 |請求書が生成された日付。 |
|支払条件 |1 回限りの購入の場合は、常に 60 日間になります。 |
|支払期日 |この日付までに、お客様からの支払いが受領される必要があります。 |


**1 回限りの料金の詳細な一覧**

|**フィールド** |**定義**|
|:----------------|:-----------------------------|
|日付 |購入日。 |
|説明 |製品名。 |
|Quantity |購入した製品 (予約など) の数。 |
|単価 |製品 (予約など) ごとの価格。 |
|割引 |適用される割引。 |
|税抜き額 |課税前の購入額の小計。 |
|売上税 |税額。 |
|Total |お支払いの合計額。 |


## <a name="azure-reserved-vm-instance-reconciliation-file-descriptions"></a>Azure Reserved VM Instances の調整ファイルの内容

|**フィールド** |**定義**|
|:----------------|:-----------------------------|
|PartnerId |GUID 形式のパートナー ID。 |
|CustomerId |顧客を識別するために使用される、GUID 形式の一意の Microsoft ID。 |
|CustomerName |パートナー センターで報告される顧客の組織名。 これは、システムの情報を使って請求書を調整するために非常に重要です。 |
|CustomerDomainName |顧客のドメイン名。 |
|CustomerCountry |顧客の在住国。 |
|InvoiceNumber |指定されたトランザクションが含まれる請求書番号。 |
|MpnId |CSP パートナー (直接または間接) の MPN ID。 |
|リセラーの MPN ID |インダイレクト モデルのパートナーの調整ファイルにのみ表示されます。 予約に対する登録リセラーの MPN ID。 これは、パートナー センターで特定の予約について示されるリセラー ID に対応します。 CSP パートナーが直接お客様に予約を販売した場合、パートナーの MPN ID が MPN ID とリセラーの MPN ID として 2 か所に表示されます。 CSP パートナーのリセラーに MPN ID がない場合は、代わりに CSP パートナーの MPN ID がこの値に設定されます。 CSP パートナーがリセラー ID を削除した場合、この値は -1 に設定されます。 |
|OrderId |Microsoft 請求プラットフォームでの注文の一意の識別子。 サポートに問い合わせる際に、Azure 予約の識別に有効な場合がありますが、調整用ではありません。 |
|OrderDate |注文が作成された日付。 |
|ProductId |製品の ID。 |
|SkuId  |特定 SKU の ID。 |
|AvailabilityId |特定の可用性 の ID。 "可用性" とは、特定の国、通貨、業界などで特定の SKU を購入可能かどうかを指します。 |
|SkuName  |特定 SKU のタイトル。 |
|ProductName |製品の名前。 |
|ChargeType |課金または調整の種類。 |
|UnitPrice |注文された製品ごとの価格。 |
|Quantity |注文された製品の数。 |
|Subtotal |合計額 (税抜)。 割引の場合、小計が、予想される合計と一致することを確認します。 |
|TaxTotal |該当するすべての税額の合計。 |
|Total |この購入の合計金額。 |
|通貨 |通貨の種類。 各課金エンティティの通貨は 1 つのみです。 最初の請求書と一致し、その後で、主要な課金プラットフォームの更新と一致することを確認します。 |
|DiscountDetails |関連する割引の詳細を示す一覧。 |


## <a name="manage-your-billing"></a>請求の管理

### <a name="view-your-current-billing-status-invoices-and-recon-files"></a>現在の請求の状態、請求書、調整ファイルを表示する

1.  パートナー センターで次のように選択します。**課金**し**1 回**、課金の状態を表示します。 
2.  請求書または調整ファイルを選択して、詳細な情報を確認します。 

### <a name="view-a-customers-order-history"></a>顧客の注文履歴を表示する

1.  選択**顧客**パートナー センターのメニューから。
2.  **[顧客]** ページで、注文履歴を表示する対象の顧客を見つけ、下矢印を選択して顧客レコードを展開します。 
3.  **[View orders]** (注文の表示) を選択して注文履歴を表示します。

### <a name="create-a-credit-or-void-note"></a>クレジット ノートまたは取り消し票を作成する

必要に応じて、請求書を無効にして新しい請求書を発行することがあります。 たとえば、顧客が会社の名前を変更した後で、以前の名前で請求書を受け取った場合などです。 

請求書を無効にし、新しい請求書を発行するには、請求ページの調整欄からフォームをダウンロードします。

## <a name="azure-reservations-resources"></a>Azure Reservations に関するリソース
|**について**   |**この記事を読む**    |
|:-----------------------------|:-----------------|
|CSP での Azure Reservations 概要  | [Microsoft Azure 予約 VM インスタンスを販売します。](azure-reservations.md)
|パートナー センターで顧客向けの Azure 予約を購入   |[Azure 予約を購入します。](azure-reservations-buying.md)
| パートナー センターでの Azure 予約を管理します。 | [パートナー センターでの Azure 予約を管理します。](azure-reservations-manage.md)
|Azure portal で Azure Reservations を購入する | [Azure Reserved VM Instances による仮想マシン料金の前払い](https://docs.microsoft.com/azure/virtual-machines/windows/prepay-reserved-vm-instances) (Azure ヘルプ) |
|Azure portal で Azure Reservations を管理する   |[予約済み VM インスタンスの管理](https://docs.microsoft.com/azure/billing/billing-manage-reserved-vm-instance) (Azure ヘルプ)  |
|パートナー センター API を使用して Azure Reservations を購入する | [Azure Reserved VM Instances の購入](https://docs.microsoft.com/partner-center/develop/purchase-azure-reservations) (パートナー センター開発者向けドキュメント)

 
