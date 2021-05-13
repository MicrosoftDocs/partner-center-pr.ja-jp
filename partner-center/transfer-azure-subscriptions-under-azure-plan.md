---
title: Azure プランで Azure サブスクリプションを別の CSP パートナーに譲渡する
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Azure プランで、クラウド ソリューション プロバイダーの Azure サブスクリプションに関連付けられているプログラム パートナーを変更する方法について説明します。
ms.custom: SEOMAY.20
ms.localizationpriority: medium
author: mckennaville
ms.author: mcville
ms.date: 07/29/2020
ms.openlocfilehash: dcacc6da51fe40c7eb05997f5409ef5fadbcf693
ms.sourcegitcommit: 7a6836bd962d5b426a8cb34a9132a87cbbbf39f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/13/2021
ms.locfileid: "109856051"
---
# <a name="transfer-a-customers-azure-plan-subscriptions-to-a-different-partner"></a>顧客の Azure プラン サブスクリプションの別のパートナーへの譲渡

**適切なロール**: アカウント管理者|Sales Agent |課金エージェント

この記事では、顧客が Azure プランで Azure サブスクリプションを 1 つのサブスクリプション (CSP) クラウド ソリューション プロバイダー切り替える方法について説明します。

顧客の Azure サブスクリプションを別のパートナーから切り替えるには、次の手順に従います。 パートナーと顧客の両方に、完了する手順があります。

>[!Note]  
>移行ツールにアクセスできるのは、Microsoft との直接請求関係を持つパートナーのみです。 間接リセラーは、この移行ツールを利用するために間接プロバイダーと一緒に作業する必要があります。

このツールを利用する前に、顧客は両方のパートナー (現在と将来) と会話している必要があります。 混乱やチャーンを避けるためには、オフラインの会話を行う必要があります。 さらに、パートナーと顧客は、移行を開始する前に、次の考慮事項と前提条件を理解する必要があります。

**主な考慮事項:**

- Azure の予約は、今後のパートナーにサブスクリプションと一緒に移動しない
- 現在のパートナーの Azure サービスの CSP 価格は切り替えされない  
- お客様に対するサポート責任は、将来のパートナーに移行します
- 請求と請求は、転送時に将来のパートナーに移行されます
- Azure Role-Based Access Control (RBAC) は転送の影響を受けない
- 代理管理者 (AOBO) は、既定では将来のパートナーに付与されません
- サード パーティのマーケットプレース製品は、製品が Marketplace の適格性チェックに合格している限り転送されます。
    - 特別な割引や地域の制限はありません
    - 製品は非サブスクリプション ベースです
    - 将来のパートナーは、発行元と一緒に、製品の展開の許可リストに記載されている必要があります
    - Marketplace 製品を譲渡するためにこれらの条件のすべてが満たされない場合は、取り消し、Azure サブスクリプションを譲渡してから、新しいパートナーと Marketplace 製品を再購入する必要があります

**前提条件:**

- お客様は、移行の意図について現在の CSP パートナーと関わる
- 将来の CSP パートナーが顧客と提携し、顧客のニーズを満たすことができます
- 将来の CSP パートナーが顧客との関係を確立し、移行を開始する前に Azure プランを購入する  
- 顧客は、将来の CSP Microsoft 顧客契約してサインインする必要があります
- 将来の CSP パートナーは、このツールを使用するためにMicrosoft Partner Agreement署名している必要があります

## <a name="customer-tasks-to-be-completed"></a>完了する顧客のタスク

Azure プランで Azure サブスクリプションを譲渡するには、顧客は現在のパートナーに連絡してプロセスを開始する必要があります。 将来のパートナーが代理で譲渡要求フォームを完了できるよう、現在のパートナーの会社名とドメインを収集する必要があります。

顧客は、現在のパートナーから譲渡するサブスクリプションも特定する必要があります。 Office 365、Enterprise Mobility Suite、または Microsoft Dynamics CRM サブスクリプションのパートナーを変更できない。

>[!Note]  
>譲渡プロセスを開始する譲渡要求フォームを完了する責任は、将来のパートナーの責任です。 Microsoft は、お客様または現在のパートナーに代わって介入することはできません。 顧客は、移行を円滑に進め、将来および現在のパートナーと密接に取り組む予定です。

## <a name="future-partner-tasks-to-be-completed"></a>今後のパートナー タスクの完了

サブスクリプションの将来のパートナーは、サブスクリプションの譲渡を要求するために、パートナー センターから譲渡要求フォームを完了する必要があります。

1.  [顧客] パートナー センター [顧客] を選択し、代理で譲渡要求フォームに入力する顧客を選択します。
2.  [顧客] メニューの [サブスクリプション] **を選択します**。
3.  [要求の **転送] セクションを** 選択します。
4.  [要求の転送 **] セクションで、[新** しい要求の **追加] を選択します**。

    :::image type="content" source="images/modernazuretransfers/Transferrequestheader.png" alt-text="[転送] セクション":::

5.  [新しい **転送要求] フォームに入力** します。

