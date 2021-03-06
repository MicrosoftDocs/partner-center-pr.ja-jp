---
title: 請求書を読み取り、&する方法
ms.topic: article
ms.date: 06/05/2020
description: 請求書と調整ファイルについて&確認します。 請求書には、そのパートナー センタープログラム、製品、顧客全体の料金が表示されます。
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: bbdf85d20e15841189191d6b415b54c26378850e
ms.sourcegitcommit: 8dc9f28f15d9760a8363826513b4470b76b40ff3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/23/2021
ms.locfileid: "112551199"
---
# <a name="understand-your-bill-and-reconciliation-file---learn-how-to-find-them-in-partner-center"></a>請求書と調整ファイルを理解する - 請求書と調整ファイルでそれらを見つけるパートナー センター


**適切なロール**: グローバル管理者|課金管理者|管理エージェント


請求書 **は** 、(プログラム全体、すべての製品 **、パートナー センター** 顧客) すべての請求金額の概要です。 

## <a name="find-your-bill-and-reconciliation-file"></a>請求書と調整ファイルを見つける 

請求書は、ダッシュボードの [課金] ページで確認パートナー センター。 このページでは、請求履歴、支出傾向、調整ファイルを確認することもできます。 

1. パートナー センター [ダッシュボード](https://partner.microsoft.com/dashboard/home)にサインインします。 

2. 左側のメニューで、[課金] を **選択します**。 

3. 請求の状態ページで、請求書または調整ファイルを選択して、詳細な情報を確認します。 

最新の請求書へのリンクは、ページの上部にある [最後の請求書の日付のアカウント残高] で確認できます。 

以前の請求書は、[課金履歴] セクションで確認できます。 適切な年を選択し、適切な請求期間の横にあるドロップダウン矢印を選択します。 [Invoices (.pdf) の横にあるリンクを選択して、その期間の請求書をダウンロードします。 

## <a name="invoice-types"></a>請求書の種類

Microsoft は、ライセンスベースの料金 (Office 365 など) と使用量ベースの料金 (Azure など) に対して 1 つの請求書を発行し、1 回限りの料金 (Azure RI、Marketplace、Azure プランなど) に対して個別の請求書を発行します。

たとえば、次のように入力します。  

**シナリオ 1 [単一通貨]**: パートナーは 145P オファーと Office 365 ライセンスを購入しています。  

- パートナーは、Office 365 と Azure (145p) の両方の料金をカバーする 1 つの請求書 PDF と 2 つの調整ファイルを取得します。  

**シナリオ 2 [単一通貨]**: パートナーは、Azure RI、Marketplace、または Azure プランの購入と 145p の購入を行っています。

- パートナーは、Azure (145p) の料金をカバーする 1 つの請求書 PDF と 1 つの調整ファイルを取得します。 

- パートナーは、Azure 予約インスタンス (RI)、Marketplace、Azure プランの料金をカバーする別の請求書 PDF と 1 つの調整ファイルを受け取る予定です。 

**シナリオ 3 [複数通貨]**: パートナーは、DKK および Azure プランの Azure RI を EUR で購入し、EUR で 145p 購入を行っています。

- パートナーは、DKK の Azure RI の料金をカバーする 1 つの請求書 PDF と 1 つの調整ファイルを受け取る。 

- パートナーは、Azure プランの料金をカバーする 1 つの請求書 PDF と 1 つの調整ファイルを EUR で受け取る予定です。 

- パートナーは、EUR (またはパートナーの請求通貨) で 145p オファーの料金をカバーする別の請求書 PDF と 1 つの調整ファイルを受け取ります。 


## <a name="understanding-invoice-pdf"></a>請求書 PDF について 

**使用量** とライセンスベースの料金の請求書: Office 365 や Azure などのサービスの料金の請求書は、選択した請求日 (UTC) から 2 日以内に利用できます。  

**1** 回限りおよび定期的な料金の請求書: Azure RI、Azure プラン、Marketplace などのサービスの料金の請求書は、毎月 8 日より後に使用できます。  

請求書 PDF ドキュメントのキー フィールドの一部を次に示します。

**請求書番号**: それぞれの請求期間に対して生成された請求書ドキュメントの一意識別子。 

**請求期間**: これは、使用量とライセンスベースのサービスがある期間です。 

**請求書の** 日付: 請求書が毎月生成される請求日または記念日。 

**支払期限:** 支払いを受け取る必要がある日付。 

**料金**: それぞれの請求期間の請求通貨で支払う金額。 

**クレジット**: クレジット (サービス レベル アグリーメント (SLA) など) またはサブスクリプションに対して行われた変更 (ライセンスの増減など) の調整。 

**支払い方法**: 地域に基づいて請求書を支払う方法の説明。 支払いを行う場合は、必ず請求書番号を含める必要があります。 

請求書ファイル内のすべてのフィールド (1 回きり料金のフィールドを含む) の詳細については、「請求書ファイルのフィールド」 [を参照してください](invoice-file.md)。 

## <a name="understand-reconciliation-files"></a>調整ファイルについて

 料金の詳細をドリルダウンまたは項目別に提供する調整ファイルは、請求書 PDF と共にダウンロードできます。 調整ファイルには、顧客の請求書を作成するために使用できる顧客識別子とサブスクリプション識別子が含まれます。 調整ファイルの詳細については、「調整ファイルを使用 [する方法」を参照してください](use-the-reconciliation-files.md)。 

## <a name="next-steps"></a>次の手順

- [調整ファイルの使用方法](use-the-reconciliation-files.md)