---
title: CSP regional authorization tenant consolidation | Partner Center
description: Use these instructions to consolidate tenants for different country/regions.
ms.assetid: 749B4C6A-26BE-4942-BDA8-F08C40DF048A
author: MaggiePucciEvans
ms.openlocfilehash: 06709900a4f98c44ef0ae8505928d7c901ee8473
ms.sourcegitcommit: c47f8e765def420017abe290f2f7327eab2cbba7
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/07/2017
---
# <a name="csp-regional-authorization-tenant-consolidation"></a>CSP regional authorization tenant consolidation

**Applies to**

-  Partner Center
-  Partner Center for Microsoft Cloud for US Government
-  Partner Center for Microsoft Cloud Germany

\[Some information relates to pre-released product which may be substantially modified before it's commercially released. Microsoft makes no warranties, express or implied, with respect to the information provided here.\]

Use these instructions to consolidate tenants for different country/regions.

**注**  切り替えアカウントからプロビジョニングされた顧客のすべてのサブスクリプションとシート数を把握しておく必要があります。 Partners will be re-provisioning those same exact subscriptions with the same seat counts under the new Central CSP account as part of the migration process. Use the export list feature to help create a list of customers to move over to the centralized tenant. Partners choose to consolidate their tenants. Once consolidation is complete, Partners cannot revert to their previous state. Note that customer action is also be required.

 

## <a name="prepare-for-migration"></a>Prepare for migration


-   Log on to <https://partnercenter.microsoft.com> with the Transitioning (existing) account and take note of all customers and all of the services provisioned for those customers.

![regional customer list](images/regionalcustomer1.png)

## <a name="migrate-customer-accounts"></a>Migrate customer accounts


1.  移行中の (新規) アカウントで <https://partnercenter.microsoft.com> にログオンし、パートナー センター ダッシュボードから [顧客] 一覧に移動します。

2.  Select Customer.

3.  **[再販業者関係の要求]** をクリックします。 You are presented with a default email message to present to your customers. This message contains a URL with the org ID unique to your new Partner Center account.

4.  **顧客のアクション:** 移行したいアクティブな各顧客がこの URL にアクセスしたことを確認します。 When opening the URL, the customer is prompted to sign in to the Office 365 portal. The customer signs in using the same Org ID that they use to access the Azure and Office 365 admin portals.

5.  After signing in, the Global Admin for the customer account is prompted to submit an agreement to give delegated admin privileges to the new CSP account. If they agree, the customer selects the checkbox and agrees to authorize the relationship.

The customers will appear in the partner’s customer list after they have submitted the agreement, one by one.

## <a name="migrating-office-365-and-non-azure-usage-based-subscriptions"></a>Migrating Office 365 and non-Azure usage-based subscriptions


1.  Once your customer has signed the agreement, you can recreate their subscriptions under your Centralized Partner Tenant.

2.  パートナー センターのダッシュボードの左側のナビゲーションで、**[顧客]** をクリックします。

3.  Open the company name for the customer you want to migrate.

4.  **[サブスクリプションの追加]** をクリックします。

5.  Add the correct subscriptions and seat counts from the catalog. **移行元**のパートナー アカウントに表示されている情報を確認します。

    ![screenshot of customer list](images/regionalcustomer2.png)

6.  **[送信]** をクリックします。

これでサービスは、**移行先**のパートナー アカウントから顧客に提供されるようになります。

Repeat these steps to migrate subscriptions for all additional customers.

Before proceeding to the next section, ensure all customer subscriptions existing under the **Transitioning From** partner accounts are re-provisioned under the **Transitioning To** partner account.

**Note**  Partners must suspend subscriptions on the **Transitioning From** Partner Tenant account in Partner Center the same day that those subscriptions are transitioned and set up under the **Transitioning To** Partner Tenant account in the Partner Center to ensure double billing does not occur. Support requests will be denied for credits due to any overlap in billing that occurs from not correctly setting the **Transitioning From** subscriptions to disabled.

 

## <a name="disabling-the-office-365-subscriptions-under-the-transitioning-from-partner-account"></a>Disabling the Office 365 subscriptions under the Transitioning From partner account


**移行元**のパートナー アカウントで CSP サブスクリプションを無効にすると、それ以降の請求は停止されます。 You do not have to manually disable Azure subscriptions, because Azure subscriptions are automatically disabled during the migration process.

1.  **移行元**の CSP アカウントで <https://partnercenter.microsoft.com> にログオンし、顧客の一覧に移動します。

2.  Open the customer with subscriptions to disable, and then select the first offer to disable.
3.  サブスクリプションを **[中断]** に設定し、**[送信]** をクリックします。

    **注**  サブスクリプションを中断することによって、二重請求を防ぐことができます。

     

    サブスクリプションの一覧で、サブスクリプションに **[中断]** と表示されます。

4.  Repeat these steps for all subscriptions under the customer. すべてが **[中断]** と表示されていることを確認します。

5.  Select the next customer on the list and repeat the process of disabling all subscriptions.

## <a name="migrating-azure-usage-based-subscriptions"></a>Migrating Azure usage-based subscriptions


Note that Azure usage-based CSP subscriptions do not need to be migrated manually as in the case with Office 365 CSP subscriptions. Microsoft Azure Support can migrate the Azure subscriptions as well as all deployed services or resources from the **Transitioning From** CSP reseller accounts to the **Transitioning To** CSP reseller account. There will be no disruption of service to the customer during this transition.

1.  Ensure that the customer accounts that need Azure subscriptions migrated have accepted the agreement to be associated with the new **Transitioning To** CSP account.
2.  Partners notify Microsoft which customer accounts that have Azure subscriptions are ready to migrate, and provides those customer’s company names.
3.  Microsoft migrates the Azure usage-based subscriptions and notifies the partner when the migration is complete.
4.  The partner confirms that the Azure subscription under the **Transitioning From** CSP reseller accounts now shows suspended in the Partner Center under the customer subscriptions section.
5.  The partner confirms that the Azure subscription under the **Transitioning To** CSP reseller account now shows a status of **active** in the Partner Center under the customer subscriptions section.

    **注**  顧客のサブスクリプションを無効にしても、顧客一覧での顧客の表示は変わりません。 There is currently no option to remove customers from the list. パートナーは、今後、**移行元**アカウントからこれらの顧客にサブスクリプションを追加しないでください。

     

6.  今後、**移行元**アカウントでの課金を停止するために、すべての顧客のすべてのサブスクリプションについて、この手順を繰り返します。 The partner will receive one final invoice with a credit for the number of unused days between the day of cancellation and the last day of the billing period. No future invoices will generate after that final billing period.

### <a name="notes"></a>Notes

-   Disabling the subscription from the **Transitioning From** CSP account does not impact end customer’s service provided the service was provisioned from the **Transitioning To** CSP account prior to the disable.

-   Subscriptions cannot be used by the customer and do not generate charges when suspended or cancelled.

-   There is currently no way to remove a customer from the Customers list completely.

-   **Note**  Partners must suspend subscriptions on the **Transitioning From** Partner Tenant account in Partner Center the same day that those subscriptions are transitioned to and set up under the **Transitioning To** Partner Tenant account in the Partner Center to ensure double billing does not occur. Microsoft will not support requests for credits due to any overlap in billing which occurs from not correctly setting the **Transitioning From** subscriptions to suspended.

     

### <a name="simplify-migration-using-export"></a>Simplify migration using Export

**エクスポート機能**を使用して、新しい統合後の構造で使用する必要があるサブスクリプションをキャプチャすることができます。

1.  ダッシュボードで **[顧客]** をクリックして、既存の構造内の顧客の一覧を表示します。

2.  Open the desired customer name.

3.  **[サブスクリプション]** ページで、**[サブスクリプションのエクスポート]** をクリックしてサブスクリプションの詳細を Excel ファイルにエクスポートします。

4.  Use this list to recreate the subscriptions in your new consolidated tenant.

### <a name="api-registration"></a>API registration

この API 登録について詳しくは、[このページ](https://go.microsoft.com/fwlink/?linkid=847990)をご覧ください。

## <a name="partner-center-activity-log"></a>Partner Center Activity log


With the Activity log, partners can view a record of all customer-affecting changes made on their tenant. This helps partners track changes on a customer tenant.

**View the Activity log**

1.  パートナー センターのダッシュボードで、**[アクティビティ ログ]** リンクをクリックします。
2.  **[アクティビティ ログ]** ページで、顧客のアカウントに加えられた変更を表示します。 アクティビティ ログを日付でフィルター処理するには、**[開始]** と **[終了]** の日付を選んで、ログで選択するレコードを絞り込みます。 **[アクティビティ ログ]** 内の顧客でフィルター処理するには、検索ボックスを使用します。

**Export the Activity log**

-   **[ログのエクスポート]** をクリックして、アクティビティ ログのデータを CSV ファイルにエクスポートします。

    You can also export the customer list and the subscription list of a single customer (from the customer’s subscription page).

 

 



