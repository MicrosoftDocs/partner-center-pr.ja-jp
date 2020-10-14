---
title: 共同販売紹介コネクタのトラブルシューティング
ms.topic: how-to
ms.date: 09/21/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 共同販売コネクタの使用に関してよく寄せられる質問への回答について説明します。 共同販売コネクタのトラブルシューティング方法については、こちらの FAQ を参照してください。
author: sroy
ms.author: sroy
ms.localizationpriority: medium
ms.openlocfilehash: 988a696a8a0a0abb4d37e3915c76f905ec5b35b0
ms.sourcegitcommit: a8adb5f044f06bd684a5b7a06c8efe9f8b03d2db
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 10/14/2020
ms.locfileid: "92031265"
---
# <a name="troubleshoot-co-sell-referrals-connectors"></a>共同販売紹介コネクタのトラブルシューティング

**適用対象:**

- パートナー センター
- Dynamics 365 CRM
- Salesforce CRM

**適切なロール**

- 紹介管理者
- CRM のシステム管理者またはシステムカスタマイザー

 ## <a name="questions-and-answers-about-pre-requisites"></a>前提条件に関する質問と回答

1. お使いの環境に対して試用版の共同販売紹介コネクタソリューションを使用できますか。

テスト/ステージング環境を使用している場合は、試用版ソリューションを選択できます。 このコネクタの有料バージョンは、AppSource で米国ドルの 15/月でご利用いただけます。 有料接続では、1日あたり10K の API 呼び出しを取得します。 コネクタは、パートナーセンターの参照 Api の上にあるラッパーです。 パートナーセンターまたは CRM 側の営業案件で、コネクタソリューションが **作成** または **更新** イベントに対して実行されるたびに、API 呼び出しが行われます。

2. CRM 環境でセクションを作成するにはどのような役割が必要ですか。

システム管理者またはシステムカスタマイザーのユーザーは、すべてのユーザーに変更を適用できます。 ただし、すべてのアプリユーザーがシステムをカスタマイズしたり、カスタマイズの一部を他のユーザーと共有したりすることもできます。 

3. パートナー販売者は、パートナーセンターで作業するために特別な役割を必要としていますか。
 
パートナーの販売元には、"紹介管理者" ロールが割り当てられている必要があります。 詳細については、次の「アクセス許可の概要」を参照してください (作成-ユーザーアカウントと-設定-アクセス許可)。

4. CRM 環境で最初にどのようなフィールドを設定する必要がありますか。 

•お客様の地域に合った通貨を使用していること、および CRM 環境に正確に対応していることを確認してください。 • Crm ユーザーとして CRM 環境に販売チームが一覧表示されている必要があります。

5. 環境の作成を自動化するために必要な前提条件は何ですか。

電力自動化環境を使用するには、次のものが必要です。

- Power 自動ライセンス認証が必要です。
- 少なくとも 1 GB のストレージが必要です。

6.  Salesforce コネクタソリューションを使用するには、Dynamics 365 サブスクリプションが必要ですか?

Salesforce コネクタソリューションの種類は "Dynamics Flow" で、他の CRM システムとの同期をサポートしています。 このソリューションでは、Dynamics 365 インスタンスまたはサブスクリプションが必要ではありません。 Salesforce ソリューションをインストールするときに、会社内の既存の CD 環境を含むドロップダウンが表示されることがあります。 その環境を選択する必要があります。 さらに、"サインインしたユーザーに接続された Dynamics 365 組織が見つかりませんでした" というエラーが表示された場合は、コネクタ用に新しい環境を作成する必要があります。

## <a name="questions-and-answers-about-configuration"></a>構成に関する質問と回答

1. パワー自動化プラットフォームでフローをアクティブ化しているときに、次のエラーが発生した場合はどうすればよいですか?

エラー: Azure Resource Manager への要求が失敗しました。エラー: ' {"エラー": {"code": "WorkflowTriggerNotFound"、"message": "ワークフロー ' e14d00f1-1fdf-4b1b-aaac-54a5064093d3 ' トリガー ' manual ' が見つかりませんでした。"}} '。 

次のトラブルシューティング手順に従います。

- CD 接続を削除してから、CD 接続を再作成してください。
- 子フローをオフまたはオンにする 
- ソリューションを削除してから、ソリューションを再インストールしてください。 

2.  Power オートメーションプラットフォームでパートナーセンターコネクタを追加するときに "サインイン" エラーが発生した場合はどうすればよいですか?

:::image type="content" source="images/cosellconnectors/failure.png" alt-text="サインインが必要なエラーメッセージ":::

