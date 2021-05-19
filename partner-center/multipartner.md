---
title: マルチパートナーのサポート
ms.topic: article
ms.date: 11/29/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 顧客が、クラウド ソリューション プロバイダー プログラムで、サービス専門分野の異なる複数のパートナーとの連携を求める場合があります。
author: dineshvu
ms.author: dineshvu
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: b41d3ee33b789c8f839ff1b3b5f5d8fd27c23f02
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/19/2021
ms.locfileid: "110151153"
---
# <a name="multi-partner-support-for-customers-who-want-to-work-with-more-than-one-partner"></a><span data-ttu-id="2655c-103">複数のパートナーと仕事をしたいお客様向けマルチパートナー サポート</span><span class="sxs-lookup"><span data-stu-id="2655c-103">Multi-partner support for customers who want to work with more than one partner</span></span>

<span data-ttu-id="2655c-104">**適用対象**: パートナー センター |パートナー センターのMicrosoft Cloud for US Government</span><span class="sxs-lookup"><span data-stu-id="2655c-104">**Applies to**: Partner Center | Partner Center for Microsoft Cloud for US Government</span></span>

<span data-ttu-id="2655c-105">**適切なロール**: グローバル管理者|ユーザー管理管理者|セールス エージェント</span><span class="sxs-lookup"><span data-stu-id="2655c-105">**Appropriate roles**: Global admin | User management admin | Sales agent</span></span>

<span data-ttu-id="2655c-106">このパートナー センターのマルチパートナー機能は、顧客が複数のパートナーと仕事をしたいと考えるシナリオをサポートします。</span><span class="sxs-lookup"><span data-stu-id="2655c-106">The Partner Center's multi-partner feature supports scenarios when a customer wants to work with more than one partner.</span></span> <span data-ttu-id="2655c-107">たとえば、お客様は Office 365 の専門知識を持つパートナーに依頼し、さらに Microsoft Azure を専門とする別のパートナーに依頼することができます。</span><span class="sxs-lookup"><span data-stu-id="2655c-107">For example, a customer may want to hire one partner for their expertise in Office 365, but hire a different partner who specializes in Microsoft Azure.</span></span>

<span data-ttu-id="2655c-108">テナントAzure CSP、別の CSP パートナーからの追加の Azure サブスクリプションを含めできます。</span><span class="sxs-lookup"><span data-stu-id="2655c-108">An Azure CSP tenant can include an additional Azure subscription from a different CSP partner.</span></span>

<span data-ttu-id="2655c-109">パートナー センターでマルチパートナー機能を使用するには、顧客を招待して代理管理特権を顧客に要求します。</span><span class="sxs-lookup"><span data-stu-id="2655c-109">To use the multi-partner feature in the Partner Center, invite the customer to give you delegated administration privileges.</span></span> <span data-ttu-id="2655c-110">既にパートナーと連携している顧客との関係付けを確立する方法については、「[顧客との再販業者関係の要求](request-a-relationship-with-a-customer.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="2655c-110">See [Request a relationship with a customer](request-a-relationship-with-a-customer.md) for information about how to establish a relationship with a customer who is already working with a partner.</span></span>

<span data-ttu-id="2655c-111">マルチパートナー機能では、次のことは行われません。</span><span class="sxs-lookup"><span data-stu-id="2655c-111">Multi-partner functionality does not:</span></span>

- <span data-ttu-id="2655c-112">顧客の既存のサブスクリプションを変更する</span><span class="sxs-lookup"><span data-stu-id="2655c-112">Change any of the customer's existing subscriptions</span></span>

- <span data-ttu-id="2655c-113">顧客の既存のサブスクリプションまたはアカウントの所有権を移行する</span><span class="sxs-lookup"><span data-stu-id="2655c-113">Transition the customer's existing subscriptions or account ownership</span></span>

- <span data-ttu-id="2655c-114">既存のサブスクリプションに対する使用条件または顧客の義務を変更する</span><span class="sxs-lookup"><span data-stu-id="2655c-114">Change the terms or customer's obligations for any of their existing subscriptions</span></span>

- <span data-ttu-id="2655c-115">サブスクリプションの指名パートナーの変更</span><span class="sxs-lookup"><span data-stu-id="2655c-115">Change the partner of record for a subscription</span></span>

> [!IMPORTANT]  
> <span data-ttu-id="2655c-116">CSP プログラムのパートナーは、現在、CSP プログラムの別のパートナーにオンライン サービスを再販することはできません。</span><span class="sxs-lookup"><span data-stu-id="2655c-116">A partner in the CSP program cannot resell online services to another partner in the CSP program currently.</span></span> <span data-ttu-id="2655c-117">この制限は、CSP 取引の実行に使用されるテナントにのみ適用されます。</span><span class="sxs-lookup"><span data-stu-id="2655c-117">This restriction only applies to the tenant used for conducting CSP transactions.</span></span> <span data-ttu-id="2655c-118">自社の社内向けに CSP 以外のテナントを使用する CSP パートナーは、別の CSP パートナーからオンライン サービスを購入できます。</span><span class="sxs-lookup"><span data-stu-id="2655c-118">CSP partners who use a non-CSP tenant for their corporate usage can purchase online services from another CSP partner.</span></span> <span data-ttu-id="2655c-119">Microsoft では、すべてのプログラムのポリシーと機能を継続的に見直してています。</span><span class="sxs-lookup"><span data-stu-id="2655c-119">Microsoft continuously reviews the policies and capabilities of all programs.</span></span> <span data-ttu-id="2655c-120">機能のリリースやポリシーの変更に関するすべての新情報は、[パートナー センターのお知らせ](announcements/index.md)など、通常の伝達方法でお知らせします。</span><span class="sxs-lookup"><span data-stu-id="2655c-120">Any news about feature releases or policy changes will be announced through the usual communications channels, including [Partner Center announcements](announcements/index.md).</span></span>
