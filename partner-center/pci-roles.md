---
title: パートナー センター Insights のロールベースのアクセス
ms.topic: article
ms.date: 05/19/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 分析情報レポートを表示するために必要な特定のパートナー センターについて説明します。 これには、エグゼクティブ レポート ビューアーとレポート ビューアーのロールが含まれます。
author: shganesh-dev
ms.author: shganesh
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 803c299311f129c4842a92a27abd9b9addb49f17
ms.sourcegitcommit: 7a6836bd962d5b426a8cb34a9132a87cbbbf39f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/13/2021
ms.locfileid: "109854436"
---
# <a name="role-based-access-control-to-the-partner-center-insights-dashboard"></a><span data-ttu-id="14297-104">パートナー センター Insights ダッシュボードへのロールベースのアクセス制御</span><span class="sxs-lookup"><span data-stu-id="14297-104">Role-based access control to the Partner Center Insights dashboard</span></span>

<span data-ttu-id="14297-105">**適切なロール**: グローバル管理者|管理エージェント |レポート ビューアー |エグゼクティブ レポート ビューアー</span><span class="sxs-lookup"><span data-stu-id="14297-105">**Appropriate roles**: Global admin | Admin agent | Report viewer | Executive report viewer</span></span>

<span data-ttu-id="14297-106">Insights ダッシュボードでは、レポートへの従業員のアクセスを管理パートナー センターレポート ビューアーとレポート ビューアーの 2 つの新しいロールが使用されます。</span><span class="sxs-lookup"><span data-stu-id="14297-106">The Insights dashboard uses two new roles in Partner Center to manage employee access to the reports - Executive Report Viewer and Report Viewer.</span></span>  <span data-ttu-id="14297-107">エグゼクティブ レポート ビューアー ロールのユーザーは、すべてのレポート データセットにアクセスできます。一方、レポート ビューアー ロールのユーザーは、収益や顧客/従業員の個人データなどの機密データ セットにアクセスできます。</span><span class="sxs-lookup"><span data-stu-id="14297-107">Users in the Executive Report Viewer role have access to all reporting datasets, while users in the Report Viewer role will not have access to sensitive data sets such as revenue and customer/employee personal data.</span></span>  

<span data-ttu-id="14297-108">他のロールパートナー センターと同様に、グローバル管理者またはアカウント管理者は、[ユーザー管理] ページでそれらのロールにユーザーを割り当てることができます。</span><span class="sxs-lookup"><span data-stu-id="14297-108">As with other Partner Center roles, the Global admin or the Account admin will be able to assign users to those roles on the User management page.</span></span> <span data-ttu-id="14297-109">ロールは、会社全体または特定の MPN の場所に適用できます。</span><span class="sxs-lookup"><span data-stu-id="14297-109">The roles can be applicable across the entire company or for specific MPN location(s).</span></span> <span data-ttu-id="14297-110">特定の MPN の場所に割り当てられたロールは、選択した MPN の場所に関連付けられているレポート データのみを表示するユーザーを制限します。</span><span class="sxs-lookup"><span data-stu-id="14297-110">Roles assigned for specific MPN location(s) limit the user to viewing reporting data associated only with the selected MPN location(s).</span></span> <span data-ttu-id="14297-111">パートナーは、次のビューから 1 つ以上の場所を選択できます。</span><span class="sxs-lookup"><span data-stu-id="14297-111">Partner can select one or multiple locations from the below view.</span></span>

:::image type="content" source="images/pci/roles.png" alt-text="レポート ビューアーとエグゼクティブ レポート ビューアーパートナー センター Insights ロールの場所固有の設定を表示します。":::

>[!Note]
> <span data-ttu-id="14297-113">2020 年 1 月 20 日の MPN 管理者であるユーザーは、そのテナントのすべての場所について、会社全体の **エグゼクティブ** レポート ビューアー ロールに自動的に追加されます。</span><span class="sxs-lookup"><span data-stu-id="14297-113">Users who are MPN admins as of Jan 20th, 2020 are automatically added to the company-wide **Executive Report Viewer** role for all locations for that tenant.</span></span> <span data-ttu-id="14297-114">そのため、これらのユーザーは、グローバル管理者またはアカウント管理者が明示的な操作を行わずに、レポートにエグゼクティブ レポート ビューアーとしてアクセスできます。グローバル管理者とアカウント管理者は、これらのユーザーの自動割り当てロールをオーバーライドして、その機能をさらに増やしたり制限したりすることができます。</span><span class="sxs-lookup"><span data-stu-id="14297-114">These users are thus able to access the reports as an Executive Report viewer without any explicit action required by Global admin or Account admin. The Global admins and Account admins can override the auto-assigned roles of these users to further increase or limit their capabilities.</span></span>

## <a name="next-steps"></a><span data-ttu-id="14297-115">次の手順</span><span class="sxs-lookup"><span data-stu-id="14297-115">Next steps</span></span>

- <span data-ttu-id="14297-116">[パートナー センター Insights とそのさまざまなレポート](partner-center-insights.md)の詳細を確認してください。</span><span class="sxs-lookup"><span data-stu-id="14297-116">Learn more about [Partner Center Insights](partner-center-insights.md) and its various reports.</span></span>
