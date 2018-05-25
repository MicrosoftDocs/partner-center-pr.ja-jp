---
title: Microsoft Azure VM 予約の概要 | パートナー センター
Description: Overview of selling Microsoft Azure Reserved VM Instances in CSP.
author: v-petand
keywords: Azure, 予約, VM, 管理, 請求, 購入, Azure RI, Azure Reserved VM Instances
ms.openlocfilehash: 9fac5749fda6106772d8fed28a320432206d528c
ms.sourcegitcommit: 034336ae3a697a97a62ad549b8645c836624efaa
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/11/2018
---
# <a name="sell-microsoft-azure-reserved-vm-instances"></a>Microsoft Azure Reserved VM Instances の販売 

**適用対象**

-  パートナー ダッシュボード
-  Microsoft Azure portal
-  CSP のパートナー

クラウド ソリューション プロバイダー (CSP) プログラムのパートナーは、Microsoft Azure Virtual Machines 上の予約インスタンスを顧客に提供できるようになりました。 事前に Azure Virtual Machines で領域を予約できると、顧客はコストを大幅に節約できます。 Azure Reserved VM Instances では、以下の点で簡潔さと柔軟性が顧客に提供されます。

-   1 ～ 3 年の予約期間。 
-   簡単に開始。仮想マシンを数秒でセットアップできます。 
-   予約インスタンスはいつでも取り消しまたは交換でき、払い戻しが調整されます。 
-   組織レベルまたは個々の部署レベルで予約インスタンスの使用状況を管理できます。 

Azure Reserved VM Instances について詳しくは、Microsoft Azure Web サイトの [Azure Reserved VM Instances 製品のページ](https://azure.microsoft.com/pricing/reserved-vm-instances/)と「[Better together: Azure Reserved VM Instances and server subscriptions](https://blogs.partner.microsoft.com/mpn/better-together-azure-reserved-instances-server-subscriptions/)」(Azure Reserved VM Instances とサーバー サブスクリプションの相乗効果) をご覧ください。

Azure Reserved VM Instances には、顧客から見て以下のようなメリットがあります。

-   予約インスタンスでは、従量課金制 (PAYG) の価格設定で大幅にコストを節約できます。
-   1 年間または 3 年間の前払いにより、予算編成と支払い計画が容易になります。 
-   オフィスに近い Azure リージョンでコンピューティング処理能力を優先させることができます。  
-   Azure Reservations を Microsoft Windows Server や Azure SQL Database (パートナー ダッシュボードに近日追加予定) などのソフトウェアと組み合わせることで、エンド ツー エンドのインフラストラクチャ ソリューション基盤が提供されます。   

Azure Virtual Machines のインスタンスを事前購入することによる顧客側のメリットについて詳しくは、Azure ヘルプの「[Save money on virtual machines with Reserved Virtual Machine Instances](https://docs.microsoft.com/azure/billing/billing-save-compute-costs-reservations)」 (Reserved Virtual Machine Instances で仮想マシンのコストを節約する) をご覧ください。

## <a name="before-you-begin"></a>始める前に

顧客に代わって Azure Reservations の購入を行う前に、以下の情報をご確認ください。 現時点では次のような注意点があります。

-   顧客に代わって予約を購入するには、あらかじめ顧客がアクティブな Azure サブスクリプションを持っている必要があります。  
-   Azure 予約の価格に、ソフトウェアのコストは含まれていません。 
-   販売担当者およびヘルプ デスク担当者は、顧客に代わって Azure portal で Azure サブスクリプションの購入または管理を行い、サポート要求 (交換や返金を含む) を登録できるように、Azure サブスクリプションへの明示的なアクセス許可を持っている必要があります。  
-   間接プロバイダーが Azure portal で Azure Reservations を購入する場合は、選択した Azure CSP サブスクリプションから指名パートナー (間接リセラー) が継承されます。 
-   Azure Reservations の指名パートナーを購入後に変更することはできません。 既存の予約を取り消して、新しい指名パートナーで新しい予約を購入することもできます。 
-   顧客が Azure サブスクリプションを直接サブスクリプションまたは EA サブスクリプションから CSP に移行した場合、予約は移行されません。 

>[!NOTE]
> Azure 予約インスタンスは、パートナー ダッシュボード、Azure portal、およびパートナー ダッシュボード API を使用して購入、販売、管理できます。 方法については、各リンク先をご覧ください。 

## <a name="azure-reservations-resources"></a>Azure Reservations に関するリソース
|**情報**   |**参照先**    |
|:-----------------------------|:-----------------|
|パートナー ダッシュボードで顧客の Azure Reservations を購入する   |[Azure Reservations の購入](azure-reservations-buying.md)
|Azure Reservations の請求   |[Azure Reservations の請求](azure-reservations-billing.md)   |
|パートナー ダッシュボードで Azure Reservations を管理する | [パートナー ダッシュボードで Azure Reservations を管理する](azure-reservations-manage.md)
|適切な VM サイズの判断と顧客による VM 使用状況の確認   |[最大限の Azure 予約使用に備えた VM サイズ](azure-usage.md)   |
|Azure portal で Azure Reservations を購入する | [Azure Reserved VM Instances による仮想マシン料金の前払い](https://docs.microsoft.com/azure/virtual-machines/windows/prepay-reserved-vm-instances) (Azure ヘルプ) |
|Azure portal で Azure Reservations を管理する   |[予約済み VM インスタンスの管理](https://docs.microsoft.com/azure/billing/billing-manage-reserved-vm-instance) (Azure ヘルプ)  |
|パートナー センター API を使用して Azure Reservations を購入する | [Azure Reserved VM Instances の購入](https://docs.microsoft.com/partner-center/develop/purchase-azure-reserved-vm-instances) (パートナー センター開発者向けドキュメント)

 

