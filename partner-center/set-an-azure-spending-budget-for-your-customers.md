---
title: 顧客の Azure 支出予算を設定する
ms.topic: how-to
ms.date: 03/17/2021
description: 顧客の毎月の Azure 支出予算を設定または削除する方法と、Azure の支出データを表示し、予算関連の通知を設定する方法について説明します。
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 14e901f51841e58b28a3cbbb1b7a19ce89d7c324
ms.sourcegitcommit: 7a6836bd962d5b426a8cb34a9132a87cbbbf39f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/13/2021
ms.locfileid: "109855354"
---
# <a name="set-check-or-remove-monthly-azure-spending-budgets-for-customers-in-partner-center"></a>顧客の月間 Azure 支出予算を設定、確認、または削除パートナー センター

**適切なロール**: 管理エージェント

顧客に [対して毎月の Azure 支出予算を](#set-azure-spending-budget) 設定するには、パートナー センター。 これは、顧客が Azure の支出を管理するのに役立ちます。 このオプションを使用すると、顧客の Azure 支出を月の予算と比較できます。 また、月次請求が予想よりも高くないほど、顧客が Azure の支出を予算化するのにも役立ちます。

> [!NOTE]  
> この機能は、サンドボックスまたは Test in Production (TIP) アカウントでは使用できません。

顧客の [Azure 支出予算を](#set-azure-spending-budget)設定した後は、次の方法で顧客の使用状況を確認できます。 これらのオプションは、正しく構成されていないサービスや、不正行為を示唆する可能性がある異常な傾向を見つけるのに役立つ場合があります。 その後、顧客と一緒に作業し、根本原因を特定し、コストを管理できます。 必要に応じて、顧客 [の予算を高い](#set-azure-spending-budget) 金額に変更できます。

- [Azure の現在の支出を確認する](#check-current-azure-spending)

- [顧客の支出が予算の上限に近い場合の電子メール通知を有効にする](#notifications-for-budget-limits)

- [使用量ベースのサブスクリプションのサービス別の項目別コストを表示する](#itemized-costs-by-service)

顧客の [Azure 支出予算](#remove-azure-spending-budget) は、いつでも削除できます。

## <a name="azure-spending-data"></a>Azure の支出データ

Azure の支出データは見積 *もりであり* 、 *実際の請求金額は異なる場合があります*。 データの値には *、税金* 、クレジット、調整、または適用される可能性があるその他の料金は反映されません。

支出データは *、1 日に 1 回更新されます*。 顧客は、Azure サービスとリソースのアカウント設定を変更しない限り、引き続き Azure サービスとリソースを使用Azure portal。

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

3. **Azure** の支出ページの **[Microsoft Azure** サブスクリプションを持つ顧客] では、顧客の毎月の予算、現在の支出の見積もり、使用されている予算の割合の概要を確認できます。

## <a name="notifications-for-budget-limits"></a>予算制限に関する通知

顧客の *毎月の支出が* 予算の上限に近い場合の電子メール通知を有効にできます。 このオプションを有効にすると、顧客が月次予算の 80% 以上を使用すると通知されます。 このオプションは、Azure の請求書を見守るのに役立ちます。 電子メール通知を構成するには:

1. パートナー センターにサインインします。

2. **[設定]** に移動します。

3. [自分 **の設定] を選択します**。

4. ない場合は、優先メール アドレスを構成します。

5. 通知の優先言語を構成します。

6. [通知 **の基本設定** ] セクションの **[CSP] タブを** 選択します。

7. Azure 支出通知の [電子メール **] オプションをオン** にし、 を保存 **します**。


## <a name="itemized-costs-by-service"></a>サービス別の明細化されたコスト

使用量ベース *のサブスクリプションのサービス別に*、項目化されたコスト (および推定使用量) を表示できます。

1. パートナー センターにサインインします。

2. 左側のメニューの **[CSP]** で、[顧客] を **選択します**。

3. [顧客 **] ページ** で、顧客の [会社名] **を選択します**。

4. 顧客の [サブスクリプション] **ページの** [ **使用量ベースの** サブスクリプション] で、サブスクリプション の名前を選択 **します**。

5. サブスクリプションのページで、サービス別の項目化されたコストと、当月の推定使用量を確認できます。


## <a name="next-steps"></a>次の手順

- [CSP の新しいコマース エクスペリエンス - Azure の請求](azure-plan-billing.md)
