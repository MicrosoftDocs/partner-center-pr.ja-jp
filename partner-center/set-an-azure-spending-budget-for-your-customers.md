---
title: 顧客の Azure 支出予算を設定する
ms.topic: how-to
ms.date: 03/17/2021
description: 顧客向けの月単位の Azure 支出予算を設定または削除する方法と、Azure の支出データを表示し、予算に関連する通知を設定する方法について説明します。
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: eaf54898d7a130ca38e5a2aaeba279fb722c9e66
ms.sourcegitcommit: e8e8362d2777d25efac3e1076af5939765ed13d0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/20/2021
ms.locfileid: "104712751"
---
# <a name="set-check-or-remove-monthly-azure-spending-budgets-for-customers-in-partner-center"></a>パートナーセンターのお客様に対する月単位の Azure 支出予算を設定、確認、または削除する

**適切なロール**

- 管理エージェント

パートナーセンターでは、 [顧客の Azure 支出予算を毎月設定](#set-azure-spending-budget) できます。 これにより、お客様は Azure の支出を管理できます。 このオプションを使用すると、顧客の Azure の支出を月の予算と比較できます。 また、お客様が Azure の使用量を予算に費やして、月々の請求額が予想よりも高くならないようにすることもできます。

> [!NOTE]  
> この機能は、サンドボックスまたは Test in Production (TIP) アカウントでは使用できません。

[顧客の Azure 支出予算を設定](#set-azure-spending-budget)した後、次の方法で顧客の使用状況を確認することもできます。 これらのオプションを使用すると、正しく構成されていないサービスや、不正行為の可能性がある異常な傾向を特定できます。 その後、顧客と協力して根本原因を特定し、コストを管理できます。 必要に応じ [て、お客様の予算](#set-azure-spending-budget) をより高い金額に変更することもできます。

- [現在の Azure の支出を確認する](#check-current-azure-spending)

- [顧客の支出が予算制限に近づいたときの電子メール通知を有効にする](#notifications-for-budget-limits)

- [使用量ベースのサブスクリプションのサービス別コストを表示する](#itemized-costs-by-service)

また、お客様の [Azure 支出予算](#remove-azure-spending-budget) をいつでも削除することもできます。

## <a name="azure-spending-data"></a>Azure の支出データ

Azure の支出データは *見積もり* で *あり、実際の請求金額は異なる場合があり* ます。 データの値には、適用される可能性がある税金、クレジット、調整、またはその他の料金は反映され *ません* 。

支出データは 1 *日に1回更新* されます。 Azure portal でアカウントの設定を変更しない限り、お客様は Azure のサービスとリソースを引き続き使用できます (料金が発生します)。

## <a name="set-azure-spending-budget"></a>Azure の支出予算を設定する

パートナーセンターでは、複数の顧客に対する *月単位の Azure 支出予算を設定* できます。

1. [パートナー センター ダッシュボード](https://partner.microsoft.com/dashboard/)にサインインします。

2. [ **CSP**] の左側のメニューで、[ **Azure の支出**] を選択します。

3. [ **Azure** の使用量] ページの [ **Microsoft Azure サブスクリプションを持つ顧客**] で、予算を設定する顧客を選択します。

4. **月単位の予算** の値を入力します。

5. [ **適用** ] を選択して変更を保存します。

また、サブスクリプション設定で *個々の顧客の予算を設定* することもできます。

1. パートナー センター ダッシュボードにサインインします。

2. [ **CSP**] の左側のメニューで、[ **Customers**] を選択します。

3. [ **顧客** ] ページで、顧客の **会社名** を選択します。

4. 顧客の [ **サブスクリプション** ] ページの [ **使用量ベースのサブスクリプション**] で、[ **予算の変更**] を選択します。

5. 予算の値を入力します。

6. [ **適用** ] を選択して変更を保存します。

## <a name="remove-azure-spending-budget"></a>Azure の支出予算の削除

パートナーセンターでは、お客様の *月単位の Azure 支出予算を削除* できます。

1. [パートナー センター ダッシュボード](https://partner.microsoft.com/dashboard/)にサインインします。

2. [ **CSP**] の左側のメニューで、[ **Azure の支出**] を選択します。

3. [ **Azure** の使用量] ページの [ **Microsoft Azure サブスクリプションを持つ顧客**] で、予算を削除する顧客を選択します。

4. [ **予算の削除**] を選択します。

## <a name="check-current-azure-spending"></a>現在の Azure の支出を確認する

*お客様の現在の Azure の支出と月々の予算* をいつでも追跡できます。

1. [パートナー センター ダッシュボード](https://partner.microsoft.com/dashboard/)にサインインします。

2. [ **CSP**] の左側のメニューで、[ **Azure の支出**] を選択します。

3. [ **Azure** の使用量] ページで、[ **Microsoft Azure のサブスクリプションをお持ちのお客様**] の下に、顧客の月々の予算、現在の支出見積もり、使用された予算の割合の概要が表示されます。

## <a name="notifications-for-budget-limits"></a>予算制限の通知

お客様の月々の支出が予算制限に近づいたときに、 *電子メール通知を有効* にすることができます。 このオプションをオンにすると、顧客が80% 以上の月間予算を使用した場合に通知が表示されます。 このオプションを使用すると、Azure の課金内容を監視できます。 電子メール通知を構成するには:

1. パートナー センターにサインインします。

2. **[設定]** に移動します。

3. [ **個人用設定**] を選択します。

4. お持ちでない場合は、優先する電子メールアドレスを構成します。

5. 通知の優先言語を構成します。

6. [**通知の設定**] セクションの [ **CSP** ] タブを選択します。

7. **Azure** の使用量に関する通知の電子メールオプションを確認し、**保存** します。


## <a name="itemized-costs-by-service"></a>サービス別コストの明細

*使用状況に基づいたサブスクリプションのサービスごとに、明細のコスト (および推定使用量) を表示* できます。

1. パートナー センターにサインインします。

2. [ **CSP**] の左側のメニューで、[ **Customers**] を選択します。

3. [ **顧客** ] ページで、顧客の **会社名** を選択します。

4. 顧客の [ **サブスクリプション** ] ページの [ **使用量ベースのサブスクリプション**] で、 **サブスクリプション** の名前を選択します。

5. サブスクリプションのページで、サービスごとの **明細コスト** と当月の **推定使用量** を確認できます。


## <a name="next-steps"></a>次のステップ

- [CSP の新しいコマース エクスペリエンス - Azure の請求](azure-plan-billing.md)
