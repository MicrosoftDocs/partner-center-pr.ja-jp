---
title: CSP によるソフトウェア サブスクリプションの販売 |パートナー センター
ms.topic: article
ms.date: 12/18/2019
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: CSP プログラムのパートナーがパートナーセンターを使用して、Azure 予約インスタンスと顧客のサーバーサブスクリプションを購入、管理、販売、キャンセルする方法について説明します。
author: MaggiePucciEvans
ms.author: evansma
keywords: クラウドソリューションプロバイダー、CSP、クラウドベースのサービス、Azure、Azure RI、Windows Server、SQL Server、ソフトウェアサブスクリプション、キャンセルソフトウェア
ms.localizationpriority: medium
ms.custom: seodec18
ms.openlocfilehash: 733c8ab6c2d15109011dfa240c2ce5954d748fea
ms.sourcegitcommit: 855b2aed1c395b199d8aaba88ac08cc277f474ea
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/19/2019
ms.locfileid: "75190243"
---
# <a name="sell-software-subscriptions-through-csp"></a><span data-ttu-id="1cd1e-104">CSP によるソフトウェア サブスクリプションの販売</span><span class="sxs-lookup"><span data-stu-id="1cd1e-104">Sell software subscriptions through CSP</span></span>

<span data-ttu-id="1cd1e-105">**適用対象**</span><span class="sxs-lookup"><span data-stu-id="1cd1e-105">**Applies to**</span></span>

- <span data-ttu-id="1cd1e-106">クラウド ソリューション プロバイダー</span><span class="sxs-lookup"><span data-stu-id="1cd1e-106">Cloud Solution Providers</span></span>

<span data-ttu-id="1cd1e-107">**適切なロール**</span><span class="sxs-lookup"><span data-stu-id="1cd1e-107">**Appropriate roles**</span></span>

- <span data-ttu-id="1cd1e-108">管理エージェント</span><span class="sxs-lookup"><span data-stu-id="1cd1e-108">Admin agent</span></span>
- <span data-ttu-id="1cd1e-109">グローバル管理</span><span class="sxs-lookup"><span data-stu-id="1cd1e-109">Global admin</span></span>

<span data-ttu-id="1cd1e-110">Azure の予約とサーバーサブスクリプション (Windows Server および SQL Server サブスクリプション) を使用すると、CSP プログラムのパートナーは、高度な予測可能性と持続性をサポートするためのコスト効率に優れたソリューションを実現するために、急速に成長する顧客の需要に対応することができます。クラウドワークロード。</span><span class="sxs-lookup"><span data-stu-id="1cd1e-110">With Azure reservations and Server subscriptions (Windows Server and SQL Server subscriptions), partners in the CSP program can better address the fast-growing customer demand for more cost-effective solutions to support highly predictable and persistent cloud workloads.</span></span> 

<span data-ttu-id="1cd1e-111">Azure ハイブリッド特典を利用して、パートナーセンターと Azure ポータルを使用して、商用顧客に代わって Azure 予約とサーバーサブスクリプションを取得、プロビジョニング、および管理できるようになりました。</span><span class="sxs-lookup"><span data-stu-id="1cd1e-111">You can now acquire, provision, and manage Azure reservations and Server subscriptions on behalf of commercial customers through Partner Center and the Azure Portal by taking advantage of the Azure Hybrid Benefit.</span></span>

<span data-ttu-id="1cd1e-112">Azure ハイブリッド特典を利用すると、Windows Server ライセンスから得られる価値を拡大し、仮想マシンのコストを最大で 40% 節約できます。</span><span class="sxs-lookup"><span data-stu-id="1cd1e-112">The Azure Hybrid Benefit helps you get more value from your Windows Server licenses and save up to 40 percent on virtual machines.</span></span> <span data-ttu-id="1cd1e-113">この特典はソフトウェア アシュアランスに含まれており、Windows Server Datacenter および Standard エディションのライセンスで利用できます。</span><span class="sxs-lookup"><span data-stu-id="1cd1e-113">You can use the benefit with Windows Server Datacenter and Standard edition licenses covered with Software Assurance.</span></span> <span data-ttu-id="1cd1e-114">エディションによっては、ライセンスを変換または再利用して、低いベース コンピューティング レート (Linux 仮想マシン レーなどト) で Windows Server 仮想マシンを Azure で実行できます。</span><span class="sxs-lookup"><span data-stu-id="1cd1e-114">Depending on the edition, you can convert or re-use your licenses to run Windows Server virtual machines in Azure and pay a lower base compute rate (Linux virtual machine rates, e.g.).</span></span>

## <a name="azure-reservations-unavailable-markets"></a><span data-ttu-id="1cd1e-115">Azure Reservations を利用できない市場</span><span class="sxs-lookup"><span data-stu-id="1cd1e-115">Azure reservations unavailable markets</span></span>

