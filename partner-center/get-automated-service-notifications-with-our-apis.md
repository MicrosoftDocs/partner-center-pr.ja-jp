---
title: 自動化されたサービス通知に API を使用する
ms.topic: article
ms.date: 05/18/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: パートナーは、Office 365 および Microsoft Azure パートナー向け API を使用して、リアルタイムのサービス正常性、メッセージ センターの通信、および計画メンテナンス イベントを実現できます。
author: Kim-Davis
ms.author: kimnich
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: b5092113ca90bccab6414fdf4013c76dd0ab4969
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/19/2021
ms.locfileid: "110150813"
---
# <a name="use-apis-for-automated-service-notifications-for-azure-insights--office-365-service-communications"></a><span data-ttu-id="b42e1-103">Office 365 サービス通信で Azure Insights の自動& API を使用する</span><span class="sxs-lookup"><span data-stu-id="b42e1-103">Use APIs for automated service notifications for Azure Insights & Office 365 service communications</span></span>

<span data-ttu-id="b42e1-104">**適切なロール**: 管理エージェント |グローバル管理者|Sales Agent |ヘルプデスク エージェント</span><span class="sxs-lookup"><span data-stu-id="b42e1-104">**Appropriate roles**: Admin agent | Global admin | Sales agent | Helpdesk agent</span></span>

<span data-ttu-id="b42e1-105">Office 365 と Microsoft Azure は、リアルタイムのサービスの正常性、メッセージ センターの通信、計画されたメンテナンス イベントを取得するために使うことができる API を提供しています。</span><span class="sxs-lookup"><span data-stu-id="b42e1-105">Office 365 and Microsoft Azure each provide an API that partners can use to retrieve real-time service health, message center communications, and planned maintenance events.</span></span> <span data-ttu-id="b42e1-106">これらの API は一般に公開されていて、委任された管理者特権があるため、パートナーはそれらをお客様に代わって使うことができます。</span><span class="sxs-lookup"><span data-stu-id="b42e1-106">These APIs are publicly available, and partners can use them on behalf of their customers because of their delegated admin privileges.</span></span>

<span data-ttu-id="b42e1-107">これらの API は社内の開発者のみが使うことができます。</span><span class="sxs-lookup"><span data-stu-id="b42e1-107">These APIs are available for your developers:</span></span>

- [<span data-ttu-id="b42e1-108">Office 365 サービス通信 API</span><span class="sxs-lookup"><span data-stu-id="b42e1-108">Office 365 service communications API</span></span>](/office/office-365-management-api/office-365-service-communications-api-reference)
- <span data-ttu-id="b42e1-109">Azure Insights REST [API リファレンス](/rest/api/monitor/)</span><span class="sxs-lookup"><span data-stu-id="b42e1-109">Azure Insights REST [API reference](/rest/api/monitor/)</span></span>
