---
title: 顧客アカウントの複数のユーザーをインポートするための .csv ファイルのフィールド
ms.topic: article
ms.date: 08/01/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 顧客アカウントに複数のユーザーを追加するには、適切なフィールドを含むコンマ区切り値 (.csv) ファイルを作成します。
author: parthpandyaMSFT
ms.author: parthp
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 8ba08d97f1d360eae5af1941ed36753addd24939
ms.sourcegitcommit: 3c26a61982082787bbdaf5d1e92553b26f3a5076
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/06/2021
ms.locfileid: "106441423"
---
# <a name="add-multiple-users-to-a-customer-account-by-creating-a-csv-file"></a>.Csv ファイルを作成して顧客アカウントに複数のユーザーを追加する

**適切なロール**

- グローバル管理者

コンマ区切り値ファイル形式 (.csv) のデータファイルをパートナーセンターにアップロードすることで、顧客のアカウントに複数のユーザーを一度に追加します。 パートナー センターからサンプル データ ファイルをダウンロードし、それを編集して使用することも、以下に定義するデータ モデルを使用して新しいデータ ファイルを作成することもできます。

## <a name="data-file-requirements"></a><a href="" id="creatingtheimportcsvfile"></a>データ ファイルの要件

一括アップロードプロセスを使用して顧客のアカウントに複数のユーザーを追加するには、次の要件を満たす必要があります。

- 顧客アカウントに対してグローバル管理者のアクセス許可が必要です。
- 各ユーザーは、顧客の電子メール ドメインに追加された、一意のメール アドレスを持っている必要があります。
- 一度に最大 100 個のレコードをアップロードすることができます。 100 を超えるユーザーを追加する必要がある場合は、追加のデータ ファイルを作成してアップロードします。
- すべてのユーザーは、地理的に同じ **場所** にいる必要があります。
- 次に示すデータのみを入力します。 余分なデータがあると、アップロードに失敗します。

データ ファイルに、次のデータを入力します。

| **列名** | **説明**  | **制限事項**  |
|:-------- |:------  |:----- |
| 名  | ユーザーの名 (オプションフィールド)  | 50 字以内  |
| 姓  | ユーザーの姓 (省略可能なフィールド)  | 50 字以内  |
| Display name    | パートナー センターで表示される名前 (必須フィールド)                            | 50 字以内                         |
| Email   | 顧客会社のユーザーの勤務先の電子メールアドレス (必須フィールド)           | 各ユーザーに一意の電子メール アドレスが必要 |
| 状態の更新   | 新しいユーザーレコードが正常に作成されたかどうかを示すために使用されます | \*\*空白のままにする\*\*                        |

## <a name="next-steps"></a>次のステップ

- [顧客に複数ユーザーを追加する方法](adding-multiple-users-to-a-customer-account.md)