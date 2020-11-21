---
title: 譲渡資格–請求先アカウント間でのサブスクリプションの譲渡に関するガイドライン (Azure Marketplace)
description: Azure portal 内の請求先アカウント間でサブスクリプションを転送する前の商用小切手のガイドライン。
ms.prod: marketplace-customer
ms.topic: conceptual
author: Guyshu
ms.author: gushuchm
ms.date: 11/20/2020
ms.openlocfilehash: a6a3c8954643ea982ae5107ae417a900ed51e77d
ms.sourcegitcommit: 1aa43438ad181278052788f15e017f9ae7777943
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/21/2020
ms.locfileid: "95007220"
---
# <a name="transfer-eligibility-for-a-subscription-between-billing-accounts"></a><span data-ttu-id="e1c01-103">課金アカウント間のサブスクリプションの資格を譲渡する</span><span class="sxs-lookup"><span data-stu-id="e1c01-103">Transfer eligibility for a subscription between billing accounts</span></span>

<span data-ttu-id="e1c01-104">[サブスクリプションは](/azure/cost-management-billing/understand/subscription-transfer)、Azure portal の [課金] セクションで、1つの請求アカウントから別のアカウントに転送できます。</span><span class="sxs-lookup"><span data-stu-id="e1c01-104">You can [transfer a subscription](/azure/cost-management-billing/understand/subscription-transfer) from one billing account to another in the billing section of the Azure portal.</span></span> <span data-ttu-id="e1c01-105">転送前に、サードパーティ製品のサブスクリプションがスキャンされます。</span><span class="sxs-lookup"><span data-stu-id="e1c01-105">Prior to a transfer, the subscription is scanned for third-party products.</span></span> <span data-ttu-id="e1c01-106">転送は *すべて* の製品に対してクリアされている場合にのみ許可されます (以下の [条件](#criteria-for-transfer-approval-or-denial) を参照)。</span><span class="sxs-lookup"><span data-stu-id="e1c01-106">The transfer is permitted only if *all* products are cleared for transfer (see the [criteria](#criteria-for-transfer-approval-or-denial) below).</span></span> <span data-ttu-id="e1c01-107">システムは、次の手順を決定するのに役立つように、クリアされなかったアプリに関連するエラーメッセージを生成します。</span><span class="sxs-lookup"><span data-stu-id="e1c01-107">The system will generate relevant error messages for the apps that failed to clear to help you determine next steps.</span></span>

> [!NOTE]
> <span data-ttu-id="e1c01-108">Saas リソースはサブスクリプションではなくテナントに関連付けられているため、この記事は SaaS プランには適用されません。</span><span class="sxs-lookup"><span data-stu-id="e1c01-108">This article does not apply to SaaS offers because SaaS resources are attached to a tenant, not a subscription.</span></span> <span data-ttu-id="e1c01-109">SaaS リソースは課金アカウント間で転送されますが、これはリソースごとに、Azure サポートによってサポート要求として行われます。</span><span class="sxs-lookup"><span data-stu-id="e1c01-109">SaaS resources are transferable from one billing account to another, but this is done per resource and by Azure support as a support request.</span></span>

## <a name="criteria-for-transfer-approval-or-denial"></a><span data-ttu-id="e1c01-110">転送の承認または拒否の条件</span><span class="sxs-lookup"><span data-stu-id="e1c01-110">Criteria for transfer approval or denial</span></span>

<span data-ttu-id="e1c01-111">いずれかのサードパーティ製アプリが次のいずれかの条件を満たしている場合は、サブスクリプションを転送できません。</span><span class="sxs-lookup"><span data-stu-id="e1c01-111">You cannot transfer a subscription if any of its third-party apps meet any of the following criteria:</span></span>

- <span data-ttu-id="e1c01-112">ターゲットアカウントは商用で、アプリはパートナーによって販売されることがオプトアウトされます。</span><span class="sxs-lookup"><span data-stu-id="e1c01-112">The target account is commercial and the app is opt-out to be sold via partners.</span></span>
- <span data-ttu-id="e1c01-113">選択したパートナーのアプリがオプトインされていますが、対象のアカウントが許可リストに含まれていません。</span><span class="sxs-lookup"><span data-stu-id="e1c01-113">The app is opt-in for selected partners and the target account is not in the allow list.</span></span>
- <span data-ttu-id="e1c01-114">プランは、選択したサブスクリプションについて過去に提供されていたプレビュー版であったか、またはプライベートプランだったので、許可リストに登録されていません。</span><span class="sxs-lookup"><span data-stu-id="e1c01-114">The offer was a preview offer in the past for selected subscriptions or was a private offer and the subscription is no longer in the allow list.</span></span>
- <span data-ttu-id="e1c01-115">新しい請求先アカウントは、プランが販売されているリージョンとは異なるリージョンにあり、そのリージョンでプランを販売することはできません。</span><span class="sxs-lookup"><span data-stu-id="e1c01-115">The new billing account is in a region different from where the offer is sold AND the offer is not to be sold in that region.</span></span>

<span data-ttu-id="e1c01-116">ブロックされた転送は、サブスクリプションからリソースを削除するまで有効です。その後、転送を再試行することができます。</span><span class="sxs-lookup"><span data-stu-id="e1c01-116">A blocked transfer remains in effect until you remove the resource from the subscription, after which you can try the transfer again.</span></span>

## <a name="next-steps"></a><span data-ttu-id="e1c01-117">次の手順</span><span class="sxs-lookup"><span data-stu-id="e1c01-117">Next steps</span></span>

[<span data-ttu-id="e1c01-118">Microsoft AppSource と Azure Marketplace のサポートを受ける</span><span class="sxs-lookup"><span data-stu-id="e1c01-118">Get support for Microsoft AppSource and Azure Marketplace</span></span>](get-support.md)

