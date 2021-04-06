---
title: 自動化されたサービス通知に Api を使用する
ms.topic: article
ms.date: 05/18/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: パートナーは、Office 365 および Microsoft Azure パートナー向けの Api を使用して、リアルタイムのサービス正常性、メッセージセンターの通信、および計画されたメンテナンスイベントを利用できます。
author: Kim-Davis
ms.author: kimnich
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: bdcc9feb9f6f022642ece217aa1ba17e24bd20da
ms.sourcegitcommit: 3c26a61982082787bbdaf5d1e92553b26f3a5076
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/06/2021
ms.locfileid: "106441440"
---
# <a name="use-apis-for-automated-service-notifications-for-azure-insights--office-365-service-communications"></a><span data-ttu-id="dd7e7-103">Azure Insights & Office 365 サービス通信用の自動化されたサービス通知に Api を使用する</span><span class="sxs-lookup"><span data-stu-id="dd7e7-103">Use APIs for automated service notifications for Azure Insights & Office 365 service communications</span></span>

<span data-ttu-id="dd7e7-104">**適切なロール**</span><span class="sxs-lookup"><span data-stu-id="dd7e7-104">**Appropriate roles**</span></span>

- <span data-ttu-id="dd7e7-105">管理エージェント</span><span class="sxs-lookup"><span data-stu-id="dd7e7-105">Admin agent</span></span>
- <span data-ttu-id="dd7e7-106">グローバル管理者</span><span class="sxs-lookup"><span data-stu-id="dd7e7-106">Global admin</span></span>
- <span data-ttu-id="dd7e7-107">販売代理店</span><span class="sxs-lookup"><span data-stu-id="dd7e7-107">Sales agent</span></span>
- <span data-ttu-id="dd7e7-108">ヘルプデスク エージェント</span><span class="sxs-lookup"><span data-stu-id="dd7e7-108">Helpdesk agent</span></span>

<span data-ttu-id="dd7e7-109">Office 365 と Microsoft Azure は、リアルタイムのサービスの正常性、メッセージ センターの通信、計画されたメンテナンス イベントを取得するために使うことができる API を提供しています。</span><span class="sxs-lookup"><span data-stu-id="dd7e7-109">Office 365 and Microsoft Azure each provide an API that partners can use to retrieve real-time service health, message center communications, and planned maintenance events.</span></span> <span data-ttu-id="dd7e7-110">これらの API は一般に公開されていて、委任された管理者特権があるため、パートナーはそれらをお客様に代わって使うことができます。</span><span class="sxs-lookup"><span data-stu-id="dd7e7-110">These APIs are publicly available, and partners can use them on behalf of their customers because of their delegated admin privileges.</span></span>

<span data-ttu-id="dd7e7-111">これらの API は社内の開発者のみが使うことができます。</span><span class="sxs-lookup"><span data-stu-id="dd7e7-111">These APIs are available for your developers:</span></span>

- [<span data-ttu-id="dd7e7-112">Office 365 サービス通信 API</span><span class="sxs-lookup"><span data-stu-id="dd7e7-112">Office 365 service communications API</span></span>](/office/office-365-management-api/office-365-service-communications-api-reference)
- <span data-ttu-id="dd7e7-113">Azure Insights REST [API リファレンス](/rest/api/monitor/)</span><span class="sxs-lookup"><span data-stu-id="dd7e7-113">Azure Insights REST [API reference](/rest/api/monitor/)</span></span>

 

 
