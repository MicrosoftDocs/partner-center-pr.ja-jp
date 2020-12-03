---
title: ロール、パートナー獲得クレジットのアクセス許可
ms.topic: article
ms.date: 05/04/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: パートナーがパートナーの獲得クレジット (PEC) を獲得できるようにするためのロールとアクセス許可について説明します。 これらは、パートナーセンターで動作するロールとは異なります。
author: adamyeh
ms.author: adamyeh
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 8c36883dc7d12b7ea0ce8f2644dbac86595ab131
ms.sourcegitcommit: 2d9aab15ddc20cb3d9537e68ace33d36f7d8a250
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/02/2020
ms.locfileid: "96534592"
---
# <a name="roles-and-permissions-required-to-earn-partner-earned-credit"></a>パートナーの獲得クレジットを獲得するために必要なロールとアクセス許可

次のロールは、パートナーがパートナーの獲得クレジットを利用できるかどうかを判断するアクセス許可レベルにマップされます。

>[!Important]
>これらのロールとアクセス許可は、ユーザーがパートナーセンターで作業するために必要な役割とアクセス許可とは異なります。

|**ロール**   |**説明**   |**PEC 対象**   |
|-----------------|:------------------|:--------------|
|所有者  |リソースへのアクセスを含め、すべてを管理します。|はい|
|Contributor |リソースへのアクセスを許可する以外はすべて管理します。|はい|
|Reader|すべてを表示できますが、変更を加えることはできません。|いいえ|
|ACRDelete|acr の削除|はい|
|ACRImageSigner 方|ACR イメージ署名者|はい|
|ACRPull|acr のプル|はい|
|AcrPush|acr のプッシュ|はい|
|AcrQuarantineReader|ACR 検査データ閲覧者|いいえ|
|AcrQuarantineWriter| ACR 検査データ作成者|はい|
|API Management Service Contributor|サービスと API を管理できます|はい|
|API Management Service Operator Role|サービスを管理できますが、API は対象外です|はい|
|API Management Service Reader Role|サービスと API への読み取り専用アクセスです|いいえ|
|Application Insights Component Contributor|Application Insights コンポーネントを管理します|はい|
|Application Insights Snapshot Debugger|Application Insights スナップショット デバッガーで収集されたデバック スナップショットの表示とダウンロードを実行できるアクセス許可をユーザーに与えます。 これらのアクセス許可は、所有者ロールまたは共同作成者ロールには含まれないことに注意してください。|はい|
Automation ジョブ オペレーター | Automation Runbook を使用してジョブを作成および管理します。 | はい | 
Automation Operator | Automation オペレーターはジョブを開始、停止、中断、再開することができます | はい | 
Automation Runbook オペレーター | Runbook のジョブを作成する方法については、Runbook のプロパティを参照してください。 | はい | 
Avere 共同作成者 | Avere vFXT クラスターを作成および管理できます。 | はい | 
Avere オペレーター | クラスターを管理するために Avere vFXT クラスターによって使用されます | はい | 
Azure Event Hubs データ所有者 | Azure Event Hubs リソースへのフル アクセスを許可します。 | はい | 
Azure Event Hubs データ受信者 | Azure Event Hubs リソースへの受信アクセスを許可します。 | はい | 
Azure Event Hubs データ送信者 | Azure Event Hubs リソースへの送信アクセスを許可します。 | はい | 
Azure Kubernetes Service クラスター管理者ロール | クラスター管理者の資格情報アクションを一覧表示します。 | はい | 
Azure Kubernetes Service クラスター ユーザー ロール | クラスター ユーザーの資格情報アクションを一覧表示します。 | はい | 
Azure Maps データ閲覧者 (プレビュー) | Azure Maps アカウントからマップ関連データを読み取るためのアクセス権を付与します。 | いいえ | 
Azure Service Bus データ所有者 | Azure Service Bus リソースへのフル アクセスを許可します。 | はい | 
Azure Service Bus データ受信者 | Azure Service Bus リソースへの受信アクセスを許可します。 | はい | 
Azure Service Bus データ送信者 | Azure Service Bus リソースへの送信アクセスを許可します。 | はい | 
Azure Stack Registration Owner | Azure Stack の登録を管理できます。 | はい | 
Backup Contributor | バックアップ サービスを管理できますが、資格情報コンテナーの作成や他のユーザーに対するアクセス権の付与を行うことはできません | はい | 
Backup Operator | バックアップ サービスを管理できます (バックアップの削除、資格情報コンテナーの作成、他のユーザーに対するアクセス権の付与を除く) | はい | 
Backup Reader | バックアップ サービスを表示できますが、変更を行うことはできません | いいえ | 
Billing Reader | 課金データへの読み取りアクセスを許可します | いいえ | 
BizTalk Contributor | BizTalk Services を管理できます。ただし、それらへのアクセスは含まれません。 | はい | 
ブロックチェーン メンバー ノードへのアクセス (プレビュー) | ブロックチェーン メンバー ノードにアクセスできるようにします | はい | 
ブループリント共同作成者 | ブループリントの定義を管理できますが、それらを割り当てることはできません。 | はい | 
ブループリント オペレーター | 既存の発行済みのブループリントを割り当てることはできますが、ブループリントの新規作成はできません。 注: これは、ユーザーが割り当てたマネージド ID を使用して割り当てが行われた場合にのみ機能します。 | はい | 
CDN Endpoint Contributor | CDN エンドポイントを管理できますが、アクセス権を他のユーザーに付与することはできません。 | はい | 
CDN Endpoint Reader | CDN エンドポイントを表示できますが、変更はできません。 | いいえ | 
CDN Profile Contributor | CDN プロファイルとそのエンドポイントを管理できますが、アクセス権を他のユーザーに付与することはできません。 | はい | 
CDN Profile Reader | CDN プロファイルとそのエンドポイントを表示できますが、変更はできません。 | いいえ | 
Classic Network Contributor | 従来のネットワークを管理できます。ただし、それらへのアクセスは含まれません。 | はい | 
Classic Storage Account Contributor | 従来のストレージ アカウントを管理できますが、アクセスすることはできません。 | はい | 
従来のストレージ アカウント キー オペレーターのサービス ロール | 従来のストレージ アカウント キー オペレーターは、従来のストレージ アカウントでのキーの一覧表示と再生成を行うことができます | はい | 
Classic Virtual Machine Contributor | 従来の仮想マシンを管理できますが、アクセスすることはできません。また、接続先の仮想ネットワークやストレージ アカウントにもアクセスできません。 | はい | 
Cognitive Services 共同作成者 | Cognitive Services のキーの作成、読み取り、更新、削除、管理を行うことができます。 | はい | 
Cognitive Services データ閲覧者 (プレビュー) | Cognitive Services データを読み取ります。 | いいえ | 
Cognitive Services ユーザー | Cognitive Services のキーの読み取りおよび一覧表示を行うことができます。 | いいえ | 
Cosmos DB アカウントの閲覧者ロール | Cosmos DB アカウントのデータを読み取ることができます。 Azure Cosmos DB アカウントの管理については、「DocumentDB Account Contributor」をご覧ください。 | いいえ | 
Cosmos DB オペレーター | Azure Cosmos DB アカウントを管理することができます。ただし、アカウント内のデータにはアクセスできません。 アカウント キーと接続文字列へのアクセスは禁止されます。 | はい | 
CosmosBackupOperator | Cosmos DB データベースまたはアカウントのコンテナーの復元要求を送信できます | はい | 
Cost Management 共同作成者 | コストを表示し、コストの構成 (予算、エクスポートなど) を管理することができます。 | はい | 
Cost Management 閲覧者 | コストのデータと構成 (予算、エクスポートなど) を表示することができます。 | いいえ | 
Data Box Contributor | Data Box サービスですべてを管理できます (他のユーザーに対するアクセス権の付与を除く)。 | はい | 
Data Box 閲覧者 | Data Box サービスを管理できます (注文の作成または注文の詳細の編集、および他のユーザーに対するアクセス権の付与を除く)。 | いいえ | 
Data Factory Contributor | データ ファクトリまたデータ ファクトリ内の子リソースを作成し管理します。 | はい | 
Data Lake Analytics Developer | 独自のジョブを送信、監視、管理できますが、Data Lake Analytics アカウントを作成または削除することはできません。 | はい | 
Data Purger | 分析データを削除することができます。 | はい | 
DevTest Labs User | Azure DevTest Labs で仮想マシンの接続、起動、再起動、シャットダウンができます。 | はい | 
DNS Zone Contributor | Azure DNS の DNS ゾーンとレコード セットを管理できますが、それにアクセスできるユーザーを制御することはできません。 | はい | 
DocumentDB Account Contributor | Azure Cosmos DB アカウントを管理できます。 Azure Cosmos DB は以前は DocumentDB と呼ばれていました。 | はい | 
EventGrid EventSubscription 共同作成者 | EventGrid のイベント サブスクリプション操作を管理できます。 | はい | 
EventGrid EventSubscription 閲覧者 | EventGrid のイベント サブスクリプションを読み取ることができます。 | いいえ | 
HDInsight クラスター オペレーター | HDInsight クラスター構成の読み取りと変更を実行できます。 | はい | 
HDInsight ドメイン サービス共同作成者 | HDInsight Enterprise セキュリティ パッケージに必要なドメイン サービス関連の操作の読み取り、作成、変更、削除を行うことができます。 | はい | 
Intelligent Systems Account Contributor | Intelligent Systems のアカウントを管理できます。ただし、それらへのアクセスは含まれません。 | はい | 
Key Vault Contributor | キー コンテナーを管理できますが、アクセスすることはできません。 | はい | 
Lab Creator | Azure Lab アカウントで管理対象のラボを作成、管理、削除できます。 | はい | 
Log Analytics 共同作成者 | Log Analytics 共同作成者は、すべての監視データを読み取り、監視設定を編集できます。 監視設定の編集には、VM 拡張機能の VM への追加、Azure Storage からログの収集を設定できるようにするためのストレージ アカウント キーの読み取り、Automation アカウントの作成と構成、ソリューションの追加、すべての Azure リソースでの Azure Diagnostics の構成が含まれます。 | はい | 
Log Analytics 閲覧者 | Log Analytics Reader は、すべての監視データの表示と検索、およびすべての Azure リソース上の Azure Diagnostics 構成の表示など、監視設定の表示を行うことができます。 | いいえ | 
Logic App Contributor | ロジック アプリを管理できますが、アクセス権を変更することはできません。 | はい | 
Logic App Operator | ロジック アプリの読み取り、有効化、無効化ができますが、編集または更新はできません。 | はい | 
Managed Application Operator Role | マネージド アプリケーション リソースに対する読み取りとアクションの実行が可能です。 | はい | 
Managed Applications 閲覧者 | マネージド アプリおよび要求 JIT アクセスでリソースを読み取ることができます。 | いいえ | 
Managed Identity Contributor | ユーザー割り当て ID の作成、読み取り、更新、削除を行います | はい | 
Managed Identity Operator | ユーザー割り当て ID の読み取りと割り当てを行います | はい | 
管理グループ共同作成者 | 管理グループ共同作成者ロール | はい | 
管理グループ閲覧者 | 管理グループ閲覧者ロール | いいえ | 
Monitoring Contributor | すべての監視データを読み取り、監視設定を編集できます。 「Azure Monitor での役割、アクセス許可、およびセキュリティの概要」も参照してください。 | はい | 
監視メトリック パブリッシャー | Azure リソースに対するメトリックの公開を有効にします | はい | 
Monitoring Reader | すべての監視データ (メトリック、ログなど) を読み取ることができます。 「Azure Monitor での役割、アクセス許可、およびセキュリティの概要」も参照してください。 | いいえ | 
Network Contributor | ネットワークを管理できます。ただし、それらへのアクセスは含まれません。 | はい | 
New Relic APM Account Contributor | New Relic Application Performance Management のアカウントとアプリケーションを管理できます。ただし、それらへのアクセスは含まれません。 | はい | 
Reader and Data Access | すべてを表示することができますが、ストレージ アカウントや含まれるリソースの削除や作成はできません。 ストレージ アカウント キーへのアクセスを使用して、ストレージ アカウントに含まれるすべてのデータへの読み取り/書き込みアクセスも許可されます。 | はい | 
Redis Cache Contributor | Redis Caches を管理できます。ただし、それらへのアクセスは含まれません。 | はい | 
リソース ポリシーの共同作成者 (プレビュー) | (プレビュー) リソース ポリシーの作成/変更、サポート チケットの作成、リソース/階層の読み取りを実行する権限により、ユーザーを EA からバックフィルしました。 | はい | 
Scheduler Job Collections Contributor | スケジューラ ジョブ コレクションを管理できます。ただし、それらへのアクセスは含まれません。 | はい | 
Search Service Contributor | Search サービスを管理できます。ただし、それらへのアクセスは含まれません。 | はい | 
セキュリティ管理者 | Security Center のみ: セキュリティ ポリシーの表示、セキュリティ状態の表示、セキュリティ ポリシーの編集、アラートと推奨事項の表示、アラートと推奨事項の却下を行うことができます | はい | 
セキュリティ マネージャー (レガシ) | これは、レガシ ロールです。 代わりにセキュリティ管理者をご使用ください。 | はい | 
セキュリティ閲覧者 | Security Center のみ: 推奨事項とアラート、セキュリティ ポリシー、セキュリティの状態を表示することはできますが、変更することはできません | いいえ | 
Site Recovery Contributor | 資格情報コンテナーの作成とロールの割り当てを除く、Site Recovery サービスを管理できます | はい | 
Site Recovery Operator | フェールオーバーとフェールバックを実行できますが、その他の Site Recovery 管理操作は実行しません | はい | 
Site Recovery Reader | Site Recovery の状態を表示できますが、その他の管理操作は実行できません | いいえ | 
Spatial Anchors アカウント共同作成者 | アカウントで Spatial Anchors を管理します (削除は含まない) | はい | 
Spatial Anchors アカウント所有者 | アカウントで Spatial Anchors を管理します (削除も含む) | はい | 
Spatial Anchors アカウント閲覧者 | アカウントで Spatial Anchors のプロパティを検索して読み取ります | いいえ | 
SQL DB Contributor | SQL データベースを管理できます。ただし、それらへのアクセスは含まれません。 また、セキュリティ関連のポリシーまたは親 SQL Server を管理することはできません。 | はい | 
SQL マネージド インスタンス共同作成者 | SQL マネージド インスタンスと必要なネットワーク構成を管理することができますが、他のユーザーにアクセス権を付与することはできません。 | はい | 
SQL Security Manager | SQL サーバーとデータベースのセキュリティ関連のポリシーを管理できます。ただし、それらへのアクセスは管理できません。 | はい | 
SQL Server Contributor | SQL サーバーとデータベースを管理できます。ただし、それらへのアクセスや、それらのセキュリティ関連ポリシーは管理できません。 | はい | 
Storage Account Contributor | ストレージ アカウントの管理を許可します。 アカウント キーへのアクセスを提供します。これを使用して、共有キー認証を使用してデータにアクセスすることができます。 | はい | 
ストレージ アカウント キー オペレーターのサービス ロール | ストレージ アカウント アクセス キーを一覧表示および再生成できます。 | はい | 
ストレージ BLOB データ共同作成者 | Azure Storage コンテナーと BLOB の読み取り、書き込み、削除を行います。 特定のデータ操作に必要なアクションについては、「Permissions for calling blob and queue data operations (BLOB およびキューのデータの操作を呼び出すためのアクセス許可)」をご覧ください。 | はい | 
ストレージ BLOB データ所有者 | Azure Storage Blob コンテナーとデータに対するフル アクセス (POSIX アクセスの制御の割り当てを含む) を提供します。 特定のデータ操作に必要なアクションについては、「Permissions for calling blob and queue data operations (BLOB およびキューのデータの操作を呼び出すためのアクセス許可)」をご覧ください。 | はい | 
ストレージ BLOB データ閲覧者 | Azure Storage コンテナーと BLOB の読み取りと一覧表示を行います。 特定のデータ操作に必要なアクションについては、「Permissions for calling blob and queue data operations (BLOB およびキューのデータの操作を呼び出すためのアクセス許可)」をご覧ください。 | いいえ | 
Storage Blob デリゲータ | Azure AD 資格情報で署名されたコンテナーまたは BLOB 用の共有アクセス署名を作成するために使用できるユーザー委任キーを取得します。 詳細については、「ユーザー委任 SAS を作成する」を参照してください。 | はい | 
記憶域ファイル データの SMB 共有の共同作成者 | SMB 経由の Azure Storage ファイル共有に対する読み取りアクセス、書き込みアクセス、削除アクセスを許可します。 | はい | 
記憶域ファイル データの SMB 共有の管理者特権共同作成者 | SMB 経由の Azure Storage ファイル共有に対する読み取りアクセス、書き込みアクセス、削除アクセス、NTFS アクセス許可の変更アクセスを許可します。 | はい | 
記憶域ファイル データの SMB 共有の閲覧者 | SMB 経由の Azure ファイル共有に対する読み取りアクセスを許可します。 | いいえ | 
ストレージ キュー データ共同作成者 | Azure Storage キューおよびキュー メッセージの読み取り、書き込み、削除を行います。 特定のデータ操作に必要なアクションについては、「Permissions for calling blob and queue data operations (BLOB およびキューのデータの操作を呼び出すためのアクセス許可)」をご覧ください。 | はい | 
ストレージ キュー データのメッセージ プロセッサ | Azure Storage キューからのメッセージのピーク、取得、削除を行います。 特定のデータ操作に必要なアクションについては、「Permissions for calling blob and queue data operations (BLOB およびキューのデータの操作を呼び出すためのアクセス許可)」をご覧ください。 | はい | 
ストレージ キュー データ メッセージ送信者 | Azure Storage キューにメッセージを追加します。 特定のデータ操作に必要なアクションについては、「Permissions for calling blob and queue data operations (BLOB およびキューのデータの操作を呼び出すためのアクセス許可)」をご覧ください。 | はい | 
ストレージ キュー データ閲覧者 | Azure Storage キューおよびキュー メッセージの読み取りと一覧表示を行います。 特定のデータ操作に必要なアクションについては、「Permissions for calling blob and queue data operations (BLOB およびキューのデータの操作を呼び出すためのアクセス許可)」をご覧ください。 | いいえ | 
Support Request Contributor | Support request を作成して管理できます | はい | 
Traffic Manager Contributor | Traffic Manager プロファイルを管理できますが、それにアクセスできるユーザーを制御することはできません。 | はい | 
User Access Administrator | Azure リソースに対するユーザー アクセスを管理します。 | はい | 
Virtual Machine Administrator Login | ポータルで仮想マシンを表示し、管理者としてログインします | はい | 
Virtual Machine Contributor | 仮想マシンを管理できますが、アクセスすることはできません。また、接続先の仮想ネットワークやストレージ アカウントにもアクセスできません。 | はい | 
Virtual Machine User Login | ポータルで仮想マシンを表示し、通常のユーザーとしてログインします。 | はい | 
Web Plan Contributor | Web サイトの Web プランを管理できます。ただし、それらへのアクセスは含まれません。 | はい | 
Website Contributor | Web サイト (web プランではない) を管理できますが、アクセスすることはできません | はい |

## <a name="next-steps"></a>次のステップ

- [パートナー獲得クレジット - CSP の新しいコマース エクスペリエンスにおける仕組みの概要](partner-earned-credit.md)