>[!IMPORTANT] 
><span data-ttu-id="1cd1e-116">次の市場では Azure Reservations を "*利用できません*"。</span><span class="sxs-lookup"><span data-stu-id="1cd1e-116">Azure reservations *are not* available in the following markets:</span></span>  
>  
> | <span data-ttu-id="1cd1e-117">利用できない市場</span><span class="sxs-lookup"><span data-stu-id="1cd1e-117">Unavailable markets</span></span> | &nbsp; | &nbsp; |
> |--------------------------------|-----------------------------------|------------------------------------------|
> | <span data-ttu-id="1cd1e-118">オーランド諸島</span><span class="sxs-lookup"><span data-stu-id="1cd1e-118">Åland Islands</span></span>     | <span data-ttu-id="1cd1e-119">グリーンランド</span><span class="sxs-lookup"><span data-stu-id="1cd1e-119">Greenland</span></span>     | <span data-ttu-id="1cd1e-120">パプアニューギニア</span><span class="sxs-lookup"><span data-stu-id="1cd1e-120">Papua New Guinea</span></span>     |
> | <span data-ttu-id="1cd1e-121">米領サモア</span><span class="sxs-lookup"><span data-stu-id="1cd1e-121">American Samoa</span></span>     | <span data-ttu-id="1cd1e-122">グレナダ</span><span class="sxs-lookup"><span data-stu-id="1cd1e-122">Grenada</span></span>     | <span data-ttu-id="1cd1e-123">ピトケアン島</span><span class="sxs-lookup"><span data-stu-id="1cd1e-123">Pitcairn Islands</span></span>     |
> | <span data-ttu-id="1cd1e-124">アンドラ</span><span class="sxs-lookup"><span data-stu-id="1cd1e-124">Andorra</span></span>     | <span data-ttu-id="1cd1e-125">グアドループ</span><span class="sxs-lookup"><span data-stu-id="1cd1e-125">Guadeloupe</span></span>     | <span data-ttu-id="1cd1e-126">レユニオン</span><span class="sxs-lookup"><span data-stu-id="1cd1e-126">Reunion</span></span>     |
> | <span data-ttu-id="1cd1e-127">アンギラ</span><span class="sxs-lookup"><span data-stu-id="1cd1e-127">Anguilla</span></span>     | <span data-ttu-id="1cd1e-128">グアム</span><span class="sxs-lookup"><span data-stu-id="1cd1e-128">Guam</span></span>     | <span data-ttu-id="1cd1e-129">サバ島</span><span class="sxs-lookup"><span data-stu-id="1cd1e-129">Saba</span></span>   |
> | <span data-ttu-id="1cd1e-130">南極</span><span class="sxs-lookup"><span data-stu-id="1cd1e-130">Antarctica</span></span>     | <span data-ttu-id="1cd1e-131">ガーンジー島</span><span class="sxs-lookup"><span data-stu-id="1cd1e-131">Guernsey</span></span>     | <span data-ttu-id="1cd1e-132">サン・バルテルミー</span><span class="sxs-lookup"><span data-stu-id="1cd1e-132">Saint Barthélemy</span></span>   |
> | <span data-ttu-id="1cd1e-133">アンティグア・バーブーダ</span><span class="sxs-lookup"><span data-stu-id="1cd1e-133">Antigua and Barbuda</span></span>       | <span data-ttu-id="1cd1e-134">ギニア</span><span class="sxs-lookup"><span data-stu-id="1cd1e-134">Guinea</span></span>     | <span data-ttu-id="1cd1e-135">セントルシア</span><span class="sxs-lookup"><span data-stu-id="1cd1e-135">Saint Lucia</span></span>   |
> | <span data-ttu-id="1cd1e-136">アルバ</span><span class="sxs-lookup"><span data-stu-id="1cd1e-136">Aruba</span></span>       | <span data-ttu-id="1cd1e-137">ギニアビサウ</span><span class="sxs-lookup"><span data-stu-id="1cd1e-137">Guinea-Bissau</span></span>     | <span data-ttu-id="1cd1e-138">サンマルタン島</span><span class="sxs-lookup"><span data-stu-id="1cd1e-138">Saint Martin</span></span>   |
> | <span data-ttu-id="1cd1e-139">アゼルバイジャン</span><span class="sxs-lookup"><span data-stu-id="1cd1e-139">Azerbaijan</span></span>       | <span data-ttu-id="1cd1e-140">ガイアナ</span><span class="sxs-lookup"><span data-stu-id="1cd1e-140">Guyana</span></span>     | <span data-ttu-id="1cd1e-141">サンピエール・ミクロン</span><span class="sxs-lookup"><span data-stu-id="1cd1e-141">Saint Pierre and Miquelon</span></span>   |
> | <span data-ttu-id="1cd1e-142">ベナン</span><span class="sxs-lookup"><span data-stu-id="1cd1e-142">Benin</span></span>     | <span data-ttu-id="1cd1e-143">ハイチ</span><span class="sxs-lookup"><span data-stu-id="1cd1e-143">Haiti</span></span>       | <span data-ttu-id="1cd1e-144">セントビンセントおよびグレナディーン諸島</span><span class="sxs-lookup"><span data-stu-id="1cd1e-144">Saint Vincent and the Grenadines</span></span>     |
> | <span data-ttu-id="1cd1e-145">ブータン</span><span class="sxs-lookup"><span data-stu-id="1cd1e-145">Bhutan</span></span>     | <span data-ttu-id="1cd1e-146">ハード・マクドナルド諸島</span><span class="sxs-lookup"><span data-stu-id="1cd1e-146">Heard Island and McDonald Islands</span></span>       | <span data-ttu-id="1cd1e-147">サモア</span><span class="sxs-lookup"><span data-stu-id="1cd1e-147">Samoa</span></span>     |
> | <span data-ttu-id="1cd1e-148">ボネール島</span><span class="sxs-lookup"><span data-stu-id="1cd1e-148">Bonaire</span></span>     | <span data-ttu-id="1cd1e-149">マン島</span><span class="sxs-lookup"><span data-stu-id="1cd1e-149">Isle of Man</span></span>     | <span data-ttu-id="1cd1e-150">サンマリノ</span><span class="sxs-lookup"><span data-stu-id="1cd1e-150">San Marino</span></span>     |
> | <span data-ttu-id="1cd1e-151">ブーベ島</span><span class="sxs-lookup"><span data-stu-id="1cd1e-151">Bouvet Island</span></span>     | <span data-ttu-id="1cd1e-152">ヤンマイエン島</span><span class="sxs-lookup"><span data-stu-id="1cd1e-152">Jan Mayen</span></span>     | <span data-ttu-id="1cd1e-153">サントメ・プリンシペ</span><span class="sxs-lookup"><span data-stu-id="1cd1e-153">São Tomé and Príncipe</span></span>   |
> | <span data-ttu-id="1cd1e-154">英領インド洋地域</span><span class="sxs-lookup"><span data-stu-id="1cd1e-154">British Indian Ocean Territory</span></span>       | <span data-ttu-id="1cd1e-155">ジャージー島</span><span class="sxs-lookup"><span data-stu-id="1cd1e-155">Jersey</span></span>     | <span data-ttu-id="1cd1e-156">セーシェル</span><span class="sxs-lookup"><span data-stu-id="1cd1e-156">Seychelles</span></span>   |
> | <span data-ttu-id="1cd1e-157">英領バージン諸島</span><span class="sxs-lookup"><span data-stu-id="1cd1e-157">British Virgin Islands</span></span>     | <span data-ttu-id="1cd1e-158">キリバス</span><span class="sxs-lookup"><span data-stu-id="1cd1e-158">Kiribati</span></span>       | <span data-ttu-id="1cd1e-159">シエラレオネ</span><span class="sxs-lookup"><span data-stu-id="1cd1e-159">Sierra Leone</span></span>   |
> | <span data-ttu-id="1cd1e-160">ブルキナファソ</span><span class="sxs-lookup"><span data-stu-id="1cd1e-160">Burkina Faso</span></span>     | <span data-ttu-id="1cd1e-161">コソボ</span><span class="sxs-lookup"><span data-stu-id="1cd1e-161">Kosovo</span></span>     | <span data-ttu-id="1cd1e-162">シント・ユースタティウス島</span><span class="sxs-lookup"><span data-stu-id="1cd1e-162">Sint Eustatius</span></span>     |
> | <span data-ttu-id="1cd1e-163">ブルンジ</span><span class="sxs-lookup"><span data-stu-id="1cd1e-163">Burundi</span></span>     | <span data-ttu-id="1cd1e-164">ラオス</span><span class="sxs-lookup"><span data-stu-id="1cd1e-164">Laos</span></span>     | <span data-ttu-id="1cd1e-165">シント・マールテン島</span><span class="sxs-lookup"><span data-stu-id="1cd1e-165">Sint Maarten</span></span>     |
> | <span data-ttu-id="1cd1e-166">カンボジア</span><span class="sxs-lookup"><span data-stu-id="1cd1e-166">Cambodia</span></span>     | <span data-ttu-id="1cd1e-167">レソト</span><span class="sxs-lookup"><span data-stu-id="1cd1e-167">Lesotho</span></span>     | <span data-ttu-id="1cd1e-168">ソロモン諸島</span><span class="sxs-lookup"><span data-stu-id="1cd1e-168">Solomon Islands</span></span>     |
> | <span data-ttu-id="1cd1e-169">中央アフリカ共和国</span><span class="sxs-lookup"><span data-stu-id="1cd1e-169">Central African Republic</span></span>     | <span data-ttu-id="1cd1e-170">リベリア</span><span class="sxs-lookup"><span data-stu-id="1cd1e-170">Liberia</span></span>     | <span data-ttu-id="1cd1e-171">ソマリア</span><span class="sxs-lookup"><span data-stu-id="1cd1e-171">Somalia</span></span>     |
> | <span data-ttu-id="1cd1e-172">チャド</span><span class="sxs-lookup"><span data-stu-id="1cd1e-172">Chad</span></span>     | <span data-ttu-id="1cd1e-173">マダガスカル</span><span class="sxs-lookup"><span data-stu-id="1cd1e-173">Madagascar</span></span>     | <span data-ttu-id="1cd1e-174">サウスジョージア・サウスサンドウィッチ諸島</span><span class="sxs-lookup"><span data-stu-id="1cd1e-174">South Georgia and South Sandwich Islands</span></span>     |
> | <span data-ttu-id="1cd1e-175">中国</span><span class="sxs-lookup"><span data-stu-id="1cd1e-175">China</span></span>     | <span data-ttu-id="1cd1e-176">マラウイ</span><span class="sxs-lookup"><span data-stu-id="1cd1e-176">Malawi</span></span>     | <span data-ttu-id="1cd1e-177">南スーダン</span><span class="sxs-lookup"><span data-stu-id="1cd1e-177">South Sudan</span></span>     |
> | <span data-ttu-id="1cd1e-178">クリスマス島</span><span class="sxs-lookup"><span data-stu-id="1cd1e-178">Christmas Island</span></span>     | <span data-ttu-id="1cd1e-179">モルディブ</span><span class="sxs-lookup"><span data-stu-id="1cd1e-179">Maldives</span></span>     | <span data-ttu-id="1cd1e-180">セントヘレナ、アセンションおよびトリスタンダクーニャ</span><span class="sxs-lookup"><span data-stu-id="1cd1e-180">St Helena, Ascension, Tristan da Cunha</span></span>     |
> | <span data-ttu-id="1cd1e-181">ココス諸島</span><span class="sxs-lookup"><span data-stu-id="1cd1e-181">Cocos (Keeling) Islands</span></span>     | <span data-ttu-id="1cd1e-182">マリ</span><span class="sxs-lookup"><span data-stu-id="1cd1e-182">Mali</span></span>     | <span data-ttu-id="1cd1e-183">スリナム</span><span class="sxs-lookup"><span data-stu-id="1cd1e-183">Suriname</span></span>     |
> | <span data-ttu-id="1cd1e-184">コモロ</span><span class="sxs-lookup"><span data-stu-id="1cd1e-184">Comoros</span></span>     | <span data-ttu-id="1cd1e-185">マーシャル諸島</span><span class="sxs-lookup"><span data-stu-id="1cd1e-185">Marshall Islands</span></span>     | <span data-ttu-id="1cd1e-186">スバールバル諸島</span><span class="sxs-lookup"><span data-stu-id="1cd1e-186">Svalbard</span></span>     |
> | <span data-ttu-id="1cd1e-187">コンゴ共和国</span><span class="sxs-lookup"><span data-stu-id="1cd1e-187">Congo</span></span>     | <span data-ttu-id="1cd1e-188">マルチニーク島</span><span class="sxs-lookup"><span data-stu-id="1cd1e-188">Martinique</span></span>     | <span data-ttu-id="1cd1e-189">スワジランド</span><span class="sxs-lookup"><span data-stu-id="1cd1e-189">Swaziland</span></span>     |
> | <span data-ttu-id="1cd1e-190">コンゴ民主共和国</span><span class="sxs-lookup"><span data-stu-id="1cd1e-190">Congo (DRC)</span></span>     | <span data-ttu-id="1cd1e-191">モーリタニア</span><span class="sxs-lookup"><span data-stu-id="1cd1e-191">Mauritania</span></span>     | <span data-ttu-id="1cd1e-192">ティモール・レステ</span><span class="sxs-lookup"><span data-stu-id="1cd1e-192">Timor-Leste</span></span>   |
> | <span data-ttu-id="1cd1e-193">クック諸島</span><span class="sxs-lookup"><span data-stu-id="1cd1e-193">Cook Islands</span></span>     | <span data-ttu-id="1cd1e-194">マイヨット島</span><span class="sxs-lookup"><span data-stu-id="1cd1e-194">Mayotte</span></span>     | <span data-ttu-id="1cd1e-195">トーゴ</span><span class="sxs-lookup"><span data-stu-id="1cd1e-195">Togo</span></span>   |
> | <span data-ttu-id="1cd1e-196">ジブチ</span><span class="sxs-lookup"><span data-stu-id="1cd1e-196">Djibouti</span></span>     | <span data-ttu-id="1cd1e-197">ミクロネシア</span><span class="sxs-lookup"><span data-stu-id="1cd1e-197">Micronesia</span></span>     | <span data-ttu-id="1cd1e-198">トケラウ諸島</span><span class="sxs-lookup"><span data-stu-id="1cd1e-198">Tokelau</span></span>   |
> | <span data-ttu-id="1cd1e-199">ドミニカ国</span><span class="sxs-lookup"><span data-stu-id="1cd1e-199">Dominica</span></span>     | <span data-ttu-id="1cd1e-200">モンセラット</span><span class="sxs-lookup"><span data-stu-id="1cd1e-200">Montserrat</span></span>     | <span data-ttu-id="1cd1e-201">トンガ</span><span class="sxs-lookup"><span data-stu-id="1cd1e-201">Tonga</span></span>   |
> | <span data-ttu-id="1cd1e-202">赤道ギニア</span><span class="sxs-lookup"><span data-stu-id="1cd1e-202">Equatorial Guinea</span></span>     | <span data-ttu-id="1cd1e-203">モザンビーク</span><span class="sxs-lookup"><span data-stu-id="1cd1e-203">Mozambique</span></span>     | <span data-ttu-id="1cd1e-204">タークス・カイコス諸島</span><span class="sxs-lookup"><span data-stu-id="1cd1e-204">Turks and Caicos Islands</span></span>   |
> | <span data-ttu-id="1cd1e-205">エリトリア</span><span class="sxs-lookup"><span data-stu-id="1cd1e-205">Eritrea</span></span>     | <span data-ttu-id="1cd1e-206">ミャンマー</span><span class="sxs-lookup"><span data-stu-id="1cd1e-206">Myanmar</span></span>     | <span data-ttu-id="1cd1e-207">ツバル</span><span class="sxs-lookup"><span data-stu-id="1cd1e-207">Tuvalu</span></span>   |
> | <span data-ttu-id="1cd1e-208">フォークランド諸島</span><span class="sxs-lookup"><span data-stu-id="1cd1e-208">Falkland Islands</span></span>     | <span data-ttu-id="1cd1e-209">ナウル</span><span class="sxs-lookup"><span data-stu-id="1cd1e-209">Nauru</span></span>     | <span data-ttu-id="1cd1e-210">合衆国領有小離島</span><span class="sxs-lookup"><span data-stu-id="1cd1e-210">U.S. Outlying Islands</span></span>   |
> | <span data-ttu-id="1cd1e-211">フランス領ギアナ</span><span class="sxs-lookup"><span data-stu-id="1cd1e-211">French Guiana</span></span>     | <span data-ttu-id="1cd1e-212">ニューカレドニア</span><span class="sxs-lookup"><span data-stu-id="1cd1e-212">New Caledonia</span></span>     | <span data-ttu-id="1cd1e-213">バヌアツ</span><span class="sxs-lookup"><span data-stu-id="1cd1e-213">Vanuatu</span></span>   |
> | <span data-ttu-id="1cd1e-214">フランス領ポリネシア</span><span class="sxs-lookup"><span data-stu-id="1cd1e-214">French Polynesia</span></span>     | <span data-ttu-id="1cd1e-215">ニジェール</span><span class="sxs-lookup"><span data-stu-id="1cd1e-215">Niger</span></span>     | <span data-ttu-id="1cd1e-216">バチカン市国</span><span class="sxs-lookup"><span data-stu-id="1cd1e-216">Vatican City</span></span>   |
> | <span data-ttu-id="1cd1e-217">仏領極南諸島</span><span class="sxs-lookup"><span data-stu-id="1cd1e-217">French Southern Territories</span></span>     | <span data-ttu-id="1cd1e-218">ニウエ</span><span class="sxs-lookup"><span data-stu-id="1cd1e-218">Niue</span></span>     | <span data-ttu-id="1cd1e-219">ワリス・フテュナ諸島</span><span class="sxs-lookup"><span data-stu-id="1cd1e-219">Wallis and Futuna</span></span>   |
> | <span data-ttu-id="1cd1e-220">ガボン</span><span class="sxs-lookup"><span data-stu-id="1cd1e-220">Gabon</span></span>     | <span data-ttu-id="1cd1e-221">ノーフォーク島</span><span class="sxs-lookup"><span data-stu-id="1cd1e-221">Norfolk Island</span></span>     | <span data-ttu-id="1cd1e-222">イエメン</span><span class="sxs-lookup"><span data-stu-id="1cd1e-222">Yemen</span></span>   |
> | <span data-ttu-id="1cd1e-223">ガンビア</span><span class="sxs-lookup"><span data-stu-id="1cd1e-223">Gambia</span></span>     | <span data-ttu-id="1cd1e-224">北マリアナ諸島</span><span class="sxs-lookup"><span data-stu-id="1cd1e-224">Northern Mariana Islands</span></span>     |    |
> | <span data-ttu-id="1cd1e-225">ジブラルタル</span><span class="sxs-lookup"><span data-stu-id="1cd1e-225">Gibraltar</span></span>     | <span data-ttu-id="1cd1e-226">パラオ</span><span class="sxs-lookup"><span data-stu-id="1cd1e-226">Palau</span></span>       |    |
<!--Nov 30, 2019 - this list of countries was correct as of today.
-->