6.  [転送要求 **の送信] を**  >  **選択します**。

    :::image type="content" source="images/modernazuretransfers/CompleteTrnasferRequestForm.png" alt-text="[転送要求の完了] フォーム":::

7.  転送要求の確認の確認

    :::image type="content" source="images/modernazuretransfers/TransferPending.png" alt-text="保留中の転送を確認する":::

    >[!Note]
    >今後のパートナーは、転送要求の状態が"保留中" の場合にのみ、右上隅にある [キャンセル要求] を選択して、転送要求を取り消します。 転送要求の状態が "進行中" または "完了" の場合、取り消しはできません。

## <a name="current-partner-tasks-to-be-completed"></a>完了する現在のパートナー タスク

顧客の現在のパートナーの管理エージェントは、顧客がサブスクリプションの譲渡を要求しているという電子メールを受け取る:

:::image type="content" source="images/modernazuretransfers/SourceReviewEmail.png" alt-text="確認":::

サブスクリプションの譲渡を完了するには、パートナー センター要求フォームを確認して同意します。

>[!Note]  
>現在のパートナーが 30 日以内にアクションを実行した場合、要求は期限切れになります。今後のパートナーは、新しい譲渡要求を作成する を持つ必要があります。

1.  電子メール **から [転送要求の** 確認] を選択するか、
1.  [顧客] パートナー センター [顧客]を選択し、転送要求が代理で送信された顧客を選択します。
2.  [顧客] メニューの [サブスクリプション] **を選択します**。
3.  [要求の **転送] セクションを** 選択します。
4.  [受信した要求] で選択した転送要求 ID を **選択して** 、転送 **情報を展開します**

:::image type="content" source="images/modernazuretransfers/ReviewRequest.png" alt-text="ソース レビュー転送要求":::

5.  譲渡要求を確認します。 転送する要求された Azure サブスクリプションを選択します。

>[!Note]  
> 続行する前に、選択したサブスクリプションにアクセスできなくなります。
> 今後の使用のために請求されることはありません。
> Azure の予約は、サブスクリプションと共には転送されません。

6.  次に、[ **受け入れて転送** ] を選択して、転送プロセスを完了します。

:::image type="content" source="images/modernazuretransfers/SelectSubs.png" alt-text="Azure プランで転送するサブスクリプションを選択します":::

7.  転送の受け入れ確認を表示します。

   この時点で、今後のパートナー、顧客、および現在のパートナーには、電子メールで受け入れられた譲渡要求が通知されます。

   その後、移行が受け入れられると、システムが更新されている間、転送状態が最大15分間保留状態のままになることがあります。 時間がかかると、システムは3日間試行し続けます。 転送の状態が保留中のままである場合、パートナーはサービス要求を送信する必要があります。

   転送が完了すると、要求内に含まれているサブスクリプションが、今後のパートナーの Azure プランに表示され、お客様と共に表示されなくなります。

>[!Note]  
>間接プロバイダーの場合: 譲渡要求が受け入れられたことを間接リセラーに知らせてください。

### <a name="managing-your-transferred-customer-subscriptions"></a>転送された顧客サブスクリプションの管理

- 移転中、Azure ロールベースのアクセス制御 (RBAC) を使用して割り当てられた既存のユーザー、グループ、またはサービス プリンシパルへのアクセスは影響を受けません。 Azure のロールベースのアクセス制御 [(AZURE RBAC)](/azure/role-based-access-control/overview) を使用すると、顧客は、azure リソースにアクセスできるユーザー、それらのリソースを使用して実行できること、およびアクセス権を持つ領域を管理できます。 新しいパートナーとして、サブスクリプションの譲渡後に、お客様のリソースに対する RBAC アクセス権は付与されません。 お客様の以前のパートナーは、RBAC アクセスを維持しています。 お客様と協力して、サブスクリプションについての洞察を持つユーザーと、必要な変更を行う方法を理解します。

- そのため、お客様は前のパートナー向けの Azure RBAC アクセスを削除し、新しいパートナーのアクセス権を追加することが重要です。 新しいアクセス権を付与する顧客の詳細については、「Azure ロールベースのアクセス制御 [(Azure RBAC) とは」を参照してください。](/azure/role-based-access-control/overview) 顧客が以前のパートナーの RBAC アクセスを削除する方法の詳細については、「ロールの割り当てを削除 [する」を参照してください](/azure/role-based-access-control/role-assignments-portal#remove-a-role-assignment)。

- さらに、サブスクリプションへの代理管理者 [(AOBO)](https://channel9.msdn.com/Series/cspdev/Module-11-Admin-On-Behalf-Of-AOBO) アクセス権は自動的に取得されません。 パートナーが顧客に代わって顧客の Azure サブスクリプションを管理するには、AOBO が必要です。 Azure の特権の詳細については、「顧客のサービスまたはサブスクリプションを管理するためのアクセス許可を [取得する」を参照してください。](./customers-revoke-admin-privileges.md)

## <a name="next-steps"></a>次のステップ:

- [(Azure RBAC)](/azure/role-based-access-control/overview)
- [顧客のサービスまたはサブスクリプションを管理するためのアクセス許可を取得します。](./customers-revoke-admin-privileges.md)
