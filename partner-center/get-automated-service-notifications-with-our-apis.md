---
title: 自動化されたサービス通知に Api を使用する
ms.topic: article
ms.date: 05/18/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: パートナーは、Office 365 および Microsoft Azure パートナー向けの Api を使用して、リアルタイムのサービス正常性、メッセージセンターの通信、および計画されたメンテナンスイベントを利用できます。
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 28a858afc0f34ff51523da8af2365141191348dc
ms.sourcegitcommit: e0a1b4506840486f4bb82620051e0f6a5e81662a
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/18/2020
ms.locfileid: "84991251"
---
# <a name="use-apis-for-automated-service-notifications-for-azure-insights--office-365-service-communications"></a><span data-ttu-id="b1899-103">Azure Insights & Office 365 サービス通信用の自動化されたサービス通知に Api を使用する</span><span class="sxs-lookup"><span data-stu-id="b1899-103">Use APIs for automated service notifications for Azure Insights & Office 365 service communications</span></span>

<span data-ttu-id="b1899-104">**適用対象**</span><span class="sxs-lookup"><span data-stu-id="b1899-104">**Applies to**</span></span>

-  <span data-ttu-id="b1899-105">パートナー センター</span><span class="sxs-lookup"><span data-stu-id="b1899-105">Partner Center</span></span>

<span data-ttu-id="b1899-106">**適切なロール**</span><span class="sxs-lookup"><span data-stu-id="b1899-106">**Appropriate roles**</span></span>

- <span data-ttu-id="b1899-107">管理エージェント</span><span class="sxs-lookup"><span data-stu-id="b1899-107">Admin agent</span></span>
- <span data-ttu-id="b1899-108">グローバル</span><span class="sxs-lookup"><span data-stu-id="b1899-108">Global</span></span> 
- <span data-ttu-id="b1899-109">販売代理店</span><span class="sxs-lookup"><span data-stu-id="b1899-109">Sales agent</span></span>
- <span data-ttu-id="b1899-110">ヘルプデスク エージェント</span><span class="sxs-lookup"><span data-stu-id="b1899-110">Helpdesk agent</span></span>

<span data-ttu-id="b1899-111">Office 365 と Microsoft Azure は、リアルタイムのサービスの正常性、メッセージ センターの通信、計画されたメンテナンス イベントを取得するために使うことができる API を提供しています。</span><span class="sxs-lookup"><span data-stu-id="b1899-111">Office 365 and Microsoft Azure each provide an API that partners can use to retrieve real-time service health, message center communications, and planned maintenance events.</span></span> <span data-ttu-id="b1899-112">これらの API は一般に公開されていて、委任された管理者特権があるため、パートナーはそれらをお客様に代わって使うことができます。</span><span class="sxs-lookup"><span data-stu-id="b1899-112">These APIs are publicly available, and partners can use them on behalf of their customers because of their delegated admin privileges.</span></span>

<span data-ttu-id="b1899-113">これらの API は社内の開発者のみが使うことができます。</span><span class="sxs-lookup"><span data-stu-id="b1899-113">These APIs are available for your developers:</span></span>

[<span data-ttu-id="b1899-114">Office 365 サービス通信 API</span><span class="sxs-lookup"><span data-stu-id="b1899-114">Office 365 service communications API</span></span>](https://go.microsoft.com/fwlink/p/?LinkId=616899)

<span data-ttu-id="b1899-115">Azure Insights REST API: [コード](https://go.microsoft.com/fwlink/p/?LinkId=617299)と [API リファレンス](https://go.microsoft.com/fwlink/p/?LinkId=617300)</span><span class="sxs-lookup"><span data-stu-id="b1899-115">Azure Insights REST API: [code](https://go.microsoft.com/fwlink/p/?LinkId=617299) and [API reference](https://go.microsoft.com/fwlink/p/?LinkId=617300)</span></span>

 

 



