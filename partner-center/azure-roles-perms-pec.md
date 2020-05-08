---
title: ロール、パートナー獲得クレジットのアクセス許可
ms.topic: article
ms.date: 05/04/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: パートナーがパートナーの獲得クレジット (PEC) を獲得できるようにするためのロールとアクセス許可について説明します。 これらは、パートナーセンターで動作するロールとは異なります。
ms.assetid: ''
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: af21fe17afdab07ef259634d9df18d65ae072d5d
ms.sourcegitcommit: e9b627159745bcce53a8c2b1676f63f5249bba76
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/07/2020
ms.locfileid: "82908275"
---
# <a name="roles-and-permissions-eligible-to-earn-partner-earned-credit"></a>パートナーの獲得クレジットを獲得できるロールとアクセス許可

次のロールは、パートナーがパートナーの獲得クレジットを利用できるかどうかを判断するアクセス許可レベルにマップされます。

>[!Important]
>これらのロールとアクセス許可は、ユーザーがパートナーセンターで作業するために必要な役割とアクセス許可とは異なります。

|**ロール**   |**説明**   |**PEC 対象**   |
|-----------------|:------------------|:--------------|
|所有者  |リソースへのアクセスを含め、すべてを管理します。|はい|
|Contributor |リソースへのアクセスを許可する以外はすべて管理します。|はい|
|Reader|すべてを表示できますが、変更を加えることはできません。|いいえ|
|ACRDelete|acr の削除|はい|
|ACRImageSigner 方|ACR イメージ署名者|はい|
|ACRPull|acr のプル|はい|
|AcrPush|acr のプッシュ|はい|
|AcrQuarantineReader|ACR 検査データ閲覧者|いいえ|
|AcrQuarantineWriter| ACR 検査データ作成者|はい|
|API Management Service Contributor|サービスと API を管理できます|はい|
|API Management Service Operator Role|サービスを管理できますが、API は対象外です|はい|
|API Management Service Reader Role|サービスと API への読み取り専用アクセスです|いいえ|
|Application Insights Component Contributor|Application Insights コンポーネントを管理します|はい|
|Application Insights Snapshot Debugger|Application Insights スナップショット デバッガーで収集されたデバック スナップショットの表示とダウンロードを実行できるアクセス許可をユーザーに与えます。 これらのアクセス許可は、所有者ロールまたは共同作成者ロールには含まれないことに注意してください。|はい|
|