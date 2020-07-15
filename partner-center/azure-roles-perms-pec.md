---
title: ロール、パートナー獲得クレジットのアクセス許可
ms.topic: article
ms.date: 05/04/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: パートナーがパートナーの獲得クレジット (PEC) を獲得できるようにするためのロールとアクセス許可について説明します。 これらは、パートナーセンターで動作するロールとは異なります。
author: adamyeh
ms.author: adamyeh
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: fa6241755e228e36abdd15022c127d2b243b488f
ms.sourcegitcommit: 6d45415908711cd0e28aeb19756b036274dcd326
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/15/2020
ms.locfileid: "86390589"
---
# <a name="roles-and-permissions-eligible-to-earn-partner-earned-credit"></a><span data-ttu-id="ea303-104">パートナーの獲得クレジットを獲得できるロールとアクセス許可</span><span class="sxs-lookup"><span data-stu-id="ea303-104">Roles and permissions eligible to earn partner earned credit</span></span>

<span data-ttu-id="ea303-105">次のロールは、パートナーがパートナーの獲得クレジットを利用できるかどうかを判断するアクセス許可レベルにマップされます。</span><span class="sxs-lookup"><span data-stu-id="ea303-105">The following roles map to permissions levels that determine whether a partner is eligible for partner earned credits.</span></span>

>[!Important]
><span data-ttu-id="ea303-106">これらのロールとアクセス許可は、ユーザーがパートナーセンターで作業するために必要な役割とアクセス許可とは異なります。</span><span class="sxs-lookup"><span data-stu-id="ea303-106">These roles and permissions are not the same as the roles and permissions a user needs to work in Partner Center.</span></span>

