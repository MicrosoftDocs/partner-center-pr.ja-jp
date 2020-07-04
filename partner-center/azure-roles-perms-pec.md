---
title: ロール、パートナー獲得クレジットのアクセス許可
ms.topic: article
ms.date: 05/04/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: パートナーがパートナーの獲得クレジット (PEC) を獲得できるようにするためのロールとアクセス許可について説明します。 これらは、パートナーセンターで動作するロールとは異なります。
author: dineshvu
ms.author: dineshvu
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: c0f4e99dab2c898564941e926fc6d754547d66c1
ms.sourcegitcommit: 36a60f672c1c3d6b63fd225d04c5ffa917694ae0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/03/2020
ms.locfileid: "85948260"
---
# <a name="roles-and-permissions-eligible-to-earn-partner-earned-credit"></a>パートナーの獲得クレジットを獲得できるロールとアクセス許可

次のロールは、パートナーがパートナーの獲得クレジットを利用できるかどうかを判断するアクセス許可レベルにマップされます。

>[!Important]
>これらのロールとアクセス許可は、ユーザーがパートナーセンターで作業するために必要な役割とアクセス許可とは異なります。

|**ロール**   |**説明**   |**PEC 対象**   |
|-----------------|:------------------|:--------------|
|所有者  |リソースへのアクセスを含め、すべてを管理します。|Yes|
|共同作成者 |リソースへのアクセスを許可する以外はすべて管理します。|Yes|
|Reader|すべてを表示できますが、変更を加えることはできません。|No|
|ACRDelete|acr の削除|Yes|
|ACRImageSigner 方|ACR イメージ署名者|Yes|
|ACRPull|acr のプル|Yes|
|AcrPush|acr のプッシュ|Yes|
|AcrQuarantineReader|ACR 検査データ閲覧者|No|
|AcrQuarantineWriter| ACR 検査データ作成者|Yes|
|API Management Service Contributor|サービスと API を管理できます|Yes|
|API Management Service Operator Role|サービスを管理できますが、API は対象外です|Yes|
|API Management Service Reader Role|サービスと API への読み取り専用アクセスです|No|
|Application Insights Component Contributor|Application Insights コンポーネントを管理します|Yes|
|Application Insights Snapshot Debugger|Application Insights スナップショット デバッガーで収集されたデバック スナップショットの表示とダウンロードを実行できるアクセス許可をユーザーに与えます。 これらのアクセス許可は、所有者ロールまたは共同作成者ロールには含まれないことに注意してください。|はい|
|