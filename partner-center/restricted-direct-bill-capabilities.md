---
title: 限定された直接請求の機能 |パートナーセンター
ms.topic: article
ms.date: 01/24/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 新しい要件を満たしていないダイレクト請求パートナーは、直接請求の機能が制限されています
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
keywords: 直接請求、制限
ms.openlocfilehash: 7f2dae72edff59b3e6d84c74f93bae437be4ce30
ms.sourcegitcommit: d11c52e1386c181e177df72d6c7244508f1d6c0e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/29/2020
ms.locfileid: "76860503"
---
# <a name="restricted-direct-bill-capabilities"></a>制限付きの直接請求機能  

**概要**

直接請求先のパートナーは、新しい[要件](direct-partner-new-requirements.md)を満たしている必要があります。 そうしないと、直接請求の機能へのアクセスが最終的に制限され、顧客に対して新しい購入を行うなど、特定のタスクを実行できなくなります。 

>[!Note]
>CSP 直接請求パートナープログラムの新しい要件を満たしていない直接請求先のパートナーは、直接請求書の機能が制限されるときに Microsoft によって通知されます。 これは、直接請求[パートナーから間接リセラーへの移行](transition-direct-to-indirect.md)を選択したかどうかに関係なく、すべての直接請求パートナーに適用されます。  
 
## <a name="how-to-tell-if-your-direct-bill-capabilities-has-been-restricted"></a>直接請求の機能が制限されているかどうかを確認する方法 

直接請求パートナーテナントの直接請求機能へのアクセスが制限されているかどうかを確認するには、次のようにします。 

1. [パートナーセンターのダッシュボード](https://partner.microsoft.com/dashboard)にログインします。 

2. [**パートナーの設定** -> **パートナープロファイル**] にアクセスします。 

3. **[プログラム情報]** で、 **Microsoft Cloud ソリューションプロバイダーの状態**を探します。 

4. プログラムの状態に "値が**制限**されている" ということは、直接請求先のパートナーのテナントによる直接請求の機能へのアクセスが制限されていることを意味します。 
 
## <a name="affected-direct-bill-capabilities"></a>影響を受ける直接請求機能 

直接請求書の機能が制限されている場合は、パートナーセンターで顧客の新しい購入を行うことができなくなります。 たとえば、次のようなアニメーションや効果を作成できます。 

- Azure サブスクリプション 
- 座席ベースのサブスクリプション 
- 既存の座席ベースのサブスクリプションに新しいアドオンを追加します。 
- ソフトウェアと予約製品 (ソフトウェアサブスクリプション、永続ソフトウェア、Azure Reserved Virtual Machine instances など) を1回だけ購入する 

また、CSP プログラムの下にある[azure partner shared services プラン](shared-services.md)を使用して、新しい azure サブスクリプションを独自に購入することもできません。 

既存の直接請求サブスクリプションは影響を受けません。 それらは有効なまま残り、自動的に更新されます。 キャンセルされるまで、Microsoft による直接の課金が継続されます。 既存のサブスクリプションは、次の方法で引き続き管理できます。 

- 既存のサブスクリプションを中断します 
- 既存の接続クライアント数に基づくサブスクリプションの接続クライアント数の調整 
- サブスクリプションに対する既存のアドオンのシート数を調整します。 注: 新しいアドオンは新規購入として扱われるため、既存のサブスクリプションに追加することはできません。 
- 新しい Azure リソースのデプロイと、既存の Azure リソースの管理は、既存の Azure サブスクリプションの下で行います。 これには、Azure marketplace と Visual Studio サブスクリプションで利用可能なリソースが含まれます。 

新規購入だけでなく、パートナー センターで次の直接請求機能にアクセスすることもできません。 

- 新しい顧客テナントを作成することはできません。 パートナーセンターの **[顧客]** ページにある **[顧客の作成]** オプションは使用できません。 
- 直接再販業者の関係を要求している顧客への招待を生成することはできません。 パートナーセンターの **[顧客]** ページにある **[再販業者の関係を要求する]** オプションは使用できません。 

    >[!Note]
    >直接請求パートナーから間接リセラーへの移行の一環として、直接請求パートナーテナントを間接リセラーとして既に登録している場合は、代わりに間接再販業者の関係を要求する顧客への招待を生成できます。 
 
- 新しいサンドボックステナントを作成することはできません。 各直接請求パートナー テナントでは、直接請求 API の統合のために 1 つのサンドボックス テナントを作成できます。 以前に作成したことがない場合は、direct 請求パートナーの機能が制限された後に、この操作を行うことはできません。  

## <a name="see-also"></a>「 
- [間接リセラーになることについての追加情報](https://assetsprod.microsoft.com/csp-directbill-to-indirect-transition.pdf) 
- [CSP の直接パートナーの新しい要件](direct-partner-new-requirements.md)