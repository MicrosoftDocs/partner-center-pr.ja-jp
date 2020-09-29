---
title: Azure プランで Azure サブスクリプションを別の CSP パートナーに転送する
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Azure プランで顧客の Azure サブスクリプションに関連付けられているクラウドソリューションプロバイダープログラムパートナーを変更する方法について説明します。
ms.custom: SEOMAY.20
ms.localizationpriority: medium
author: mckennaville
ms.author: mcville
ms.date: 07/29/2020
ms.openlocfilehash: e1b70f26dc146507ac3764ae223ca27915162f0c
ms.sourcegitcommit: 3329fd120d8d49a4831412b79e044678ec71b84c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/29/2020
ms.locfileid: "91422570"
---
# <a name="transfer-a-customers-azure-plan-subscriptions-to-a-different-partner"></a>顧客の Azure プランサブスクリプションを別のパートナーに譲渡する

## <a name="applies-to"></a>適用対象

- クラウド ソリューション プロバイダー (CSP) プログラムのパートナー

この記事では、顧客が azure プランの Azure サブスクリプションを1つのクラウドソリューションプロバイダー (CSP) から別のクラウドソリューションプロバイダー (CSP) に切り替える方法について説明します。

顧客の Azure サブスクリプションを別のパートナーから切り替えるには、次の手順を実行します。 パートナーと顧客の両方に対して、手順を完了する必要があります。

>[!Note]  
>Microsoft との直接の課金関係を持つパートナーだけが、移行ツールにアクセスできます。 間接リセラーは、この移行ツールを活用するために間接プロバイダーと協力する必要があります。

お客様は、このツールを利用する前に、両方のパートナー (現在と将来) との話し合いを行う必要があります。 オフラインのメッセージ交換では、混乱とチャーンを避ける必要があります。 また、移行を開始する前に、パートナーと顧客がこれらの考慮事項と前提条件を理解しておく必要があります。

**主な考慮事項:**

- Azure Reservations は、今後のパートナーにサブスクリプションと共に移動することはありません
- 現在のパートナーの Azure サービスの CSP 価格は移行されません  
- お客様のサポート責任が将来のパートナーに移行されます
- 課金と請求は、転送時に将来のパートナーに移行されます
- Azure のロールベースの Access Control (RBAC) は、転送の影響を受けません。
- (AOBO) の代理管理者は、既定では今後のパートナーに付与されません
- 製品が Marketplace の適格性チェックに合格している限り、サードパーティの marketplace 製品は譲渡されます。
    - 特別な割引や地域の制限はありません
    - 製品は非サブスクリプションベースです
    - 将来のパートナーは、発行元と協力して、製品の展開の許可リストに含まれていることを確認する必要があります。
    - これらのすべての条件が満たされていない場合は、Marketplace 製品をキャンセルし、Azure サブスクリプションを譲渡した後、新しいパートナーと共に Marketplace 製品を再購入します。

**前提条件:**

- お客様が現在の CSP パートナーを移行の目的で利用
- 将来の CSP パートナーがお客様と連携して顧客のニーズを満たすことができるようにする
- 将来の CSP パートナーが、移行を開始する前に顧客との関係を確立する  
- お客様は、今後の CSP パートナーと共に Microsoft カスタマー契約に署名する必要があります
- このツールを使用するには、今後の CSP パートナーが Microsoft パートナー契約に署名している必要があります

## <a name="customer-tasks-to-be-completed"></a>完了する顧客タスク

Azure プランで Azure サブスクリプションを譲渡するには、お客様は現在のパートナーに連絡してプロセスを開始する必要があります。 パートナーは、現在のパートナーの会社名とドメインを収集する必要があります。これにより、将来のパートナーが代理で転送要求フォームを完了できるようになります。

また、お客様は、現在のパートナーから譲渡するサブスクリプションを特定する必要があります。 Office 365、Enterprise Mobility Suite、または Microsoft Dynamics CRM サブスクリプションのパートナーを変更することはできません。

