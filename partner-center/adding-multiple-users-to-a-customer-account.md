---
title: 顧客アカウントに複数のユーザーを追加する
ms.topic: how-to
ms.date: 08/01/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 顧客のアカウントに複数のユーザーを追加するには、コンマ区切り値 (.csv) ファイル形式を使用して パートナー センター にデータ ファイルをアップロードします。
author: parthpandyaMSFT
ms.author: parthp
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 268cc9cb42bc72a444da6aec99425c2b29b71cb4
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/19/2021
ms.locfileid: "110150473"
---
# <a name="upload-a-csv-file-of-users-to-a-customers-account"></a>ユーザーの .csv ファイルを顧客のアカウントにアップロードする


**適切なロール**: グローバル管理者

コンマ区切り値ファイル形式 (.csv) のデータ ファイルを パートナー センター にアップロードして、複数のユーザーを顧客のアカウントに一度に追加します。 

## <a name="create-the-file-of-customer-users-and-upload-to-customer-account"></a>顧客ユーザーのファイルを作成し、顧客アカウントにアップロードする

1. 以下に説明するデータを使用して、コンマ区切り値 (.csv) データ ファイルを作成します。 後の手順を参照できるように、ファイルを保存します。 顧客 [アカウントの複数のユーザーをインポートするには、「.csv ファイルのフィールド」を参照してください](file-customer-users.md)。 

2. パートナー センター [ダッシュボード](https://partner.microsoft.com/dashboard)にサインインします。

3. パートナー センター メニューから **[顧客]** を選択し、一覧から顧客を選びます。

4. 顧客の [ユーザーとライセンス] **タブを選択し** 、[ユーザーのアップロード] **を選択します**。

5. **[ユーザー情報のアップロード]** の **[参照]** を選びます。

6. ファイル セレクターで、データ ファイルを選び、**[開く]** を選びます。

7. **[検証]** を選択します。

    **注:** ほとんどのアカウント作成エラーは、データ ファイルの問題が原因です。情報が不足している、メール アドレスの形式が正しくないか、重複している、ファイル内のレコードが多すぎるなどです。

8. パートナー センターでファイルが検証された後、新しいユーザーの地理的な **場所** を選びます。
9. **[保存]** を選択します。
10. ユーザーの一時パスワードの情報をダウンロードします。

    >[!IMPORTANT]
    > 一時的なパスワードを含むファイルは必ずこのときにダウンロードしてください。後でこの操作を行うことはできません。 新しいユーザーは、新しいアカウントの一時的なパスワードを使用して、新しいアカウントにログインする必要があります。

11. 新しいユーザーには、ライセンスとサービスを使用できる **のアクセス許可が自動的に割り当てられます**。 

## <a name="next-steps"></a>次のステップ

- [顧客に独自の製品パートナー センター購入するアクセス許可を付与する](give-customers-permission.md)
