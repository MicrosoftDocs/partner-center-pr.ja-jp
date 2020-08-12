---
title: Azure AD サービス プリンシパル
ms.topic: how-to
ms.date: 06/03/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: サービス プリンシパルを Azure AD テナント追加する方法を確認します。 そのようにすることによってパートナー センターで Azure AD アプリケーション (サービス プリンシパル) が追加されます。
author: dhirajgandhi
ms.author: dhgandhi
ms.localizationpriority: High
ms.custom: SEOMAY.20
ms.openlocfilehash: 21ef2aaa46359570bbf13c12c5fb6c1f5eab080a
ms.sourcegitcommit: 37b0b2a7141907c8d21839de3128fb8a98575886
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/05/2020
ms.locfileid: "87811242"
---
# <a name="add-an-azure-ad-application-service-principal-in-partner-center"></a><span data-ttu-id="dcb9e-104">パートナー センターで Azure AD アプリケーション (サービス プリンシパル) を追加する</span><span class="sxs-lookup"><span data-stu-id="dcb9e-104">Add an Azure AD application (service principal) in Partner Center</span></span>

<span data-ttu-id="dcb9e-105">**適用対象**</span><span class="sxs-lookup"><span data-stu-id="dcb9e-105">**Applies to**</span></span>

- <span data-ttu-id="dcb9e-106">パートナー センター</span><span class="sxs-lookup"><span data-stu-id="dcb9e-106">Partner Center</span></span>

<span data-ttu-id="dcb9e-107">**適切なロール**</span><span class="sxs-lookup"><span data-stu-id="dcb9e-107">**Appropriate roles**</span></span>

- <span data-ttu-id="dcb9e-108">グローバル管理者</span><span class="sxs-lookup"><span data-stu-id="dcb9e-108">Global admin</span></span>

<span data-ttu-id="dcb9e-109">パートナー センターのコマーシャル マーケットプレース プログラムでは、Azure AD アプリケーション (サービス プリンシパル) を パートナー センター アカウントのユーザーとして追加できるようになりました。</span><span class="sxs-lookup"><span data-stu-id="dcb9e-109">In the Commercial Marketplace program in Partner Center, you are now able to add an Azure AD application (service principal) as a user in your Partner Center account.</span></span> <span data-ttu-id="dcb9e-110">(以前は、Cloud パートナー ポータルまたは CPP のアカウントでこれを行うことができました。</span><span class="sxs-lookup"><span data-stu-id="dcb9e-110">(You were able to do so previously in your Cloud Partner Portal, or CPP, account.</span></span> <span data-ttu-id="dcb9e-111">パートナーセンターに移行されたため、CPP アカウントは読み取り専用になります)。</span><span class="sxs-lookup"><span data-stu-id="dcb9e-111">Now that you have migrated to Partner Center, the CPP account is read-only.)</span></span>
 
>[!Note] 
><span data-ttu-id="dcb9e-112">サービス プリンシパルは、Azure AD アプリケーションと同義です。</span><span class="sxs-lookup"><span data-stu-id="dcb9e-112">Service principal is synonymous with Azure AD application.</span></span>

## <a name="add-an-azure-ad-application-service-principal"></a><span data-ttu-id="dcb9e-113">Azure AD アプリケーション (サービス プリンシパル) を追加する</span><span class="sxs-lookup"><span data-stu-id="dcb9e-113">Add an Azure AD application (service principal)</span></span>

1. <span data-ttu-id="dcb9e-114">パートナー センター ダッシュボードで **[設定]** を選択し、 **[開発者向け設定]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="dcb9e-114">From the Partner Center dashboard, select **Settings** and then select **Developer settings**.</span></span>

2. <span data-ttu-id="dcb9e-115">**[ユーザー]** を選択し、 **[Azure AD アプリケーションの追加]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="dcb9e-115">Select **Users** and then select **Add Azure AD Applications**.</span></span>

3. <span data-ttu-id="dcb9e-116">既存の Azure AD アプリケーションを選択するか、新しいものを作成します。</span><span class="sxs-lookup"><span data-stu-id="dcb9e-116">Select an existing Azure AD application or create a new one.</span></span>

4. <span data-ttu-id="dcb9e-117">新しい Azure AD アプリケーションを作成する場合は、次の情報を含めます。</span><span class="sxs-lookup"><span data-stu-id="dcb9e-117">If you create a new Azure AD Application, include the following information:</span></span>  

   - <span data-ttu-id="dcb9e-118">**応答 URL**:ユーザーが Azure AD アプリケーションを使用するためにサインインできる URL です。</span><span class="sxs-lookup"><span data-stu-id="dcb9e-118">**Reply URL**: The URL where users can sign in to use your Azure AD application.</span></span>

   - <span data-ttu-id="dcb9e-119">**アプリ ID の URI**:Azure AD アプリケーションの論理識別子であり、シングル サインオン要求を Azure AD に送るときに提供されます。</span><span class="sxs-lookup"><span data-stu-id="dcb9e-119">**App ID URI**: A logical identifier for the Azure AD application that is presented when it sends a single sign-on request to Azure AD.</span></span>

   - <span data-ttu-id="dcb9e-120">**セキュリティ ロール**:**マネージャー** (CPP の '所有者' ロールと同じ) と **開発者** (CPP の 'コントリビューター' ロールと同じ) のロールは、パートナー センターのコマーシャル マーケットプレース プログラムに適用され、この Azure AD アプリケーションに関連付けることができます。</span><span class="sxs-lookup"><span data-stu-id="dcb9e-120">**Security roles**: The roles **Manager** (the same as  ‘Owner’ role in CPP) and **Developer** (the same as ‘Contributor’ role in CPP) apply to the Commercial Marketplace program in Partner Center, and they can be associated with this Azure AD Application.</span></span>  

## <a name="next-steps"></a><span data-ttu-id="dcb9e-121">次の手順</span><span class="sxs-lookup"><span data-stu-id="dcb9e-121">Next steps</span></span>

- [<span data-ttu-id="dcb9e-122">パートナー センターのコマーシャル マーケットプレースの概要</span><span class="sxs-lookup"><span data-stu-id="dcb9e-122">Overview of the commercial marketplace in Partner Center</span></span>](csp-commercial-marketplace-overview.md)