>[!Note]  
>譲渡プロセスを開始する転送要求フォームを完了するのは、今後のパートナーの責任です。 Microsoft は、お客様または現在のパートナーに代わって介入することはできません。 お客様は、将来と現在のパートナーと密接に連携して、移行を円滑に進めることを計画する必要があります。

## <a name="future-partner-tasks-to-be-completed"></a>今後のパートナータスクの完了

サブスクリプションの今後のパートナーは、パートナーセンターから譲渡要求フォームを完了して、サブスクリプションの譲渡を要求する必要があります。

1.  パートナーセンターメニューから、[ **顧客**] を選択し、代理で転送要求フォームを完了する顧客を選択します。
2.  カスタマーメニューから [ **サブスクリプション**] を選択します。
3.  [ **転送要求** ] セクションを選択します。
4.  [ **転送要求] セクション**で、[ **新しい要求の追加**] を選択します。

    :::image type="content" source="images/modernazuretransfers/Transferrequestheader.png" alt-text="転送セクション":::

5.  **新しい転送要求**フォームに入力します。

6.  [**転送要求**の送信] を選択し  >  **Send**ます。

    :::image type="content" source="images/modernazuretransfers/CompleteTrnasferRequestForm.png" alt-text="転送要求の完了フォーム":::

7.  転送要求の確認の確認

    :::image type="content" source="images/modernazuretransfers/TransferPending.png" alt-text="保留中の転送の確認":::

    >[!Note]
    >将来のパートナーは、転送要求の状態が [保留中] の場合にのみ、右上隅にある **[要求のキャンセル]** を選択して、譲渡要求を取り消すことができます。 転送要求の状態が "進行中" または "完了" になると、取り消しはできなくなります。

## <a name="current-partner-tasks-to-be-completed"></a>完了する現在のパートナータスク

お客様の現在のパートナーの管理者エージェントは、お客様がサブスクリプションの譲渡を要求しているという電子メールを受け取ります。

:::image type="content" source="images/modernazuretransfers/SourceReviewEmail.png" alt-text="レビュー":::

パートナーセンターから譲渡要求フォームを確認して同意し、サブスクリプションの譲渡を完了します。

>[!Note]  
>現在のパートナーが30日以内にアクションを実行しなかった場合は、要求の有効期限が切れ、今後のパートナーは新しい転送要求を作成するためにを使用します。

1.  [電子メールからの **転送要求のレビュー** ] を選択します。
1.  パートナーセンターメニューから [ **顧客**] を選択し、譲渡要求が送信された顧客を選択します。
2.  カスタマーメニューから [ **サブスクリプション**] を選択します。
3.  [ **転送要求** ] セクションを選択します。
4.  [**受信した要求**] で選択した**転送要求 ID**を選択して、[転送情報] を展開します。

:::image type="content" source="images/modernazuretransfers/ReviewRequest.png" alt-text="ソースレビューの譲渡要求":::

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

- そのため、お客様は前のパートナー向けの Azure RBAC アクセスを削除し、新しいパートナーのアクセス権を追加することが重要です。 顧客が新しいアクセス権を付与する方法の詳細については、「 [azure のロールベースのアクセス制御 (AZURE RBAC) とは](/azure/role-based-access-control/overview)」を参照してください。 以前のパートナーの RBAC アクセスを削除する顧客の詳細については、「 [ロールの割り当てを削除する](/azure/role-based-access-control/role-assignments-portal#remove-a-role-assignment)」を参照してください。

- さらに、サブスクリプションへ [の (AOBO) アクセスの代理](https://channel9.msdn.com/Series/cspdev/Module-11-Admin-On-Behalf-Of-AOBO) として自動的に管理者を取得することはありません。 AOBO は、パートナーが顧客の Azure サブスクリプションを代理として管理するために必要です。 Azure の特権の詳細について[は、「顧客のサービスまたはサブスクリプションを管理するためのアクセス許可を取得する](/partner-center/customers-revoke-admin-privileges)」を参照してください。

## <a name="next-steps"></a>次のステップ:

- [(Azure RBAC)](/azure/role-based-access-control/overview)
- [顧客のサービスまたはサブスクリプションを管理するためのアクセス許可を取得します。](/partner-center/customers-revoke-admin-privileges)