このトラブルシューティングの手順に従います。

- パートナーセンターの資格情報を使用して、flow 環境に1回サインインします (flow.microsoft.com)。


3. Power オートメーションプラットフォームでパートナーセンターから CRM へのフローをアクティブにするときに、次のエラーが発生した場合はどうすればよいですか?
 
:::image type="content" source="images/cosellconnectors/powererror.png" alt-text="サインインが必要なエラーメッセージ":::

次のトラブルシューティング手順に従います。

- パートナーセンターを CRM フローにアクティブ化する前に、まず次の2つの子フローをアクティブ化します。
      - パートナーセンターから CRM ヘルパーへ (Insider Preview)
      - パートナーセンターの Microsoft 共同販売の CRM の参照の更新 (Insider Preview)

4. フローを編集しようとすると、フローに接続を追加できない場合はどうすればよいですか。

フローの実行中にフローへの接続を追加し、各フローに個別に追加します。  フローの編集中に接続を追加するダイアログボックスが自動的に開かない場合は、フローの各ステップとサブステップを個別に編集できます。

- 各フローを選択し、個別に編集します。
- フロー内のすべてのステップを展開する 

:::image type="content" source="images/cosellconnectors/flowsteps.png" alt-text="サインインが必要なエラーメッセージ":::

- 接続の関連付けと接続の追加を求める警告アイコンが表示される手順を選択します。 

:::image type="content" source="images/cosellconnectors/editflow.png" alt-text="サインインが必要なエラーメッセージ":::


5. 共同販売参照コネクタソリューションのフローが有効になっていない場合はどうすればよいですか。

A. Power の自動化では、次の順序でフローを編集し、正しい接続を使用するように更新する必要があります。

- パートナーセンターの Webhook の登録 (Insider Preview)
- パートナーセンターへの共同販売参照の作成-Salesforce (Insider Preview)
- パートナーセンター: Microsoft 共同での Salesforce の参照の更新 (Insider Preview)
- パートナーセンターから Salesforce へ (Insider Preview)
- Salesforce からパートナーセンターへ (Insider Preview)
- パートナーセンターへの Salesforce の営業案件 (Insider Preview)
- パートナーセンターへの Salesforce Microsoft ソリューション (Insider Preview)

 B. 各フローに対して、[ **ユーザーのみ実行** ] オプションを選択します。 [**実行専用ユーザーによって提供される**のではなく、**接続を使用する**] を選択します。  

:::image type="content" source="images/cosellconnectors/runonly.png" alt-text="サインインが必要なエラーメッセージ":::


C. 以下のフローフローをアクティブにします。

 - パートナーセンター: Microsoft 共同での Salesforce の参照の更新 (Insider Preview)

- Salesforce からパートナーセンターへ (Insider Preview)

    
D. 残りのすべてのフローをアクティブ化します。

E. Flow パートナーセンターの Webhook 登録で、[ **実行**] を選択します。 **パートナーセンター**の最初のアクションから Salesforce flow に**http url**を指定します。 [ **登録するイベント** ] の下にある4つのオプションをすべて選択し、[上書き] で [ **はい]** を選択します。

## <a name="questions-and-answers-about-runmaintenance"></a>実行/メンテナンスに関する質問と回答

1. 電源自動化フロー実行中にエラーが発生した場合のトラブルシューティング方法

フローが期待どおりに実行されるようにし、実行中のエラーをトラブルシューティングするには、 [フローエラーの修正](/power-automate/fix-flow-failures)に関する記述を参照してください。

2. パートナーセンターまたは CRM 環境で適切に同期されていない参照が表示される場合は、どうすればよいですか。
 
参照同期の状態を確認するには、[ **監査**] を選択します。 

:::image type="content" source="images/cosellconnectors/synch.png" alt-text="サインインが必要なエラーメッセージ":::

次の条件が満たされていることを確認します。

- ソリューション id は、営業案件の一部として提供されます。

- 2文字の国コードが必要です。

- 営業案件について Microsoft からのヘルプが選択されている場合は、顧客の連絡先情報が必要です。

3. 参照を双方向に同期させる方法

手順は次のとおりです。

- パートナーの販売者は、CRM セクションで **パートナーセンターオプションとの同期** を有効にしていることを確認する必要があります。

:::image type="content" source="images/cosellconnectors/enablesynch.png" alt-text="サインインが必要なエラーメッセージ" として閉じられていないことを確認します。

## <a name="next-steps"></a>次の手順

- [見込み客を管理する](manage-leads.md)
 
- [共同販売の機会を管理する](manage-co-sell-opportunities.md)