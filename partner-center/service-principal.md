---
title: Azure AD サービス プリンシパル
ms.topic: article
ms.date: 06/03/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: サービス プリンシパルを Azure AD テナント追加する方法を確認します。 そのようにすることによってパートナー センターで Azure AD アプリケーション (サービス プリンシパル) が追加されます。
author: dhirajgandhi
ms.author: dhgandhi
Keywords: Azure, Azure プラン, サービス プリンシパル, Azure AD アプリケーション
robots: ''
ms.localizationpriority: High
ms.custom: SEOMAY.20
ms.openlocfilehash: bd2880f57d1ccb3c3675fef4fae7499f7ac02f4b
ms.sourcegitcommit: 36a60f672c1c3d6b63fd225d04c5ffa917694ae0
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/03/2020
ms.locfileid: "85949630"
---
# <a name="add-an-azure-ad-application-service-principal-in-partner-center"></a><span data-ttu-id="26842-105">パートナー センターで Azure AD アプリケーション (サービス プリンシパル) を追加する</span><span class="sxs-lookup"><span data-stu-id="26842-105">Add an Azure AD application (service principal) in Partner Center</span></span>

<span data-ttu-id="26842-106">パートナー センターのコマーシャル マーケットプレース プログラムでは、Azure AD アプリケーション (サービス プリンシパル) を パートナー センター アカウントのユーザーとして追加できるようになりました。</span><span class="sxs-lookup"><span data-stu-id="26842-106">In the Commercial Marketplace program in Partner Center, you are now able to add an Azure AD application (service principal) as a user in your Partner Center account.</span></span> <span data-ttu-id="26842-107">(以前は、Cloud パートナー ポータルまたは CPP のアカウントでこれを行うことができました。</span><span class="sxs-lookup"><span data-stu-id="26842-107">(You were able to do so previously in your Cloud Partner Portal, or CPP, account.</span></span> <span data-ttu-id="26842-108">パートナーセンターに移行されたため、CPP アカウントは読み取り専用になります)。</span><span class="sxs-lookup"><span data-stu-id="26842-108">Now that you have migrated to Partner Center, the CPP account is read-only.)</span></span>
 
>[!Note] 
><span data-ttu-id="26842-109">サービス プリンシパルは、Azure AD アプリケーションと同義です。</span><span class="sxs-lookup"><span data-stu-id="26842-109">Service principal is synonymous with Azure AD application.</span></span>

## <a name="add-an-azure-ad-application-service-principal"></a><span data-ttu-id="26842-110">Azure AD アプリケーション (サービス プリンシパル) を追加する</span><span class="sxs-lookup"><span data-stu-id="26842-110">Add an Azure AD application (service principal)</span></span>

1. <span data-ttu-id="26842-111">パートナー センター ダッシュボードで **[設定]** を選択し、 **[開発者向け設定]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="26842-111">From the Partner Center dashboard, select **Settings** and then select **Developer settings**.</span></span>

2. <span data-ttu-id="26842-112">**[ユーザー]** を選択し、 **[Azure AD アプリケーションの追加]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="26842-112">Select **Users** and then select **Add Azure AD Applications**.</span></span>

3. <span data-ttu-id="26842-113">既存の Azure AD アプリケーションを選択するか、新しいものを作成します。</span><span class="sxs-lookup"><span data-stu-id="26842-113">Select an existing Azure AD application or create a new one.</span></span>

4. <span data-ttu-id="26842-114">新しい Azure AD アプリケーションを作成する場合は、次の情報を含めます。</span><span class="sxs-lookup"><span data-stu-id="26842-114">If you create a new Azure AD Application, include the following information:</span></span>  

   - <span data-ttu-id="26842-115">**応答 URL**:ユーザーが Azure AD アプリケーションを使用するためにサインインできる URL です。</span><span class="sxs-lookup"><span data-stu-id="26842-115">**Reply URL**: The URL where users can sign in to use your Azure AD application.</span></span>

   - <span data-ttu-id="26842-116">**アプリ ID の URI**:Azure AD アプリケーションの論理識別子であり、シングル サインオン要求を Azure AD に送るときに提供されます。</span><span class="sxs-lookup"><span data-stu-id="26842-116">**App ID URI**: A logical identifier for the Azure AD application that is presented when it sends a single sign-on request to Azure AD.</span></span>

   - <span data-ttu-id="26842-117">**セキュリティ ロール**:**マネージャー** (CPP の '所有者' ロールと同じ) と **開発者** (CPP の 'コントリビューター' ロールと同じ) のロールは、パートナー センターのコマーシャル マーケットプレース プログラムに適用され、この Azure AD アプリケーションに関連付けることができます。</span><span class="sxs-lookup"><span data-stu-id="26842-117">**Security roles**: The roles **Manager** (the same as  ‘Owner’ role in CPP) and **Developer** (the same as ‘Contributor’ role in CPP) apply to the Commercial Marketplace program in Partner Center, and they can be associated with this Azure AD Application.</span></span>  
