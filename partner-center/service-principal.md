---
title: Azure AD サービス プリンシパル |パートナー センター
ms.topic: article
ms.date: 12/11/2019
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Azure AD テナントにサービス プリンシパルを追加する
author: LauraBrenner
ms.author: labrenne
Keywords: Azure, Azure プラン, サービス プリンシパル, Azure AD アプリケーション
robots: ''
ms.localizationpriority: High
ms.openlocfilehash: 1fe4211879df2063f7b865c249870c49a346f518
ms.sourcegitcommit: 369aceafc54e960ac0bd3a023edc85b06361492b
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/12/2019
ms.locfileid: "75010383"
---
# <a name="add-an-azure-ad-application-service-principal-in-partner-center"></a><span data-ttu-id="5fcd2-104">パートナー センターで Azure AD アプリケーション (サービス プリンシパル) を追加する</span><span class="sxs-lookup"><span data-stu-id="5fcd2-104">Add an Azure AD application (service principal) in Partner Center</span></span>

<span data-ttu-id="5fcd2-105">パートナー センターのコマーシャル マーケットプレース プログラムでは、Azure AD アプリケーション (サービス プリンシパル) を Azure AD テナントのユーザーとして追加できるようになりました。</span><span class="sxs-lookup"><span data-stu-id="5fcd2-105">In the Commercial Marketplace program in Partner Center, you are now able to add an Azure AD application (service principal) as a user in your Azure AD tenant.</span></span> <span data-ttu-id="5fcd2-106">(これは、以前は Cloud パートナー ポータル (CPP) アカウントで実行できましたが、パートナー センターに移行したため、CPP アカウントは読み取り専用になりました。)サービス プリンシパルは Azure AD アプリケーションと同義であることに注意してください。</span><span class="sxs-lookup"><span data-stu-id="5fcd2-106">(You were able to do this previously in your Cloud Partner Portal (CPP) account, but now that you have migrated to Partner Center, the CPP acount is read-only.) Note that service principal is synonymous with Azure AD application.</span></span>

## <a name="add-an-azure-ad-application-service-principal"></a><span data-ttu-id="5fcd2-107">Azure AD アプリケーション (サービス プリンシパル) を追加する</span><span class="sxs-lookup"><span data-stu-id="5fcd2-107">Add an Azure AD application (service principal)</span></span>

1. <span data-ttu-id="5fcd2-108">パートナー センター ダッシュボードで **[設定]** を選択し、 **[開発者向け設定]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="5fcd2-108">From the Partner Center dashboard, select **Settings** and then select **Developer settings**.</span></span>

2. <span data-ttu-id="5fcd2-109">**[ユーザー]** を選択し、 **[Azure AD アプリケーションの追加]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="5fcd2-109">Select **Users** and then select **Add Azure AD Applications**.</span></span>

3. <span data-ttu-id="5fcd2-110">既存の Azure AD アプリケーションを選択するか、新しいものを作成します。</span><span class="sxs-lookup"><span data-stu-id="5fcd2-110">Select an existing Azure AD application or create a new one.</span></span>

4. <span data-ttu-id="5fcd2-111">新しい Azure AD アプリケーションを作成する場合は、次の情報を含めます。</span><span class="sxs-lookup"><span data-stu-id="5fcd2-111">If you create a new Azure AD Application, include the following information:</span></span>  
<span data-ttu-id="5fcd2-112">  
**名前\*\*:これは、CPP ポータルの [フレンドリ名] フィールドに似ています。</span><span class="sxs-lookup"><span data-stu-id="5fcd2-112">  
\*\*Name\*\*: This is similar to the ‘friendly name’ field in the CPP portal.</span></span>

<span data-ttu-id="5fcd2-113">**応答 URL**:これは、ユーザーが Azure AD アプリケーションを使用するためにサインインできる URL です。</span><span class="sxs-lookup"><span data-stu-id="5fcd2-113">**Reply URL**: This is the URL where users can sign in to use your Azure AD application.</span></span> 

<span data-ttu-id="5fcd2-114">**アプリ ID の URI**:これは、Azure AD アプリケーションの論理識別子であり、シングル サインオン要求を Azure AD に送るときに提供されます。</span><span class="sxs-lookup"><span data-stu-id="5fcd2-114">**App ID URI**: This is a logical identifier for the Azure AD application that is presented when it sends a single sign-on request to Azure AD.</span></span> 

<span data-ttu-id="5fcd2-115">**セキュリティ ロール**:**マネージャー** (CPP の '所有者' ロールと同じ) と **開発者** (CPP の 'コントリビューター' ロールと同じ) のロールは、パートナー センターのコマーシャル マーケットプレース プログラムに適用され、この Azure AD アプリケーションに関連付けることができます。</span><span class="sxs-lookup"><span data-stu-id="5fcd2-115">**Security roles**: The roles **Manager** (the same as  ‘Owner’ role in CPP) and **Developer** (the same as ‘Contributor’ role in CPP) apply to the Commercial Marketplace program in Partner Center, and they can be associated with this Azure AD Application.</span></span>  

<span data-ttu-id="5fcd2-116">**[保存]** を選択すると、パートナー センターでこれを作成するために、この情報も CPP システムに同期されます。</span><span class="sxs-lookup"><span data-stu-id="5fcd2-116">When you select **Save**,  to create this in Partner Center, the information is also synced back to the CPP system.</span></span>  
