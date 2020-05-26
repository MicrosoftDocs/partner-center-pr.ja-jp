---
title: Dynamics 365 CRM パートナーセンターの共同販売コネクタ
ms.topic: article
ms.date: 05/22/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Dynamics 365 コネクタを使用して、Microsoft からの参照を取得します。
ms.assetid: c6fca2c0-2e6c-41b1-9be8-b363b139f15b
author: LauraBrenner
ms.author: labrenne
keywords: ''
ms.localizationpriority: medium
ms.openlocfilehash: bddd29e9136d998ef8a25616d2058d1380b36665
ms.sourcegitcommit: 97f1ff7386562cbb945bdfbcf15c85bc8303cac2
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2020
ms.locfileid: "83825689"
---
# <a name="co-sell-connector-for-dynamics-365-crm--overview"></a>Dynamics 365 CRM の共同販売コネクタ–概要

### <a name="appropriate-roles"></a>適切なロール

- 紹介管理者
- CRM のシステム管理者またはシステムカスタマイザー

パートナーセンターの共同販売コネクタを使用すると、販売元は CRM システム内から Microsoft と共同で販売することができます。 パートナーセンターを使用して共同販売取引を管理するためのトレーニングを行う必要はありません。 共同販売コネクタを使用すると、Microsoft の販売者に協力したり、Microsoft 販売者からの推薦を受け取ったり、紹介を受け入れたり拒否したりすることができます。また、商談価値や決算日などの取引データを変更したり、これらの共同販売取引に関するマイクロソフト販売者からの更新を受け取ることができます。 パートナーセンターではなく、選択した CRM 内での作業中に、これらすべてを実行できます。 

このソリューションは、Microsoft のパワー自動化ソリューションに基づいており、Microsoft パートナーセンター Api を使用しています。

## <a name="before-you-install---pre-requisites"></a>をインストールする前に-前提条件