## <a name="buy-software-subscriptions-on-behalf-of-customers"></a><span data-ttu-id="1cd1e-227">顧客に代わってソフトウェア サブスクリプションを購入する</span><span class="sxs-lookup"><span data-stu-id="1cd1e-227">Buy software subscriptions on behalf of customers</span></span>

<span data-ttu-id="1cd1e-228">顧客に代わってソフトウェアサブスクリプションを購入するには、次のようにします。</span><span class="sxs-lookup"><span data-stu-id="1cd1e-228">To buy software subscriptions on behalf of a customer:</span></span>

1. <span data-ttu-id="1cd1e-229">パートナーセンターの[ダッシュボード](https://partner.microsoft.com/dashboard)にサインインします。</span><span class="sxs-lookup"><span data-stu-id="1cd1e-229">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="1cd1e-230">パートナー センター メニューから **[顧客]** を選択し、一覧から顧客を選びます。</span><span class="sxs-lookup"><span data-stu-id="1cd1e-230">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

3. <span data-ttu-id="1cd1e-231">顧客の詳細ページで [製品の**追加**] を選択し、画面の指示に従って、注文の作成と支払いを行います。</span><span class="sxs-lookup"><span data-stu-id="1cd1e-231">From the customer's detail page, select **Add products**, and then follow the on-screen instructions to create and pay for your order.</span></span> <span data-ttu-id="1cd1e-232">オーストラリアとブラジルを除き、すべての商用顧客向け価格には税は含まれません。</span><span class="sxs-lookup"><span data-stu-id="1cd1e-232">All commercial pricing excludes tax with the exception of Australia and Brazil.</span></span> <span data-ttu-id="1cd1e-233">オーストラリアとブラジルの場合は、価格に税が含まれています。</span><span class="sxs-lookup"><span data-stu-id="1cd1e-233">For Australia and Brazil, the price includes tax.</span></span>

## <a name="activate-and-manage-software-subscriptions"></a><span data-ttu-id="1cd1e-234">ソフトウェア サブスクリプションのライセンス認証と管理</span><span class="sxs-lookup"><span data-stu-id="1cd1e-234">Activate and manage software subscriptions</span></span>

<span data-ttu-id="1cd1e-235">ソフトウェア サブスクリプションを購入した後は、次の手順に従ってダウンロードします。</span><span class="sxs-lookup"><span data-stu-id="1cd1e-235">After you purchase the software subscription, follow the steps below to download it.</span></span>

>[!NOTE]
><span data-ttu-id="1cd1e-236">ソフトウェアをダウンロードしてライセンス認証キーを取得するには、管理エージェントである必要があります。</span><span class="sxs-lookup"><span data-stu-id="1cd1e-236">You must be an Admin agent to download software and get activation keys.</span></span>

1. <span data-ttu-id="1cd1e-237">パートナーセンターの[ダッシュボード](https://partner.microsoft.com/dashboard)にサインインします。</span><span class="sxs-lookup"><span data-stu-id="1cd1e-237">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="1cd1e-238">パートナー センター メニューから **[顧客]** を選択し、一覧から顧客を選びます。</span><span class="sxs-lookup"><span data-stu-id="1cd1e-238">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

3. <span data-ttu-id="1cd1e-239">顧客の詳細ページに移動し、 **[ソフトウェア]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="1cd1e-239">Go to your customer's detail page and then select **Software**.</span></span> <span data-ttu-id="1cd1e-240">お客様の代わりに購入したすべてのソフトウェアの一覧が表示されます。</span><span class="sxs-lookup"><span data-stu-id="1cd1e-240">You'll see a list of all the software you've purchased on behalf of the customer.</span></span> 

4. <span data-ttu-id="1cd1e-241">ダウンロードする製品を展開します。</span><span class="sxs-lookup"><span data-stu-id="1cd1e-241">Expand the product you want to download.</span></span> <span data-ttu-id="1cd1e-242">**[製品の選択]** フィールドで、目的の **[バージョン]** 、 **[言語]** 、 **[ファイルの種類/OS]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="1cd1e-242">In the **Select product** field, select the **Version**, **Language**, and **File type/OS** that you want.</span></span> 

5. <span data-ttu-id="1cd1e-243">**[送信]** 選択して特定の製品を表示します。</span><span class="sxs-lookup"><span data-stu-id="1cd1e-243">Select **Submit** to display the specific products.</span></span> 

6. <span data-ttu-id="1cd1e-244">**[キーとダウンロードの取得]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="1cd1e-244">Select **Get keys and downloads**.</span></span> 

7. <span data-ttu-id="1cd1e-245">**[ダウンロード]** を選択してダウンロードを開始するか、 **[リンクのコピー]** を選択してリンクをコピーし、顧客に送信します。</span><span class="sxs-lookup"><span data-stu-id="1cd1e-245">Select **Download** to begin downloading, or select **Copy link** to copy the link and send it to the customer.</span></span> 

>[!NOTE]
><span data-ttu-id="1cd1e-246">このリンクは、2 週間後または 50 回のダウンロードのどちらか早い方のタイミングで期限切れになります。</span><span class="sxs-lookup"><span data-stu-id="1cd1e-246">This link will expire after two weeks or 50 downloads, whichever comes first.</span></span> <span data-ttu-id="1cd1e-247">リンクが期限切れになった場合は、このページに戻り、 **[キーとダウンロードの取得]** をもう一度選択して、2 週間または 50 回のダウンロードを再び有効にします。</span><span class="sxs-lookup"><span data-stu-id="1cd1e-247">Once the link expires, return to this page and select **Get keys and downloads** again to enable another two weeks or 50 downloads.</span></span> <span data-ttu-id="1cd1e-248">この操作は、必要な回数だけ行うことができます。</span><span class="sxs-lookup"><span data-stu-id="1cd1e-248">You can do this as many times as you need to.</span></span> 

## <a name="view-activity-for-software-key-access-and-software-downloads"></a><span data-ttu-id="1cd1e-249">ソフトウェアキーのアクセスおよびソフトウェアのダウンロードの利用状況を表示する</span><span class="sxs-lookup"><span data-stu-id="1cd1e-249">View activity for software key access and software downloads</span></span>

<span data-ttu-id="1cd1e-250">監査またはコンプライアンスの目的で、サーバーサブスクリプションのソフトウェアキーまたはダウンロードされたサーバーサブスクリプションソフトウェアにアクセスしたユーザーの一覧を確認する必要がある場合があります。</span><span class="sxs-lookup"><span data-stu-id="1cd1e-250">For auditing or compliance purposes, you may need to check a list of users who have either accessed Server subscription software keys or downloaded Server subscription software.</span></span> <span data-ttu-id="1cd1e-251">この情報にアクセスするには、以下の手順を使用します。</span><span class="sxs-lookup"><span data-stu-id="1cd1e-251">Use the procedure below to access this information.</span></span> 

>[!NOTE]
><span data-ttu-id="1cd1e-252">これらのアクティビティログを表示するには、グローバル管理者、アカウント管理者、参照管理者、またはマーケティングコンテンツ管理者である必要があります。</span><span class="sxs-lookup"><span data-stu-id="1cd1e-252">You must be a Global administrator, Account admin, Referral admin, or Marketing content admin to see these activity logs.</span></span> 

1. <span data-ttu-id="1cd1e-253">パートナーセンターの[ダッシュボード](https://partner.microsoft.com/dashboard)にサインインします。</span><span class="sxs-lookup"><span data-stu-id="1cd1e-253">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="1cd1e-254">右上隅の歯車アイコンを選択します。</span><span class="sxs-lookup"><span data-stu-id="1cd1e-254">Select the gear icon from the upper right corner.</span></span>

3. <span data-ttu-id="1cd1e-255">メニューで **[アクティビティログ]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="1cd1e-255">In the menu, select **Activity log**.</span></span>

4. <span data-ttu-id="1cd1e-256">表示する活動の日付範囲を入力します。</span><span class="sxs-lookup"><span data-stu-id="1cd1e-256">Enter the date range for the activity you want to see.</span></span> <span data-ttu-id="1cd1e-257">[アクティビティログ] には、指定した期間にソフトウェアキーまたはダウンロードしたソフトウェアにアクセスしたユーザーの一覧が表示されます。</span><span class="sxs-lookup"><span data-stu-id="1cd1e-257">The activity log will display a list of users who have either accessed software keys or downloaded software during the time you specified.</span></span> 

## <a name="cancel-a-purchase"></a><span data-ttu-id="1cd1e-258">購入を取り消す</span><span class="sxs-lookup"><span data-stu-id="1cd1e-258">Cancel a purchase</span></span>

<span data-ttu-id="1cd1e-259">購入日から 60 日以内であればソフトウェア購入を取り消すことができます。</span><span class="sxs-lookup"><span data-stu-id="1cd1e-259">You can cancel a software purchase within 60 days of the purchase date.</span></span> <span data-ttu-id="1cd1e-260">この最初の60日以内にキャンセルした場合、早期終了料金は課金されません。</span><span class="sxs-lookup"><span data-stu-id="1cd1e-260">If you cancel within this first 60-day period, you will not be charged an early termination fee.</span></span> <span data-ttu-id="1cd1e-261">60日後に、購入をキャンセルすることはできなくなります。</span><span class="sxs-lookup"><span data-stu-id="1cd1e-261">After 60 days, you can no longer cancel a purchase.</span></span> <span data-ttu-id="1cd1e-262">(このキャンセル規則の主な制限事項については、メモを参照してください。</span><span class="sxs-lookup"><span data-stu-id="1cd1e-262">(See Note for key restrictions to this cancellation rule.</span></span> <span data-ttu-id="1cd1e-263">ソフトウェアの購入をキャンセルした後の動作については、これらの手順の後にある重要な注意事項に関するページを参照してください。)</span><span class="sxs-lookup"><span data-stu-id="1cd1e-263">To learn about what happens after you cancel a software purchase, see also Important note after these steps.)</span></span> 

>[!NOTE]
><span data-ttu-id="1cd1e-264">購入をキャンセルする以下の手順は、購入後の最初の60日以内など、特定のキャンセル期間内にキャンセルが適用されるソフトウェアにのみ適用されます。</span><span class="sxs-lookup"><span data-stu-id="1cd1e-264">The following steps to cancel a purchase apply only to software that qualifies for cancellation within a specific cancellation window, such as within the first 60 days after purchase.</span></span> <span data-ttu-id="1cd1e-265">これらの購入をキャンセルする手順は、Microsoft Windows 7 の拡張セキュリティ更新プログラム2020の購入には適用されません。</span><span class="sxs-lookup"><span data-stu-id="1cd1e-265">Note that these steps to cancel a purchase do not apply to purchases of Microsoft Windows 7 Extended Security Updates 2020.</span></span> <span data-ttu-id="1cd1e-266">(Windows 7 ESU 2020 をキャンセルするには、このトピックの後半で説明するように、カスタマーサポート要求を送信する必要があります)。これらの手順は、Azure の SUSE Linux または RedHat ソフトウェアプランにも適用されません。</span><span class="sxs-lookup"><span data-stu-id="1cd1e-266">(To cancel Windows 7 ESU 2020, you need to submit a customer support request, as described later in this topic.) These steps also do not apply to a SUSE Linux or RedHat software plan in Azure.</span></span> <span data-ttu-id="1cd1e-267">現時点では、SUSE または RedHat ソフトウェアプランをキャンセルしたり交換したりすることはできません。</span><span class="sxs-lookup"><span data-stu-id="1cd1e-267">At this time, you cannot cancel or exchange a SUSE or RedHat software plan.</span></span> <span data-ttu-id="1cd1e-268">SUSE Linux または RedHat プランの使用方法については、[こちらを参照](https://docs.microsoft.com/azure/virtual-machines/linux/prepay-suse-software-charges)してください。</span><span class="sxs-lookup"><span data-stu-id="1cd1e-268">[Learn more](https://docs.microsoft.com/azure/virtual-machines/linux/prepay-suse-software-charges) about using SUSE Linux or RedHat plans.</span></span>

<span data-ttu-id="1cd1e-269">購入をキャンセルするには、次の手順に従います。</span><span class="sxs-lookup"><span data-stu-id="1cd1e-269">Follow the steps below to cancel a purchase:</span></span>

>[!NOTE]
><span data-ttu-id="1cd1e-270">購入を取り消すには、管理エージェントである必要があります。</span><span class="sxs-lookup"><span data-stu-id="1cd1e-270">You must be an Admin agent to cancel a purchase.</span></span> <span data-ttu-id="1cd1e-271">次の手順では、パートナーセンターのダッシュボードで購入をキャンセルする方法について説明します。</span><span class="sxs-lookup"><span data-stu-id="1cd1e-271">The following steps describe how to cancel a purchase in the Partner Center dashboard.</span></span> <span data-ttu-id="1cd1e-272">これは、[パートナーセンター API](https://docs.microsoft.com/partner-center/develop/cancel-software-purchases)を使用して行うこともできます。</span><span class="sxs-lookup"><span data-stu-id="1cd1e-272">You can also do this using the [Partner Center API](https://docs.microsoft.com/partner-center/develop/cancel-software-purchases).</span></span>

1. <span data-ttu-id="1cd1e-273">キャンセルプロセスを開始する前に、次のものがあることを確認してください。</span><span class="sxs-lookup"><span data-stu-id="1cd1e-273">Before you start the cancellation process, make sure you have the following:</span></span>

    - <span data-ttu-id="1cd1e-274">顧客の名前、テナントの GUID、またはドメイン名</span><span class="sxs-lookup"><span data-stu-id="1cd1e-274">The customer's name, tenant GUID or domain name</span></span>

    - <span data-ttu-id="1cd1e-275">取り消したい製品の名前</span><span class="sxs-lookup"><span data-stu-id="1cd1e-275">The name of the product you want to cancel</span></span>
    
    - <span data-ttu-id="1cd1e-276">注文 ID</span><span class="sxs-lookup"><span data-stu-id="1cd1e-276">The Order ID</span></span>

2. <span data-ttu-id="1cd1e-277">パートナーセンターの[ダッシュボード](https://partner.microsoft.com/dashboard)にサインインします。</span><span class="sxs-lookup"><span data-stu-id="1cd1e-277">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

3. <span data-ttu-id="1cd1e-278">パートナー センター メニューから **[顧客]** を選択し、一覧から顧客を選びます。</span><span class="sxs-lookup"><span data-stu-id="1cd1e-278">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

4. <span data-ttu-id="1cd1e-279">顧客の詳細ページで、 **[ソフトウェア]** を選択して、顧客用に購入したソフトウェアの一覧を表示します。</span><span class="sxs-lookup"><span data-stu-id="1cd1e-279">On the customer’s details page, select **Software** to see the list of software purchased for the customer.</span></span> 

5. <span data-ttu-id="1cd1e-280">取り消したいソフトウェア購入を見つけて、 **[キャンセル]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="1cd1e-280">Locate the software purchase you want to cancel, and then select **Cancel**.</span></span> <span data-ttu-id="1cd1e-281">ダイアログ ボックスが表示されます。</span><span class="sxs-lookup"><span data-stu-id="1cd1e-281">A dialog box will appear.</span></span>

6. <span data-ttu-id="1cd1e-282">注文番号 ドロップダウンリストから、キャンセルする正しい注文 ID 番号を選択し、**送信** を選択します。</span><span class="sxs-lookup"><span data-stu-id="1cd1e-282">From the Order number drop-down list, select the correct order ID number you want to cancel, then select **Submit**.</span></span>

7. <span data-ttu-id="1cd1e-283">顧客に対して複数の注文をキャンセルする場合は、一意の注文 ID 番号ごとに手順 4. ~ 6. をもう一度実行する必要があります。</span><span class="sxs-lookup"><span data-stu-id="1cd1e-283">If you want to cancel multiple orders for a customer, you will need to perform Steps 4 through 6 again for each, unique order ID number.</span></span> <span data-ttu-id="1cd1e-284">(注文または注文 ID 番号の詳細については、顧客の**注文履歴**ページを参照してください)。</span><span class="sxs-lookup"><span data-stu-id="1cd1e-284">(You can learn more information about an order or order ID number from the customer's **Order history** page.)</span></span>

8. <span data-ttu-id="1cd1e-285">注文を取り消すと、パートナーセンターから他の情報が表示される場合もあります (注文番号のドロップダウンリストに表示されます)。</span><span class="sxs-lookup"><span data-stu-id="1cd1e-285">When you attempt to cancel an order, Partner Center may also give you other information (that appears below the Order number drop-down list).</span></span> <span data-ttu-id="1cd1e-286">次の情報が含まれます。</span><span class="sxs-lookup"><span data-stu-id="1cd1e-286">This information can include:</span></span>

    - <span data-ttu-id="1cd1e-287">特定の注文を取り消すための残り日数</span><span class="sxs-lookup"><span data-stu-id="1cd1e-287">How many days remain for you to cancel that particular order</span></span>

    - <span data-ttu-id="1cd1e-288">キャンセルウィンドウが既に渡されていて、注文を取り消すことができないかどうか</span><span class="sxs-lookup"><span data-stu-id="1cd1e-288">Whether you have already passed the cancellation window and can no longer cancel the order</span></span>

    - <span data-ttu-id="1cd1e-289">取り消し要求に関する詳細情報が必要な場合は、**カスタマーサポート要求**フォームへのリンクが表示されることがあります。</span><span class="sxs-lookup"><span data-stu-id="1cd1e-289">If we need more information about your cancellation request, you may be given a link to a **customer support request** form.</span></span>

>[!IMPORTANT]
><span data-ttu-id="1cd1e-290">注文を取り消すと、取り消しを確認するメッセージが表示されます。</span><span class="sxs-lookup"><span data-stu-id="1cd1e-290">After you cancel an order, a message confirming your cancellation will appear.</span></span> <span data-ttu-id="1cd1e-291">ただし、キャンセルがパートナーセンターのダッシュボードに表示されるまでに、最大15分の遅延が発生する場合があります。</span><span class="sxs-lookup"><span data-stu-id="1cd1e-291">There may be a delay of up to 15 minutes, however, before the cancellation appears on the Partner Center dashboard.</span></span> <span data-ttu-id="1cd1e-292">さらに、次のキャンセル後の詳細にも注意してください。</span><span class="sxs-lookup"><span data-stu-id="1cd1e-292">Also note the following, post-cancellation details.</span></span>

<span data-ttu-id="1cd1e-293">購入を取り消した後:</span><span class="sxs-lookup"><span data-stu-id="1cd1e-293">After you cancel a purchase:</span></span>

- <span data-ttu-id="1cd1e-294">関連するすべてのソフトウェアキーとダウンロードリンクは失効します。</span><span class="sxs-lookup"><span data-stu-id="1cd1e-294">All related software keys and download links will be revoked.</span></span> <span data-ttu-id="1cd1e-295">つまり、お客様やお客様が本ソフトウェアキーを使用したり、この購入に関連するリンクをダウンロードしたりすることはできません。</span><span class="sxs-lookup"><span data-stu-id="1cd1e-295">This means neither you nor your customer can use the software keys and download links any longer related to this purchase.</span></span> <span data-ttu-id="1cd1e-296">お客様とお客様は、取り消されたすべてのソフトウェアの使用を中止する責任を負うものとします。</span><span class="sxs-lookup"><span data-stu-id="1cd1e-296">You and your customer are responsible for discontinuing the use of all cancelled software.</span></span> <span data-ttu-id="1cd1e-297">また、取り消されたソフトウェアをアンインストールし、関連するソフトウェアのダウンロードやリンクを削除する責任もあります。</span><span class="sxs-lookup"><span data-stu-id="1cd1e-297">You are also responsible for uninstalling the cancelled software and removing any, related software downloads and links.</span></span>

- <span data-ttu-id="1cd1e-298">取り消された項目は顧客のソフトウェア詳細ページに引き続き表示されますが、ライセンス認証キーは使用できません。</span><span class="sxs-lookup"><span data-stu-id="1cd1e-298">The cancelled item will still appear on the customer's Software details page but the activation key will not be available.</span></span>

- <span data-ttu-id="1cd1e-299">次の月次請求書には、取り消された注文のクレジットが表示されます。</span><span class="sxs-lookup"><span data-stu-id="1cd1e-299">A credit for the cancelled order will appear on your next monthly invoice.</span></span> <span data-ttu-id="1cd1e-300">永続的なソフトウェアには100% のクレジットが付与され、ソフトウェアのサブスクリプションは日割りで課金されます。</span><span class="sxs-lookup"><span data-stu-id="1cd1e-300">Perpetual software will receive a 100% credit and software subscriptions will receive a prorated credit.</span></span>

### <a name="submit-a-customer-support-request-to-cancel-a-purchase"></a><span data-ttu-id="1cd1e-301">カスタマーサポートリクエストを送信して購入をキャンセルする</span><span class="sxs-lookup"><span data-stu-id="1cd1e-301">Submit a customer support request to cancel a purchase</span></span>

<span data-ttu-id="1cd1e-302">パートナーセンターでソフトウェアの購入をキャンセルしようとしたが、詳細情報を提供し、カスタマーサポート要求フォームに記入するように指示された場合、これらの手順は次のような場合に役立ちます。</span><span class="sxs-lookup"><span data-stu-id="1cd1e-302">If you tried to cancel a software purchase via Partner Center but were told to provide more information and fill out a customer support request form, these steps may help you:</span></span>

1. <span data-ttu-id="1cd1e-303">購入の取り消し] ウィンドウから **[カスタマーサポート要求]** リンクを選択すると、[パートナーセンターで問題を報告する ページが開きます。</span><span class="sxs-lookup"><span data-stu-id="1cd1e-303">When you select the **customer support request** link from the Cancel purchase window, the Report a problem with Partner Center page will open.</span></span>

2. <span data-ttu-id="1cd1e-304">詳細 の 問題の種類 ボックスの一覧で、**ユーザーの代わりに CSP の購入/返金** を選択します。</span><span class="sxs-lookup"><span data-stu-id="1cd1e-304">Under Details, in the Type of problem list, select **CSP Purchase/Refund on behalf of customers**.</span></span>

3. <span data-ttu-id="1cd1e-305">[影響] フィールドと [タイトル] フィールドに入力します。</span><span class="sxs-lookup"><span data-stu-id="1cd1e-305">Fill in the Impact and Title fields.</span></span>

4. <span data-ttu-id="1cd1e-306">[説明] フィールドに、次の情報を入力します。</span><span class="sxs-lookup"><span data-stu-id="1cd1e-306">In the Description field, provide the following:</span></span>

    - <span data-ttu-id="1cd1e-307">顧客のテナント GUID またはドメイン名</span><span class="sxs-lookup"><span data-stu-id="1cd1e-307">The customer tenant GUID or domain name</span></span>
    
    - <span data-ttu-id="1cd1e-308">注文 ID またはサブスクリプション ID</span><span class="sxs-lookup"><span data-stu-id="1cd1e-308">Order ID or Subscription ID</span></span>
    
    - <span data-ttu-id="1cd1e-309">払い戻し理由</span><span class="sxs-lookup"><span data-stu-id="1cd1e-309">Refund reason</span></span>

    - <span data-ttu-id="1cd1e-310">要求された数量</span><span class="sxs-lookup"><span data-stu-id="1cd1e-310">Amount requested</span></span>

5. <span data-ttu-id="1cd1e-311">[Contact] \ (連絡先 \) フィールドに、名前、電子メールアドレス、および電話番号を入力します。</span><span class="sxs-lookup"><span data-stu-id="1cd1e-311">In the Contact field, enter your name, email address, and phone number.</span></span>

6. <span data-ttu-id="1cd1e-312">何らかの理由でファイルを添付する必要がある場合は、 **[ファイルの追加]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="1cd1e-312">If you need to attach a file for any reason, select **Add files**.</span></span> <span data-ttu-id="1cd1e-313">この手順は省略可能です。</span><span class="sxs-lookup"><span data-stu-id="1cd1e-313">This step is optional.</span></span>

7. <span data-ttu-id="1cd1e-314">終了したら、 **[送信]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="1cd1e-314">When you're finished, select **Submit**.</span></span>
