---
title: Azure サブスクリプションを別のパートナーに譲渡する
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 顧客の Azure サブスクリプションにクラウド ソリューション プロバイダープログラム パートナーを変更する方法について説明します。
ms.custom: SEOMAY.20
ms.localizationpriority: medium
author: dhirajgandhi
ms.author: dhgandhi
ms.date: 02/09/2021
ms.openlocfilehash: 94f79762e7fabb377b8d7b559ff9ba2623b135fe
ms.sourcegitcommit: 7a6836bd962d5b426a8cb34a9132a87cbbbf39f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/13/2021
ms.locfileid: "109856068"
---
# <a name="learn-how-to-transfer-a-customers-azure-subscriptions-to-another-partner"></a>顧客の Azure サブスクリプションを別のパートナーに転送する方法について学習する

**適用対象**: パートナー センター |パートナー センターのMicrosoft Cloud for US Government

**適切なロール**: グローバル管理者

この記事では、顧客が顧客のサービスを 1 Microsoft Azure (CSP) クラウド ソリューション プロバイダー切り替える方法について説明します。

顧客の Azure サービスまたはサブスクリプションを別のパートナーに切り替えるには、次の手動の手順に従います。 パートナーと顧客の両方が手順を完了する必要があります。

>[!Note]  
>現時点では、直接プロバイダーまたは間接プロバイダーだけがサブスクリプションを譲渡できます。
>Azure プラン、Office 365、Enterprise Mobility Suite、または Microsoft Dynamics CRM サブスクリプションに関連付けられている クラウド ソリューション プロバイダー サブスクリプションのパートナーを変更できない。

## <a name="switch-partners-for-azure-subscriptions"></a>Azure サブスクリプションのパートナーを切り替える

1. Azure サブスクリプションを新しいパートナーに譲渡するには、顧客がプロセスを開始し、書面で現在の指名パートナーに連絡する必要があります。

   >[!Note]
   > 切り替えのプロセスを開始するサービス チケットは、現在のパートナーの責任で作成してください。 Microsoft は、顧客または新しいパートナーの代わりに介入することはできません。 顧客は現在のパートナーと協力して、切り替えをスムーズに進める計画を作成する必要があります。