|**トピック**   |**詳細**   |**リンク**   |
|--------------|--------------------|------|
|Microsoft Partner Network ID |有効な MPN ID が必要です|[MPN](https://partner.microsoft.com/)に参加するには|
|共同販売の準備完了|お客様の IP/サービスソリューションは、共同販売の準備ができている必要があります。|[Microsoft との販売](https://partner.microsoft.com/membership/sell-with-microsoft)| 
|パートナー センター アカウント|パートナーセンターのテナントに関連付けられている MPN ID は、共同販売ソリューションに関連付けられている MPN ID と同じである必要があります。 コネクタをデプロイする前に、パートナーセンターポータルで共同販売の紹介を確認できることを確認します。|[アカウントの管理](create-user-accounts-and-set-permissions.md)|
|パートナー センターのユーザー ロール|コネクタをインストールして使用する従業員は、参照管理者である必要があります|[ユーザー ロールとアクセス許可の割り当て](create-user-accounts-and-set-permissions.md)| |Dynamics 365 CRM|CRM ユーザーロールは、システム管理者またはシステムカスタマイザーです。|[Dynamics 365 でロールを割り当てる](https://docs.microsoft.com/dynamics365/customerengagement/on-premises/customize/privileges-required-customization)|
|パワー自動化フローアカウント|CRM システム管理者またはシステムカスタマイザー用のアクティブな[電源自動化](https://flow.microsoft.com)アカウント。 そのユーザーは、インストールの前に少なくとも1回、[電源の自動](https://flow.microsoft.com)登録を行う必要があります。|

## <a name="install-partner-center-referrals-synchronization-for-dynamics-365-power-automate-solution"></a>Dynamics 365 のパートナーセンターの紹介同期をインストールする (電源自動化ソリューション) 

1. [[パワー自動化](https://flow.microsoft.com)] にアクセスし、右上隅にある [**環境**] を選択します。 これにより、使用可能な CRM インスタンスが表示されます。

2. 右上隅にあるドロップダウンから適切な CRM インスタンスを選択します。 

3. 左側のナビゲーションバーで [**ソリューション**] を選択します。

4. 上部のメニューの [ **AppSource を開く**] リンクをクリックします。

![AppSource を開く](images/cosellconnectors/openappsource.png)

5. ポップアップ画面で、 **Dynamics365 のパートナーセンターの紹介コネクタ**を検索します。  

6. [**今すぐ入手**する] ボタンをクリックし、[**続行**] をクリックします。 

7. これにより、CRM (Dynamics 365) 環境を選択してアプリケーションをインストールできるページが開きます。  使用条件に同意します。 

8. その後、[ソリューションの**管理**] ページに移動します。  ページの下部にある矢印ボタンを使用して、[パートナーセンターの紹介] に移動します。 [パートナーセンターの紹介] ソリューションの横に、[**インストールのスケジュール**] が表示されます。 インストールには10-15 分かかります。 

9. インストールが完了したら、[Power の[自動化](https://flow.microsoft.com)] に戻り、左側のナビゲーション領域から [**ソリューション**] を選択します。 **Dynamics 365 のパートナーセンターの紹介同期**は、[ソリューション] の一覧で確認できます。

10. **Dynamics 365 のパートナーセンターの紹介同期**を選択します。 次の電源の自動化フローとエンティティを利用できます。

![使用可能な CRMS](images/cosellconnectors/dynamics-available-crms.png)

## <a name="best-practice-test-before-you-go-live"></a>ベストプラクティス: 運用前にテストする

運用環境でパワー自動化ソリューションをインストール、構成、およびカスタマイズする前に、必ずステージング CRM インスタンスでソリューションをテストしてください。

- ステージング環境/CRM インスタンスに Microsoft Power 自動ソリューションをインストールします。
- ソリューションのコピーを作成し、構成を実行し、ステージング環境でフローのカスタマイズを自動化します。
- ステージング/CRM インスタンスでソリューションをテストします。 
- 成功した場合は、運用インスタンスにマネージドソリューションとしてインポートします。 

## <a name="configure-the-solution"></a>ソリューションを構成する

1. CRM インスタンスにソリューションをインストールしたら、[ [Power の自動化](https://flow.microsoft.com/)] に戻ります。

2. 右上隅にある [**環境**] ドロップダウンで、パワー自動化ソリューションをインストールした CRM インスタンスを選択します。

3. 次の3つのユーザーアカウントを関連付ける接続を作成する必要があります。 

- 参照管理者の資格情報を持つパートナーセンターのユーザー 
- パートナー センターのイベント
- Power を使用した CRM 管理ソリューションのフローが自動化されます。 

    a。 左側のナビゲーションバーから [**接続**] を選択し、一覧から "パートナーセンターの紹介" ソリューションを選択します。
    b. [**接続の作成**] をクリックして接続を作成します。 

    ![接続を作成する](images/cosellconnectors/createconnection.png)
    
    c. 右上隅の検索バーで、**パートナーセンターの参照 (プレビュー)** を検索します。
    d. 参照管理者の資格情報ロールを使用して、パートナーセンターユーザーの接続を作成します。つまり. 次に、パートナーセンターのユーザーに、参照管理者の資格情報を使用してパートナーセンターのイベント接続を作成します。f. CRM 管理者ユーザーの Common Data Service (現在の環境) の接続を作成します。

4. 電源自動化フローを接続に関連付けるには、各パワー自動化フローを編集して、Common Data Service とパートナーセンターの紹介に接続します。 変更を保存します。

5. パワー自動化フローを**有効に**します。

## <a name="next-steps"></a>次のステップ

- [Webhook を使用してリソース変更イベントを取得する](referral-connector-webhooks.md)

- [Microsoft Power の自動化プラットフォームの詳細](https://docs.microsoft.com/power-automate/)

- [見込み客を管理する](manage-leads.md)

- [共同販売の機会を管理する](manage-co-sell-opportunities.md)

