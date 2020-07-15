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
# <a name="roles-and-permissions-eligible-to-earn-partner-earned-credit"></a>パートナーの獲得クレジットを獲得できるロールとアクセス許可

次のロールは、パートナーがパートナーの獲得クレジットを利用できるかどうかを判断するアクセス許可レベルにマップされます。

>[!Important]
>これらのロールとアクセス許可は、ユーザーがパートナーセンターで作業するために必要な役割とアクセス許可とは異なります。

|**ロール**   |**説明**   |**PEC 対象**   |
|-----------------|:------------------|:--------------|
|所有者  |リソースへのアクセスを含め、すべてを管理します。|はい|
|共同作成者 |リソースへのアクセスを許可する以外はすべて管理します。|はい|
|閲覧者|すべてを表示できますが、変更を加えることはできません。|いいえ|
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