---
title: コントロール パネル ベンダーとして登録する
description: パートナーセンターで、CSP パートナーシステムとパートナーセンター Api をより適切に統合できるように、パートナーセンターでコントロールパネルベンダー (CPV) として登録する方法について説明します。
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: parthpandyaMSFT
ms.author: parthp
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.date: 05/20/2020
ms.openlocfilehash: 1bfcb4de27233283b6188903b3e1f6bbdf67698c
ms.sourcegitcommit: a8adb5f044f06bd684a5b7a06c8efe9f8b03d2db
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 10/14/2020
ms.locfileid: "92031895"
---
# <a name="enroll-as-a-control-panel-vendor-to-help-integrate-csp-partner-systems-with-partner-center-apis"></a>CSP パートナー システムとパートナー センター API との統合を支援するためにコントロール パネル ベンダーとして登録する

**適用対象**

- パートナー センター

**適切なロール**

- グローバル管理者

コントロール パネル ベンダー (CPV) は、クラウド ソリューション プロバイダー (CSP) パートナーがシステムをパートナー センター API と統合するために使用できるアプリケーションを開発する独立系ソフトウェア ベンダーです。 コントロール パネル ベンダーは、パートナー センター ダッシュボードまたはパートナー センター API に直接アクセスできる CSP パートナーではありません。

現在既にコントロール パネル ベンダー (CPV) であっても、または Microsoft パートナーと協力したい新しい CPV であっても、Microsoft は CPV に、アプリケーションを登録し、クラウド ソリューション プロバイダー パートナーをサポートするため、パートナー センターに登録することを要求します。 アカウントを作成するには、CPV パートナーは、既存の CSP パートナーのテナントや既存の CPV テナントを使用するか、またはオンボード プロセスの一環として新しいテナントを作成することができます。 CPV パートナーが既存の CSP テナントを使用することを選択した場合は、個別のマルチテナントアプリケーションを作成し、それらを CPV アクティビティのパートナーセンターに登録する必要があります。 アプリケーションを CSP と CPV アプリケーションの両方として登録することはできません。 パートナー センターに登録して、アプリケーションを登録したら、パートナー センター API にアクセスできるようになります。  Microsoft は、パートナーのサンドボックス情報を使用してパートナー センターの通知経由で連絡します。 サンドボックスアカウントを既に持っている場合は、引き続き使用します。 新しいサンドボックスは必要ありません。

「[Microsoft Control Panel Vendor agreement (Microsoft コントロール パネル ベンダー契約)](https://go.microsoft.com/fwlink/?linkid=2055198)」を確認してください


## <a name="working-in-partner-center"></a>パートナー センターでの操作
パートナーセンターの CPV エクスペリエンスに登録し、CPV 契約に同意すると、次のことができるようになります。

- マルチテナントアプリケーションを管理します (アプリケーションを追加して、パートナーセンターでアプリケーションを Azure portal、登録、登録解除します)。

    >[!Note] 
    >CPV は、パートナー センター API の承認を取得するには、パートナー センターでアプリケーションを登録する必要があります。 Azure portal にアプリケーションを追加するだけでは、CPV アプリケーションはパートナー センター API に対して承認されません。 

- CPV プロファイルの表示と管理 

- CPV 機能にアクセスする必要があるユーザーを表示および管理する。 CPV が持つことができる唯一のロールは、全体管理者です。


