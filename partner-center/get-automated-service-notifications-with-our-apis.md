---
title: 自動化されたサービス通知に Api を使用する
ms.topic: article
ms.date: 05/18/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: パートナーは、Office 365 および Microsoft Azure パートナー向けの Api を使用して、リアルタイムのサービス正常性、メッセージセンターの通信、および計画されたメンテナンスイベントを利用できます。
author: brentserbus
ms.author: brserbus
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 12a7c37bca999d6f31286a121dd191625e5b7470
ms.sourcegitcommit: 13b0e1358dc306f896190088d31a0d883644850f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/10/2020
ms.locfileid: "86219590"
---
# <a name="use-apis-for-automated-service-notifications-for-azure-insights--office-365-service-communications"></a><span data-ttu-id="9857b-103">Azure Insights & Office 365 サービス通信用の自動化されたサービス通知に Api を使用する</span><span class="sxs-lookup"><span data-stu-id="9857b-103">Use APIs for automated service notifications for Azure Insights & Office 365 service communications</span></span>

<span data-ttu-id="9857b-104">**適用対象**</span><span class="sxs-lookup"><span data-stu-id="9857b-104">**Applies to**</span></span>

-  <span data-ttu-id="9857b-105">パートナー センター</span><span class="sxs-lookup"><span data-stu-id="9857b-105">Partner Center</span></span>

<span data-ttu-id="9857b-106">**適切なロール**</span><span class="sxs-lookup"><span data-stu-id="9857b-106">**Appropriate roles**</span></span>

- <span data-ttu-id="9857b-107">管理エージェント</span><span class="sxs-lookup"><span data-stu-id="9857b-107">Admin agent</span></span>
- <span data-ttu-id="9857b-108">グローバル</span><span class="sxs-lookup"><span data-stu-id="9857b-108">Global</span></span> 
- <span data-ttu-id="9857b-109">販売代理店</span><span class="sxs-lookup"><span data-stu-id="9857b-109">Sales agent</span></span>
- <span data-ttu-id="9857b-110">ヘルプデスク エージェント</span><span class="sxs-lookup"><span data-stu-id="9857b-110">Helpdesk agent</span></span>

<span data-ttu-id="9857b-111">Office 365 と Microsoft Azure は、リアルタイムのサービスの正常性、メッセージ センターの通信、計画されたメンテナンス イベントを取得するために使うことができる API を提供しています。</span><span class="sxs-lookup"><span data-stu-id="9857b-111">Office 365 and Microsoft Azure each provide an API that partners can use to retrieve real-time service health, message center communications, and planned maintenance events.</span></span> <span data-ttu-id="9857b-112">これらの API は一般に公開されていて、委任された管理者特権があるため、パートナーはそれらをお客様に代わって使うことができます。</span><span class="sxs-lookup"><span data-stu-id="9857b-112">These APIs are publicly available, and partners can use them on behalf of their customers because of their delegated admin privileges.</span></span>

<span data-ttu-id="9857b-113">これらの API は社内の開発者のみが使うことができます。</span><span class="sxs-lookup"><span data-stu-id="9857b-113">These APIs are available for your developers:</span></span>

[<span data-ttu-id="9857b-114">Office 365 サービス通信 API</span><span class="sxs-lookup"><span data-stu-id="9857b-114">Office 365 service communications API</span></span>](https://go.microsoft.com/fwlink/p/?LinkId=616899)

<span data-ttu-id="9857b-115">Azure Insights REST API: [コード](https://go.microsoft.com/fwlink/p/?LinkId=617299)と [API リファレンス](https://go.microsoft.com/fwlink/p/?LinkId=617300)</span><span class="sxs-lookup"><span data-stu-id="9857b-115">Azure Insights REST API: [code](https://go.microsoft.com/fwlink/p/?LinkId=617299) and [API reference](https://go.microsoft.com/fwlink/p/?LinkId=617300)</span></span>

 

 