2. サブスクリプションのパートナーは、次のタスクを実行する必要があります。

   パートナー センターから Azure サービス チケットを作成して、サブスクリプションの切り替えを要求します。

   1. パートナー センターのメニューで **[顧客]** を選び、一覧から顧客を選んで、**[サービス管理]** を選びます。

   2. **[サポート チケット]** セクションで **[新しいチケット]** ドロップダウン リストを選び、**[Microsoft Azure]** を選びます。
   
   3. [新 [しい](https://portal.azure.com)Azure portal] で、[新しい **サポート 要求] を選択します**。
   
   4. 手順 1 で、問題の種類として **[サブスクリプション管理]** を選び、切り替えるサブスクリプション ID を指定して、サポート プランとして **[クラウド ソリューション プロバイダー]** を選びます。
   
   5. 手順 2 で **[C-Minimal impact]を** 選択し、問題の種類 **として [その** 他の一般的な質問] を選択します。
   
   6. [CSP サブスクリプションの譲渡フォーム](https://query.prod.cms.rt.microsoft.com/cms/api/am/binary/RWwTWC)をダウンロードします。

3. サブスクリプションのパートナーは、[CSP サブスクリプションの譲渡フォーム](https://query.prod.cms.rt.microsoft.com/cms/api/am/binary/RWwTWC)に入力して署名し、フォームを顧客に送信します。 

   フォームに入力するには、次の情報が必要です。

   - 現在のパートナーの連絡先情報と Microsoft ID。 パートナー センター メニューで、**[アカウント設定]** &gt; **[組織プロファイル]** を選び、表示される **[Microsoft ID]**、**[組織名]**、および **[住所]** を使います。

   - 顧客の Microsoft ID。 パートナー センター メニューで、**[顧客]** を選び、顧客の一覧を展開して顧客の **[Microsoft ID]** を表示します。

   - 切り替えるサブスクリプション ID。 展開した顧客一覧で、**[サブスクリプションの表示]** を選び、選んだサブスクリプションを展開して **[サブスクリプション ID]** を表示します。

   >[!Note]
   >サブスクリプションを譲渡すると、サブスクリプション ID が 2 つになり、譲渡したサブスクリプションの **[サブスクリプションの編集]** ページに両方が表示されます。請求には、**1** のパートナー センターのサブスクリプション ID が使われます。 **2** の元の Azure サブスクリプション ID も保持され、パートナー センターと Azure 管理ポータルに表示されます。 調整ファイルに表示されるのはこの ID です。  **サポート チケットを記録するときは、両方の ID を使う必要があります。**

4. 顧客とサブスクリプションの新しいパートナーが、次の操作を行います。

   フォームを確認し、新しいパートナーに関する情報を入力し、それに署名します。 新しい顧客が適切な契約書を持っていることを確認します。 フォームを現在の指名パートナーに送信します。

   *重要*: 新しい CSP パートナーが顧客とリセラーの関係を持てない場合は、サブスクリプションを譲渡する前に、パートナーがリセラー関係を確立する必要があります。 [これを行う方法については、こちらをご覧ください](request-a-relationship-with-a-customer.md)。

   >[!Note]
   >新しい CSP パートナーと顧客のテナントは、同じ国に存在する必要があります。 

5. 現在のパートナーが次の操作を行います。

   フォームに両方のパートナー管理者の連絡先情報が含まれる必要があります。 Microsoft サポート、両方の管理者に連絡して転送を確認します。 3 つの署名が 3 つすべての署名を持っている必要があります。 次に、[ **ファイルのアップロード]** オプションを使用して、完成したフォームを既存のサービス要求に添付します。 Microsoft サポート エンジニアから 8 営業時間以内に返送され、レシートと完了が検証されます。

6. 新しいパートナーは次の操作を行います。

   Azure サブスクリプションの設定を更新して、アカウントから古いパートナーを削除します。 プロビジョニングされるロールの割り当てを確認するには、2 つの PowerShell Commandlet を実行します。

   - アカウントのリセラーとして新しいパートナーを追加します。

     ```powershell
     Connect-AzAccount -Tenant 'xxxx-xxxx-xxxx-xxxx'
     ```

     >[!NOTE]
     > 顧客のテナント **ID は、パートナー センター** の Microsoft ID として **表示されます**。 特定の顧客の Microsoft ID (テナント ID) を検索するには、パートナーセンターの [ダッシュボード](https://partner.microsoft.com/dashboard)にサインインします。 次に、メニューから **Customers** を選択します。 一覧で顧客を見つけます。 下矢印を選択して、顧客の一覧を展開します。 顧客の *ドメイン名* と顧客の **Microsoft ID** に関する情報が表示されます。 PowerShell コマンドレットで16桁の **MICROSOFT ID** を使用します。

   - 前の CSP パートナーを含めて、アカウントの役割を表示します。

     ```powershell
     Get-AzRoleAssignment
     ```

7. 期限切れのアクセス許可を削除する:

   - パートナー センター メニューで、**[顧客]** を選びます。
   - 一覧で顧客を見つけます。 会社名を選択します (ダブルクリック)。 この操作により、[顧客の **サブスクリプション** ] ページが開きます。
   - [Customer detail] メニューで、[ **Service management**] を選択します。
   - [ **Microsoft Azure** で、リンクを選択して **Microsoft Azure の管理ポータル** にアクセスします。

## <a name="next-steps"></a>次の手順

- [CSP サブスクリプションの譲渡フォーム](https://query.prod.cms.rt.microsoft.com/cms/api/am/binary/RE4ATIA)をダウンロードします。

- [マルチパートナーサポート](multipartner.md)について説明します。

- [マルチパートナーサポート](multipartner.md)。
- [マルチチャネルのサポート](multichannel.md)。
- [Azure サブスクリプションの譲渡](/azure/cost-management-billing/manage/transfer-subscriptions-subscribers-csp)