|<span data-ttu-id="ea303-107">**ロール**</span><span class="sxs-lookup"><span data-stu-id="ea303-107">**Role**</span></span>   |<span data-ttu-id="ea303-108">**説明**</span><span class="sxs-lookup"><span data-stu-id="ea303-108">**Description**</span></span>   |<span data-ttu-id="ea303-109">**PEC 対象**</span><span class="sxs-lookup"><span data-stu-id="ea303-109">**PEC eligible**</span></span>   |
|-----------------|:------------------|:--------------|
|<span data-ttu-id="ea303-110">所有者</span><span class="sxs-lookup"><span data-stu-id="ea303-110">Owner</span></span>  |<span data-ttu-id="ea303-111">リソースへのアクセスを含め、すべてを管理します。</span><span class="sxs-lookup"><span data-stu-id="ea303-111">You manage everything, including access to resources.</span></span>|<span data-ttu-id="ea303-112">はい</span><span class="sxs-lookup"><span data-stu-id="ea303-112">Yes</span></span>|
|<span data-ttu-id="ea303-113">共同作成者</span><span class="sxs-lookup"><span data-stu-id="ea303-113">Contributor</span></span> |<span data-ttu-id="ea303-114">リソースへのアクセスを許可する以外はすべて管理します。</span><span class="sxs-lookup"><span data-stu-id="ea303-114">You manage everything except granting access to resources.</span></span>|<span data-ttu-id="ea303-115">はい</span><span class="sxs-lookup"><span data-stu-id="ea303-115">Yes</span></span>|
|<span data-ttu-id="ea303-116">閲覧者</span><span class="sxs-lookup"><span data-stu-id="ea303-116">Reader</span></span>|<span data-ttu-id="ea303-117">すべてを表示できますが、変更を加えることはできません。</span><span class="sxs-lookup"><span data-stu-id="ea303-117">You can view everything, but not make any changes</span></span>|<span data-ttu-id="ea303-118">いいえ</span><span class="sxs-lookup"><span data-stu-id="ea303-118">No</span></span>|
|<span data-ttu-id="ea303-119">ACRDelete</span><span class="sxs-lookup"><span data-stu-id="ea303-119">ACRDelete</span></span>|<span data-ttu-id="ea303-120">acr の削除</span><span class="sxs-lookup"><span data-stu-id="ea303-120">acr delete</span></span>|<span data-ttu-id="ea303-121">はい</span><span class="sxs-lookup"><span data-stu-id="ea303-121">Yes</span></span>|
|<span data-ttu-id="ea303-122">ACRImageSigner 方</span><span class="sxs-lookup"><span data-stu-id="ea303-122">ACRImageSigner</span></span>|<span data-ttu-id="ea303-123">ACR イメージ署名者</span><span class="sxs-lookup"><span data-stu-id="ea303-123">acr image signer</span></span>|<span data-ttu-id="ea303-124">はい</span><span class="sxs-lookup"><span data-stu-id="ea303-124">Yes</span></span>|
|<span data-ttu-id="ea303-125">ACRPull</span><span class="sxs-lookup"><span data-stu-id="ea303-125">ACRPull</span></span>|<span data-ttu-id="ea303-126">acr のプル</span><span class="sxs-lookup"><span data-stu-id="ea303-126">acr pull</span></span>|<span data-ttu-id="ea303-127">はい</span><span class="sxs-lookup"><span data-stu-id="ea303-127">Yes</span></span>|
|<span data-ttu-id="ea303-128">AcrPush</span><span class="sxs-lookup"><span data-stu-id="ea303-128">AcrPush</span></span>|<span data-ttu-id="ea303-129">acr のプッシュ</span><span class="sxs-lookup"><span data-stu-id="ea303-129">acr push</span></span>|<span data-ttu-id="ea303-130">はい</span><span class="sxs-lookup"><span data-stu-id="ea303-130">Yes</span></span>|
|<span data-ttu-id="ea303-131">AcrQuarantineReader</span><span class="sxs-lookup"><span data-stu-id="ea303-131">AcrQuarantineReader</span></span>|<span data-ttu-id="ea303-132">ACR 検査データ閲覧者</span><span class="sxs-lookup"><span data-stu-id="ea303-132">acr quarantine data reader</span></span>|<span data-ttu-id="ea303-133">いいえ</span><span class="sxs-lookup"><span data-stu-id="ea303-133">No</span></span>|
|<span data-ttu-id="ea303-134">AcrQuarantineWriter</span><span class="sxs-lookup"><span data-stu-id="ea303-134">AcrQuarantineWriter</span></span>| <span data-ttu-id="ea303-135">ACR 検査データ作成者</span><span class="sxs-lookup"><span data-stu-id="ea303-135">acr quarantine data writer</span></span>|<span data-ttu-id="ea303-136">はい</span><span class="sxs-lookup"><span data-stu-id="ea303-136">Yes</span></span>|
|<span data-ttu-id="ea303-137">API Management Service Contributor</span><span class="sxs-lookup"><span data-stu-id="ea303-137">API Management Service Contributor</span></span>|<span data-ttu-id="ea303-138">サービスと API を管理できます</span><span class="sxs-lookup"><span data-stu-id="ea303-138">Can manage service and the APIs</span></span>|<span data-ttu-id="ea303-139">はい</span><span class="sxs-lookup"><span data-stu-id="ea303-139">Yes</span></span>|
|<span data-ttu-id="ea303-140">API Management Service Operator Role</span><span class="sxs-lookup"><span data-stu-id="ea303-140">API Management Service Operator Role</span></span>|<span data-ttu-id="ea303-141">サービスを管理できますが、API は対象外です</span><span class="sxs-lookup"><span data-stu-id="ea303-141">Can manage service but not the APIs</span></span>|<span data-ttu-id="ea303-142">はい</span><span class="sxs-lookup"><span data-stu-id="ea303-142">Yes</span></span>|
|<span data-ttu-id="ea303-143">API Management Service Reader Role</span><span class="sxs-lookup"><span data-stu-id="ea303-143">API Management Service Reader Role</span></span>|<span data-ttu-id="ea303-144">サービスと API への読み取り専用アクセスです</span><span class="sxs-lookup"><span data-stu-id="ea303-144">Read-only access to service and APIs</span></span>|<span data-ttu-id="ea303-145">いいえ</span><span class="sxs-lookup"><span data-stu-id="ea303-145">No</span></span>|
|<span data-ttu-id="ea303-146">Application Insights Component Contributor</span><span class="sxs-lookup"><span data-stu-id="ea303-146">Application Insights Component Contributor</span></span>|<span data-ttu-id="ea303-147">Application Insights コンポーネントを管理します</span><span class="sxs-lookup"><span data-stu-id="ea303-147">Manages Application Insights components</span></span>|<span data-ttu-id="ea303-148">はい</span><span class="sxs-lookup"><span data-stu-id="ea303-148">Yes</span></span>|
|<span data-ttu-id="ea303-149">Application Insights Snapshot Debugger</span><span class="sxs-lookup"><span data-stu-id="ea303-149">Application Insights Snapshot Debugger</span></span>|<span data-ttu-id="ea303-150">Application Insights スナップショット デバッガーで収集されたデバック スナップショットの表示とダウンロードを実行できるアクセス許可をユーザーに与えます。</span><span class="sxs-lookup"><span data-stu-id="ea303-150">Gives user permission to view and download debug snapshots collected with the Application Insights Snapshot Debugger.</span></span> <span data-ttu-id="ea303-151">これらのアクセス許可は、所有者ロールまたは共同作成者ロールには含まれないことに注意してください。</span><span class="sxs-lookup"><span data-stu-id="ea303-151">Note that these permissions are not included in the Owner or Contributor roles.</span></span>|<span data-ttu-id="ea303-152">はい</span><span class="sxs-lookup"><span data-stu-id="ea303-152">Yes</span></span>|
|