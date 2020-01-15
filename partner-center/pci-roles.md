---
title: パートナーセンターの洞察-ロールベースのアクセス制御 |パートナーセンター
ms.topic: article
ms.date: 01/14/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 洞察レポートを表示するには、特定のロールが必要です。
ms.assetid: 2F4B9A27-37FF-41E4-8A26-5EAE88DD8A49
keywords: PCI、パフォーマンス、お客様の成功、測定、ロール
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.custom: seodec18
ms.openlocfilehash: e51e86ed20af16d4bc4c5d48b33eee712480bfab
ms.sourcegitcommit: 1a735003cca0bd430195ac1213bd8d77bd5063a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/14/2020
ms.locfileid: "75945864"
---
# <a name="roles-based-access-control-to-the-insights-dashboard"></a><span data-ttu-id="21a4e-104">Insights ダッシュボードへのロールベースのアクセス制御</span><span class="sxs-lookup"><span data-stu-id="21a4e-104">Roles-based access control to the Insights dashboard</span></span>

<span data-ttu-id="21a4e-105">Insights ダッシュボードでは、パートナーセンターの2つの新しいロールを使用して、レポートへの従業員のアクセスを管理します。このレポートビューアーとレポートビューアーは、</span><span class="sxs-lookup"><span data-stu-id="21a4e-105">The Insights dashboard uses two new roles in Partner Center to manage employee access to the reports - Executive Report Viewer and Report Viewer.</span></span>  <span data-ttu-id="21a4e-106">Executive レポートビューアーロールのユーザーは、すべてのレポートデータセットにアクセスできますが、レポートビューアーロールのユーザーは、収益や顧客/従業員の個人データなどの機密データセットにアクセスすることはできません。</span><span class="sxs-lookup"><span data-stu-id="21a4e-106">Users in the Executive Report Viewer role have access to all reporting datasets, while users in the Report Viewer role will not have access to sensitive data sets such as revenue and customer/employee personal data.</span></span>  

<span data-ttu-id="21a4e-107">他のパートナーセンターの役割と同様に、全体管理者またはアカウント管理者は、ユーザー管理ページでこれらのロールにユーザーを割り当てることができます。</span><span class="sxs-lookup"><span data-stu-id="21a4e-107">As with other Partner Center roles, the Global admin or the Account admin will be able to assign users to those roles on the User management page.</span></span> <span data-ttu-id="21a4e-108">ロールは、会社全体または特定の MPN の場所に適用できます。</span><span class="sxs-lookup"><span data-stu-id="21a4e-108">The roles can be applicable across the entire company or for specific MPN location(s).</span></span> <span data-ttu-id="21a4e-109">特定の MPN の場所に割り当てられたロールによって、ユーザーは、選択した MPN の場所のみに関連付けられたレポートデータを表示できます。</span><span class="sxs-lookup"><span data-stu-id="21a4e-109">Roles assigned for specific MPN location(s) limits the user to viewing reporting data associated only with the selected MPN location(s).</span></span> <span data-ttu-id="21a4e-110">パートナーは、以下のビューから1つまたは複数の場所を選択できます。</span><span class="sxs-lookup"><span data-stu-id="21a4e-110">Partner can select one or multiple locations from the below view.</span></span>

![役割](images/pci/roles.png)

><span data-ttu-id="21a4e-112">付箋2020年1月20日の MPN に管理されているユーザーは、そのテナントのすべての場所について、会社全体の "エグゼクティブレポートビューアー" ロールに自動的に追加されます。</span><span class="sxs-lookup"><span data-stu-id="21a4e-112">[Note] Users who are MPN admins as of Jan 20th, 2020 are automatically added to the company-wide ‘Executive Report Viewer’ role for all locations for that tenant.</span></span> <span data-ttu-id="21a4e-113">これらのユーザーは、全体管理者またはアカウント管理者による明示的な操作を必要とせずに、エグゼクティブレポートビューアーとしてレポートにアクセスできます。グローバル管理者とアカウント管理者は、これらのユーザーの自動割り当てされたロールを上書きして、機能をさらに強化または制限することができます。</span><span class="sxs-lookup"><span data-stu-id="21a4e-113">These users are thus able to access the reports as an Executive Report viewer without any explicit action required by Global admin or Account admin. The Global admins and Account admins can override the auto-assigned roles of these users to further increase or limit their capabilities.</span></span>