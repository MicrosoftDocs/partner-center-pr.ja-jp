---
title: CSP によるソフトウェア サブスクリプションの販売 |パートナー センター
ms.topic: article
ms.date: 01/24/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: CSP プログラムのパートナーがパートナー センターを使用して、顧客に代わって Azure 予約インスタンスとサーバー サブスクリプションの購入、管理、販売、および取り消しを行う方法について説明します。
author: jasonwhowell
ms.author: jasonh
keywords: クラウド ソリューション プロバイダー, CSP, クラウド ベースのサービス, Azure, Azure RI, Windows Server, SQL Server, ソフトウェア サブスクリプション, ソフトウェアの取り消し
ms.localizationpriority: high
ms.custom: seodec18
ms.openlocfilehash: 7cce25d5f16f5bd0f55169cdc9d516a69717d31a
ms.sourcegitcommit: 449cb8c32880217ad7543712b02a84ae69869289
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/23/2020
ms.locfileid: "80389991"
---
# <a name="sell-software-subscriptions-through-csp"></a><span data-ttu-id="fc424-104">CSP によるソフトウェア サブスクリプションの販売</span><span class="sxs-lookup"><span data-stu-id="fc424-104">Sell software subscriptions through CSP</span></span>

<span data-ttu-id="fc424-105">**適用対象**</span><span class="sxs-lookup"><span data-stu-id="fc424-105">**Applies to**</span></span>

- <span data-ttu-id="fc424-106">クラウド ソリューション プロバイダー</span><span class="sxs-lookup"><span data-stu-id="fc424-106">Cloud Solution Providers</span></span>

<span data-ttu-id="fc424-107">**適切なロール**</span><span class="sxs-lookup"><span data-stu-id="fc424-107">**Appropriate roles**</span></span>

- <span data-ttu-id="fc424-108">管理エージェント</span><span class="sxs-lookup"><span data-stu-id="fc424-108">Admin agent</span></span>
- <span data-ttu-id="fc424-109">グローバル管理者</span><span class="sxs-lookup"><span data-stu-id="fc424-109">Global admin</span></span>

<span data-ttu-id="fc424-110">Azure 予約とサーバー サブスクリプション (Windows Server および SQL Server サブスクリプション) を使用すると、CSP プログラムのパートナーは、予測可能性と永続性がきわめて高いクラウド ワークロードをコスト効率に優れたソリューションでサポートしたいという顧客の強い要望に適切に応えることができます。</span><span class="sxs-lookup"><span data-stu-id="fc424-110">With Azure reservations and Server subscriptions (Windows Server and SQL Server subscriptions), partners in the CSP program can better address the fast-growing customer demand for more cost-effective solutions to support highly predictable and persistent cloud workloads.</span></span> 

<span data-ttu-id="fc424-111">Azure ハイブリッド特典を活用することで、パートナー センターや Azure Portal から、企業顧客に代わって Azure 予約とサーバー サブスクリプションを取得、プロビジョニング、および管理できるようになりました。</span><span class="sxs-lookup"><span data-stu-id="fc424-111">You can now acquire, provision, and manage Azure reservations and Server subscriptions on behalf of commercial customers through Partner Center and the Azure Portal by taking advantage of the Azure Hybrid Benefit.</span></span>

<span data-ttu-id="fc424-112">Azure ハイブリッド特典を利用すると、Windows Server ライセンスから得られる価値を拡大し、仮想マシンのコストを最大で 40% 節約できます。</span><span class="sxs-lookup"><span data-stu-id="fc424-112">The Azure Hybrid Benefit helps you get more value from your Windows Server licenses and save up to 40 percent on virtual machines.</span></span> <span data-ttu-id="fc424-113">この特典はソフトウェア アシュアランスに含まれており、Windows Server Datacenter および Standard エディションのライセンスで利用できます。</span><span class="sxs-lookup"><span data-stu-id="fc424-113">You can use the benefit with Windows Server Datacenter and Standard edition licenses covered with Software Assurance.</span></span> <span data-ttu-id="fc424-114">エディションによっては、ライセンスを変換または再利用して、低いベース コンピューティング レート (Linux 仮想マシン レーなどト) で Windows Server 仮想マシンを Azure で実行できます。</span><span class="sxs-lookup"><span data-stu-id="fc424-114">Depending on the edition, you can convert or re-use your licenses to run Windows Server virtual machines in Azure and pay a lower base compute rate (Linux virtual machine rates, e.g.).</span></span>

## <a name="azure-reservations-unavailable-markets"></a><span data-ttu-id="fc424-115">Azure Reservations を利用できない市場</span><span class="sxs-lookup"><span data-stu-id="fc424-115">Azure reservations unavailable markets</span></span>

>[!IMPORTANT] 
><span data-ttu-id="fc424-116">次の市場では Azure Reservations を "*利用できません*"。</span><span class="sxs-lookup"><span data-stu-id="fc424-116">Azure reservations *are not* available in the following markets:</span></span>  
>  
> | <span data-ttu-id="fc424-117">利用できない市場</span><span class="sxs-lookup"><span data-stu-id="fc424-117">Unavailable markets</span></span> | &nbsp; | &nbsp; |
> |--------------------------------|-----------------------------------|------------------------------------------|
> | <span data-ttu-id="fc424-118">オーランド諸島</span><span class="sxs-lookup"><span data-stu-id="fc424-118">Åland Islands</span></span>     | <span data-ttu-id="fc424-119">グリーンランド</span><span class="sxs-lookup"><span data-stu-id="fc424-119">Greenland</span></span>     | <span data-ttu-id="fc424-120">パプアニューギニア</span><span class="sxs-lookup"><span data-stu-id="fc424-120">Papua New Guinea</span></span>     |
> | <span data-ttu-id="fc424-121">米領サモア</span><span class="sxs-lookup"><span data-stu-id="fc424-121">American Samoa</span></span>     | <span data-ttu-id="fc424-122">グレナダ</span><span class="sxs-lookup"><span data-stu-id="fc424-122">Grenada</span></span>     | <span data-ttu-id="fc424-123">ピトケアン島</span><span class="sxs-lookup"><span data-stu-id="fc424-123">Pitcairn Islands</span></span>     |
> | <span data-ttu-id="fc424-124">アンドラ</span><span class="sxs-lookup"><span data-stu-id="fc424-124">Andorra</span></span>     | <span data-ttu-id="fc424-125">グアドループ</span><span class="sxs-lookup"><span data-stu-id="fc424-125">Guadeloupe</span></span>     | <span data-ttu-id="fc424-126">レユニオン</span><span class="sxs-lookup"><span data-stu-id="fc424-126">Reunion</span></span>     |
> | <span data-ttu-id="fc424-127">アンギラ</span><span class="sxs-lookup"><span data-stu-id="fc424-127">Anguilla</span></span>     | <span data-ttu-id="fc424-128">グアム</span><span class="sxs-lookup"><span data-stu-id="fc424-128">Guam</span></span>     | <span data-ttu-id="fc424-129">サバ島</span><span class="sxs-lookup"><span data-stu-id="fc424-129">Saba</span></span>   |
> | <span data-ttu-id="fc424-130">南極</span><span class="sxs-lookup"><span data-stu-id="fc424-130">Antarctica</span></span>     | <span data-ttu-id="fc424-131">ガーンジー島</span><span class="sxs-lookup"><span data-stu-id="fc424-131">Guernsey</span></span>     | <span data-ttu-id="fc424-132">サン・バルテルミー</span><span class="sxs-lookup"><span data-stu-id="fc424-132">Saint Barthélemy</span></span>   |
> | <span data-ttu-id="fc424-133">アンティグア・バーブーダ</span><span class="sxs-lookup"><span data-stu-id="fc424-133">Antigua and Barbuda</span></span>       | <span data-ttu-id="fc424-134">ギニア</span><span class="sxs-lookup"><span data-stu-id="fc424-134">Guinea</span></span>     | <span data-ttu-id="fc424-135">セントルシア</span><span class="sxs-lookup"><span data-stu-id="fc424-135">Saint Lucia</span></span>   |
> | <span data-ttu-id="fc424-136">アルバ</span><span class="sxs-lookup"><span data-stu-id="fc424-136">Aruba</span></span>       | <span data-ttu-id="fc424-137">ギニアビサウ</span><span class="sxs-lookup"><span data-stu-id="fc424-137">Guinea-Bissau</span></span>     | <span data-ttu-id="fc424-138">サンマルタン島</span><span class="sxs-lookup"><span data-stu-id="fc424-138">Saint Martin</span></span>   |
> | <span data-ttu-id="fc424-139">アゼルバイジャン</span><span class="sxs-lookup"><span data-stu-id="fc424-139">Azerbaijan</span></span>       | <span data-ttu-id="fc424-140">ガイアナ</span><span class="sxs-lookup"><span data-stu-id="fc424-140">Guyana</span></span>     | <span data-ttu-id="fc424-141">サンピエール・ミクロン</span><span class="sxs-lookup"><span data-stu-id="fc424-141">Saint Pierre and Miquelon</span></span>   |
> | <span data-ttu-id="fc424-142">ベナン</span><span class="sxs-lookup"><span data-stu-id="fc424-142">Benin</span></span>     | <span data-ttu-id="fc424-143">ハイチ</span><span class="sxs-lookup"><span data-stu-id="fc424-143">Haiti</span></span>       | <span data-ttu-id="fc424-144">セントビンセントおよびグレナディーン諸島</span><span class="sxs-lookup"><span data-stu-id="fc424-144">Saint Vincent and the Grenadines</span></span>     |
> | <span data-ttu-id="fc424-145">ブータン</span><span class="sxs-lookup"><span data-stu-id="fc424-145">Bhutan</span></span>     | <span data-ttu-id="fc424-146">ハード・マクドナルド諸島</span><span class="sxs-lookup"><span data-stu-id="fc424-146">Heard Island and McDonald Islands</span></span>       | <span data-ttu-id="fc424-147">サモア</span><span class="sxs-lookup"><span data-stu-id="fc424-147">Samoa</span></span>     |
> | <span data-ttu-id="fc424-148">ボネール島</span><span class="sxs-lookup"><span data-stu-id="fc424-148">Bonaire</span></span>     | <span data-ttu-id="fc424-149">マン島</span><span class="sxs-lookup"><span data-stu-id="fc424-149">Isle of Man</span></span>     | <span data-ttu-id="fc424-150">サンマリノ</span><span class="sxs-lookup"><span data-stu-id="fc424-150">San Marino</span></span>     |
> | <span data-ttu-id="fc424-151">ブーベ島</span><span class="sxs-lookup"><span data-stu-id="fc424-151">Bouvet Island</span></span>     | <span data-ttu-id="fc424-152">ヤンマイエン島</span><span class="sxs-lookup"><span data-stu-id="fc424-152">Jan Mayen</span></span>     | <span data-ttu-id="fc424-153">サントメ・プリンシペ</span><span class="sxs-lookup"><span data-stu-id="fc424-153">São Tomé and Príncipe</span></span>   |
> | <span data-ttu-id="fc424-154">英領インド洋地域</span><span class="sxs-lookup"><span data-stu-id="fc424-154">British Indian Ocean Territory</span></span>       | <span data-ttu-id="fc424-155">ジャージー島</span><span class="sxs-lookup"><span data-stu-id="fc424-155">Jersey</span></span>     | <span data-ttu-id="fc424-156">セーシェル</span><span class="sxs-lookup"><span data-stu-id="fc424-156">Seychelles</span></span>   |
> | <span data-ttu-id="fc424-157">英領バージン諸島</span><span class="sxs-lookup"><span data-stu-id="fc424-157">British Virgin Islands</span></span>     | <span data-ttu-id="fc424-158">キリバス</span><span class="sxs-lookup"><span data-stu-id="fc424-158">Kiribati</span></span>       | <span data-ttu-id="fc424-159">シエラレオネ</span><span class="sxs-lookup"><span data-stu-id="fc424-159">Sierra Leone</span></span>   |
> | <span data-ttu-id="fc424-160">ブルキナファソ</span><span class="sxs-lookup"><span data-stu-id="fc424-160">Burkina Faso</span></span>     | <span data-ttu-id="fc424-161">コソボ</span><span class="sxs-lookup"><span data-stu-id="fc424-161">Kosovo</span></span>     | <span data-ttu-id="fc424-162">シント・ユースタティウス島</span><span class="sxs-lookup"><span data-stu-id="fc424-162">Sint Eustatius</span></span>     |
> | <span data-ttu-id="fc424-163">ブルンジ</span><span class="sxs-lookup"><span data-stu-id="fc424-163">Burundi</span></span>     | <span data-ttu-id="fc424-164">ラオス</span><span class="sxs-lookup"><span data-stu-id="fc424-164">Laos</span></span>     | <span data-ttu-id="fc424-165">シント・マールテン島</span><span class="sxs-lookup"><span data-stu-id="fc424-165">Sint Maarten</span></span>     |
> | <span data-ttu-id="fc424-166">カンボジア</span><span class="sxs-lookup"><span data-stu-id="fc424-166">Cambodia</span></span>     | <span data-ttu-id="fc424-167">レソト</span><span class="sxs-lookup"><span data-stu-id="fc424-167">Lesotho</span></span>     | <span data-ttu-id="fc424-168">ソロモン諸島</span><span class="sxs-lookup"><span data-stu-id="fc424-168">Solomon Islands</span></span>     |
> | <span data-ttu-id="fc424-169">中央アフリカ共和国</span><span class="sxs-lookup"><span data-stu-id="fc424-169">Central African Republic</span></span>     | <span data-ttu-id="fc424-170">リベリア</span><span class="sxs-lookup"><span data-stu-id="fc424-170">Liberia</span></span>     | <span data-ttu-id="fc424-171">ソマリア</span><span class="sxs-lookup"><span data-stu-id="fc424-171">Somalia</span></span>     |
> | <span data-ttu-id="fc424-172">チャド</span><span class="sxs-lookup"><span data-stu-id="fc424-172">Chad</span></span>     | <span data-ttu-id="fc424-173">マダガスカル</span><span class="sxs-lookup"><span data-stu-id="fc424-173">Madagascar</span></span>     | <span data-ttu-id="fc424-174">サウスジョージア・サウスサンドウィッチ諸島</span><span class="sxs-lookup"><span data-stu-id="fc424-174">South Georgia and South Sandwich Islands</span></span>     |
> | <span data-ttu-id="fc424-175">中国</span><span class="sxs-lookup"><span data-stu-id="fc424-175">China</span></span>     | <span data-ttu-id="fc424-176">マラウイ</span><span class="sxs-lookup"><span data-stu-id="fc424-176">Malawi</span></span>     | <span data-ttu-id="fc424-177">南スーダン</span><span class="sxs-lookup"><span data-stu-id="fc424-177">South Sudan</span></span>     |
> | <span data-ttu-id="fc424-178">クリスマス島</span><span class="sxs-lookup"><span data-stu-id="fc424-178">Christmas Island</span></span>     | <span data-ttu-id="fc424-179">モルディブ</span><span class="sxs-lookup"><span data-stu-id="fc424-179">Maldives</span></span>     | <span data-ttu-id="fc424-180">セントヘレナ、アセンションおよびトリスタンダクーニャ</span><span class="sxs-lookup"><span data-stu-id="fc424-180">St Helena, Ascension, Tristan da Cunha</span></span>     |
> | <span data-ttu-id="fc424-181">ココス諸島</span><span class="sxs-lookup"><span data-stu-id="fc424-181">Cocos (Keeling) Islands</span></span>     | <span data-ttu-id="fc424-182">マリ</span><span class="sxs-lookup"><span data-stu-id="fc424-182">Mali</span></span>     | <span data-ttu-id="fc424-183">スリナム</span><span class="sxs-lookup"><span data-stu-id="fc424-183">Suriname</span></span>     |
> | <span data-ttu-id="fc424-184">コモロ</span><span class="sxs-lookup"><span data-stu-id="fc424-184">Comoros</span></span>     | <span data-ttu-id="fc424-185">マーシャル諸島</span><span class="sxs-lookup"><span data-stu-id="fc424-185">Marshall Islands</span></span>     | <span data-ttu-id="fc424-186">スバールバル諸島</span><span class="sxs-lookup"><span data-stu-id="fc424-186">Svalbard</span></span>     |
> | <span data-ttu-id="fc424-187">コンゴ共和国</span><span class="sxs-lookup"><span data-stu-id="fc424-187">Congo</span></span>     | <span data-ttu-id="fc424-188">マルチニーク島</span><span class="sxs-lookup"><span data-stu-id="fc424-188">Martinique</span></span>     | <span data-ttu-id="fc424-189">スワジランド</span><span class="sxs-lookup"><span data-stu-id="fc424-189">Swaziland</span></span>     |
> | <span data-ttu-id="fc424-190">コンゴ民主共和国</span><span class="sxs-lookup"><span data-stu-id="fc424-190">Congo (DRC)</span></span>     | <span data-ttu-id="fc424-191">モーリタニア</span><span class="sxs-lookup"><span data-stu-id="fc424-191">Mauritania</span></span>     | <span data-ttu-id="fc424-192">ティモール・レステ</span><span class="sxs-lookup"><span data-stu-id="fc424-192">Timor-Leste</span></span>   |
> | <span data-ttu-id="fc424-193">クック諸島</span><span class="sxs-lookup"><span data-stu-id="fc424-193">Cook Islands</span></span>     | <span data-ttu-id="fc424-194">マイヨット島</span><span class="sxs-lookup"><span data-stu-id="fc424-194">Mayotte</span></span>     | <span data-ttu-id="fc424-195">トーゴ</span><span class="sxs-lookup"><span data-stu-id="fc424-195">Togo</span></span>   |
> | <span data-ttu-id="fc424-196">ジブチ</span><span class="sxs-lookup"><span data-stu-id="fc424-196">Djibouti</span></span>     | <span data-ttu-id="fc424-197">ミクロネシア</span><span class="sxs-lookup"><span data-stu-id="fc424-197">Micronesia</span></span>     | <span data-ttu-id="fc424-198">トケラウ諸島</span><span class="sxs-lookup"><span data-stu-id="fc424-198">Tokelau</span></span>   |
> | <span data-ttu-id="fc424-199">ドミニカ国</span><span class="sxs-lookup"><span data-stu-id="fc424-199">Dominica</span></span>     | <span data-ttu-id="fc424-200">モンセラット</span><span class="sxs-lookup"><span data-stu-id="fc424-200">Montserrat</span></span>     | <span data-ttu-id="fc424-201">トンガ</span><span class="sxs-lookup"><span data-stu-id="fc424-201">Tonga</span></span>   |
> | <span data-ttu-id="fc424-202">赤道ギニア</span><span class="sxs-lookup"><span data-stu-id="fc424-202">Equatorial Guinea</span></span>     | <span data-ttu-id="fc424-203">モザンビーク</span><span class="sxs-lookup"><span data-stu-id="fc424-203">Mozambique</span></span>     | <span data-ttu-id="fc424-204">タークス・カイコス諸島</span><span class="sxs-lookup"><span data-stu-id="fc424-204">Turks and Caicos Islands</span></span>   |
> | <span data-ttu-id="fc424-205">エリトリア</span><span class="sxs-lookup"><span data-stu-id="fc424-205">Eritrea</span></span>     | <span data-ttu-id="fc424-206">ミャンマー</span><span class="sxs-lookup"><span data-stu-id="fc424-206">Myanmar</span></span>     | <span data-ttu-id="fc424-207">ツバル</span><span class="sxs-lookup"><span data-stu-id="fc424-207">Tuvalu</span></span>   |
> | <span data-ttu-id="fc424-208">フォークランド諸島</span><span class="sxs-lookup"><span data-stu-id="fc424-208">Falkland Islands</span></span>     | <span data-ttu-id="fc424-209">ナウル</span><span class="sxs-lookup"><span data-stu-id="fc424-209">Nauru</span></span>     | <span data-ttu-id="fc424-210">米領小離島</span><span class="sxs-lookup"><span data-stu-id="fc424-210">U.S. Outlying Islands</span></span>   |
> | <span data-ttu-id="fc424-211">フランス領ギアナ</span><span class="sxs-lookup"><span data-stu-id="fc424-211">French Guiana</span></span>     | <span data-ttu-id="fc424-212">ニューカレドニア</span><span class="sxs-lookup"><span data-stu-id="fc424-212">New Caledonia</span></span>     | <span data-ttu-id="fc424-213">バヌアツ</span><span class="sxs-lookup"><span data-stu-id="fc424-213">Vanuatu</span></span>   |
> | <span data-ttu-id="fc424-214">フランス領ポリネシア</span><span class="sxs-lookup"><span data-stu-id="fc424-214">French Polynesia</span></span>     | <span data-ttu-id="fc424-215">ニジェール</span><span class="sxs-lookup"><span data-stu-id="fc424-215">Niger</span></span>     | <span data-ttu-id="fc424-216">バチカン市国</span><span class="sxs-lookup"><span data-stu-id="fc424-216">Vatican City</span></span>   |
> | <span data-ttu-id="fc424-217">仏領極南諸島</span><span class="sxs-lookup"><span data-stu-id="fc424-217">French Southern Territories</span></span>     | <span data-ttu-id="fc424-218">ニウエ</span><span class="sxs-lookup"><span data-stu-id="fc424-218">Niue</span></span>     | <span data-ttu-id="fc424-219">ワリス・フテュナ諸島</span><span class="sxs-lookup"><span data-stu-id="fc424-219">Wallis and Futuna</span></span>   |
> | <span data-ttu-id="fc424-220">ガボン</span><span class="sxs-lookup"><span data-stu-id="fc424-220">Gabon</span></span>     | <span data-ttu-id="fc424-221">ノーフォーク島</span><span class="sxs-lookup"><span data-stu-id="fc424-221">Norfolk Island</span></span>     | <span data-ttu-id="fc424-222">イエメン</span><span class="sxs-lookup"><span data-stu-id="fc424-222">Yemen</span></span>   |
> | <span data-ttu-id="fc424-223">ガンビア</span><span class="sxs-lookup"><span data-stu-id="fc424-223">Gambia</span></span>     | <span data-ttu-id="fc424-224">北マリアナ諸島</span><span class="sxs-lookup"><span data-stu-id="fc424-224">Northern Mariana Islands</span></span>     |    |
> | <span data-ttu-id="fc424-225">ジブラルタル</span><span class="sxs-lookup"><span data-stu-id="fc424-225">Gibraltar</span></span>     | <span data-ttu-id="fc424-226">パラオ</span><span class="sxs-lookup"><span data-stu-id="fc424-226">Palau</span></span>       |    |
<!--Nov 30, 2019 - this list of countries was correct as of today.
-->

## <a name="buy-software-subscriptions-on-behalf-of-customers"></a><span data-ttu-id="fc424-227">顧客に代わってソフトウェア サブスクリプションを購入する</span><span class="sxs-lookup"><span data-stu-id="fc424-227">Buy software subscriptions on behalf of customers</span></span>

<span data-ttu-id="fc424-228">顧客に代わってソフトウェア サブスクリプションを購入するには、次の操作を行います。</span><span class="sxs-lookup"><span data-stu-id="fc424-228">To buy software subscriptions on behalf of a customer:</span></span>

1. <span data-ttu-id="fc424-229">パートナー センター [ダッシュボード](https://partner.microsoft.com/dashboard)にサインインします。</span><span class="sxs-lookup"><span data-stu-id="fc424-229">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="fc424-230">パートナー センター メニューから **[顧客]** を選択し、一覧から顧客を選びます。</span><span class="sxs-lookup"><span data-stu-id="fc424-230">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

3. <span data-ttu-id="fc424-231">顧客の詳細ページから、 **[製品の追加]** を選択した後、画面の指示に従って注文を作成して支払います。</span><span class="sxs-lookup"><span data-stu-id="fc424-231">From the customer's detail page, select **Add products**, and then follow the on-screen instructions to create and pay for your order.</span></span> <span data-ttu-id="fc424-232">オーストラリアとブラジルを除き、すべての商用顧客向け価格には税は含まれません。</span><span class="sxs-lookup"><span data-stu-id="fc424-232">All commercial pricing excludes tax with the exception of Australia and Brazil.</span></span> <span data-ttu-id="fc424-233">オーストラリアとブラジルの場合は、価格に税が含まれています。</span><span class="sxs-lookup"><span data-stu-id="fc424-233">For Australia and Brazil, the price includes tax.</span></span>

## <a name="activate-and-manage-software-subscriptions"></a><span data-ttu-id="fc424-234">ソフトウェア サブスクリプションのライセンス認証と管理</span><span class="sxs-lookup"><span data-stu-id="fc424-234">Activate and manage software subscriptions</span></span>

<span data-ttu-id="fc424-235">ソフトウェア サブスクリプションを購入した後は、次の手順に従ってダウンロードします。</span><span class="sxs-lookup"><span data-stu-id="fc424-235">After you purchase the software subscription, follow the steps below to download it.</span></span>

>[!NOTE]
><span data-ttu-id="fc424-236">ソフトウェアをダウンロードしてライセンス認証キーを取得するには、管理エージェントである必要があります。</span><span class="sxs-lookup"><span data-stu-id="fc424-236">You must be an Admin agent to download software and get activation keys.</span></span>

1. <span data-ttu-id="fc424-237">パートナー センター [ダッシュボード](https://partner.microsoft.com/dashboard)にサインインします。</span><span class="sxs-lookup"><span data-stu-id="fc424-237">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="fc424-238">パートナー センター メニューから **[顧客]** を選択し、一覧から顧客を選びます。</span><span class="sxs-lookup"><span data-stu-id="fc424-238">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

3. <span data-ttu-id="fc424-239">顧客の詳細ページに移動し、 **[ソフトウェア]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="fc424-239">Go to your customer's detail page and then select **Software**.</span></span> <span data-ttu-id="fc424-240">顧客に代わって購入したすべてのソフトウェアの一覧が表示されます。</span><span class="sxs-lookup"><span data-stu-id="fc424-240">You'll see a list of all the software you've purchased on behalf of the customer.</span></span> 

4. <span data-ttu-id="fc424-241">ダウンロードする製品を展開します。</span><span class="sxs-lookup"><span data-stu-id="fc424-241">Expand the product you want to download.</span></span> <span data-ttu-id="fc424-242">**[製品の選択]** フィールドで、目的の **[バージョン]** 、 **[言語]** 、 **[ファイルの種類/OS]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="fc424-242">In the **Select product** field, select the **Version**, **Language**, and **File type/OS** that you want.</span></span> 

5. <span data-ttu-id="fc424-243">**[送信]** 選択して特定の製品を表示します。</span><span class="sxs-lookup"><span data-stu-id="fc424-243">Select **Submit** to display the specific products.</span></span> 

6. <span data-ttu-id="fc424-244">**[キーとダウンロードの取得]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="fc424-244">Select **Get keys and downloads**.</span></span> 

7. <span data-ttu-id="fc424-245">**[ダウンロード]** を選択してダウンロードを開始するか、 **[リンクのコピー]** を選択してリンクをコピーし、顧客に送信します。</span><span class="sxs-lookup"><span data-stu-id="fc424-245">Select **Download** to begin downloading, or select **Copy link** to copy the link and send it to the customer.</span></span> 

>[!NOTE]
><span data-ttu-id="fc424-246">このリンクは、2 週間後または 50 回のダウンロードのどちらか早い方のタイミングで期限切れになります。</span><span class="sxs-lookup"><span data-stu-id="fc424-246">This link will expire after two weeks or 50 downloads, whichever comes first.</span></span> <span data-ttu-id="fc424-247">リンクが期限切れになった場合は、このページに戻り、 **[キーとダウンロードの取得]** をもう一度選択して、2 週間または 50 回のダウンロードを再び有効にします。</span><span class="sxs-lookup"><span data-stu-id="fc424-247">Once the link expires, return to this page and select **Get keys and downloads** again to enable another two weeks or 50 downloads.</span></span> <span data-ttu-id="fc424-248">この操作は、必要な回数だけ行うことができます。</span><span class="sxs-lookup"><span data-stu-id="fc424-248">You can do this as many times as you need to.</span></span> 

## <a name="view-activity-for-software-key-access-and-software-downloads"></a><span data-ttu-id="fc424-249">ソフトウェア キーへのアクセスとソフトウェアのダウンロードに関するアクティビティを表示する</span><span class="sxs-lookup"><span data-stu-id="fc424-249">View activity for software key access and software downloads</span></span>

<span data-ttu-id="fc424-250">監査またはコンプライアンスの目的で、サーバー サブスクリプションのソフトウェア キーにアクセスしたか、サーバー サブスクリプション ソフトウェアをダウンロードしたユーザーの一覧を確認することが必要な場合があります。</span><span class="sxs-lookup"><span data-stu-id="fc424-250">For auditing or compliance purposes, you may need to check a list of users who have either accessed Server subscription software keys or downloaded Server subscription software.</span></span> <span data-ttu-id="fc424-251">この情報にアクセスするには、以下の手順を実行します。</span><span class="sxs-lookup"><span data-stu-id="fc424-251">Use the procedure below to access this information.</span></span> 

>[!NOTE]
><span data-ttu-id="fc424-252">これらのアクティビティ ログを表示するには、グローバル管理者、アカウント管理者、紹介管理者、またはマーケティング コンテンツ管理者になる必要があります。</span><span class="sxs-lookup"><span data-stu-id="fc424-252">You must be a Global administrator, Account admin, Referral admin, or Marketing content admin to see these activity logs.</span></span> 

1. <span data-ttu-id="fc424-253">パートナー センター [ダッシュボード](https://partner.microsoft.com/dashboard)にサインインします。</span><span class="sxs-lookup"><span data-stu-id="fc424-253">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="fc424-254">右上隅にある歯車アイコンを選択します。</span><span class="sxs-lookup"><span data-stu-id="fc424-254">Select the gear icon from the upper right corner.</span></span>

3. <span data-ttu-id="fc424-255">メニューで、 **[アクティビティ ログ]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="fc424-255">In the menu, select **Activity log**.</span></span>

4. <span data-ttu-id="fc424-256">表示するアクティビティの日付範囲を入力します。</span><span class="sxs-lookup"><span data-stu-id="fc424-256">Enter the date range for the activity you want to see.</span></span> <span data-ttu-id="fc424-257">アクティビティ ログに、指定した期間にソフトウェア キーにアクセスしたか、ソフトウェアをダウンロードしたユーザーの一覧が表示されます。</span><span class="sxs-lookup"><span data-stu-id="fc424-257">The activity log will display a list of users who have either accessed software keys or downloaded software during the time you specified.</span></span> 

## <a name="cancel-a-purchase"></a><span data-ttu-id="fc424-258">購入を取り消す</span><span class="sxs-lookup"><span data-stu-id="fc424-258">Cancel a purchase</span></span>

<span data-ttu-id="fc424-259">購入日から 60 日以内であればソフトウェア購入を取り消すことができます。</span><span class="sxs-lookup"><span data-stu-id="fc424-259">You can cancel a software purchase within 60 days of the purchase date.</span></span> <span data-ttu-id="fc424-260">この最初の 60 日以内に取り消した場合は、中途解約料がかかりません。</span><span class="sxs-lookup"><span data-stu-id="fc424-260">If you cancel within this first 60-day period, you will not be charged an early termination fee.</span></span> <span data-ttu-id="fc424-261">60 日を過ぎると、購入の取り消しができなくなります</span><span class="sxs-lookup"><span data-stu-id="fc424-261">After 60 days, you can no longer cancel a purchase.</span></span> <span data-ttu-id="fc424-262">(この取り消し規則の主な制限については、「注意」をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="fc424-262">(See Note for key restrictions to this cancellation rule.</span></span> <span data-ttu-id="fc424-263">ソフトウェアの購入を取り消した後の処理については、これらの手順の後にある「重要」もご覧ください。)</span><span class="sxs-lookup"><span data-stu-id="fc424-263">To learn about what happens after you cancel a software purchase, see also Important note after these steps.)</span></span> 

>[!NOTE]
><span data-ttu-id="fc424-264">購入を取り消すための次の手順は、購入後の最初の 60 日以内など、特定の取り消し期間内に取り消しの対象となったソフトウェアにのみ適用されます。</span><span class="sxs-lookup"><span data-stu-id="fc424-264">The following steps to cancel a purchase apply only to software that qualifies for cancellation within a specific cancellation window, such as within the first 60 days after purchase.</span></span> <span data-ttu-id="fc424-265">また、これらの手順は、Azure の SUSE Linux または RedHat ソフトウェア プランには適用されません。</span><span class="sxs-lookup"><span data-stu-id="fc424-265">These steps also do not apply to a SUSE Linux or RedHat software plan in Azure.</span></span> <span data-ttu-id="fc424-266">現時点では、SUSE または RedHat ソフトウェア プランのキャンセルや交換はできません。</span><span class="sxs-lookup"><span data-stu-id="fc424-266">At this time, you cannot cancel or exchange a SUSE or RedHat software plan.</span></span> <span data-ttu-id="fc424-267">SUSE Linux または RedHat プランの使用方法について詳しくは、[こちらをご覧ください](https://docs.microsoft.com/azure/virtual-machines/linux/prepay-suse-software-charges)。</span><span class="sxs-lookup"><span data-stu-id="fc424-267">[Learn more](https://docs.microsoft.com/azure/virtual-machines/linux/prepay-suse-software-charges) about using SUSE Linux or RedHat plans.</span></span>

<span data-ttu-id="fc424-268">購入をキャンセルするには、次の手順に従います。</span><span class="sxs-lookup"><span data-stu-id="fc424-268">Follow the steps below to cancel a purchase:</span></span>

>[!NOTE]
><span data-ttu-id="fc424-269">購入を取り消すには、管理エージェントである必要があります。</span><span class="sxs-lookup"><span data-stu-id="fc424-269">You must be an Admin agent to cancel a purchase.</span></span> <span data-ttu-id="fc424-270">次の手順では、パートナー センター ダッシュボードで購入を取り消す方法について説明します。</span><span class="sxs-lookup"><span data-stu-id="fc424-270">The following steps describe how to cancel a purchase in the Partner Center dashboard.</span></span> <span data-ttu-id="fc424-271">この操作は、[パートナー センター API](https://docs.microsoft.com/partner-center/develop/cancel-software-purchases) を使用して行うこともできます。</span><span class="sxs-lookup"><span data-stu-id="fc424-271">You can also do this using the [Partner Center API](https://docs.microsoft.com/partner-center/develop/cancel-software-purchases).</span></span>

1. <span data-ttu-id="fc424-272">取り消しプロセスを開始する前に、次のものが揃っていることを確認してください。</span><span class="sxs-lookup"><span data-stu-id="fc424-272">Before you start the cancellation process, make sure you have the following:</span></span>

    - <span data-ttu-id="fc424-273">顧客の名前、テナント GUID、またはドメイン名</span><span class="sxs-lookup"><span data-stu-id="fc424-273">The customer's name, tenant GUID or domain name</span></span>

    - <span data-ttu-id="fc424-274">取り消す製品の名称</span><span class="sxs-lookup"><span data-stu-id="fc424-274">The name of the product you want to cancel</span></span>
    
    - <span data-ttu-id="fc424-275">注文 ID</span><span class="sxs-lookup"><span data-stu-id="fc424-275">The Order ID</span></span>

2. <span data-ttu-id="fc424-276">パートナー センター [ダッシュボード](https://partner.microsoft.com/dashboard)にサインインします。</span><span class="sxs-lookup"><span data-stu-id="fc424-276">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

3. <span data-ttu-id="fc424-277">パートナー センター メニューから **[顧客]** を選択し、一覧から顧客を選びます。</span><span class="sxs-lookup"><span data-stu-id="fc424-277">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

4. <span data-ttu-id="fc424-278">顧客の詳細ページで、 **[ソフトウェア]** を選択して、顧客に代わって購入したソフトウェアの一覧を表示します。</span><span class="sxs-lookup"><span data-stu-id="fc424-278">On the customer’s details page, select **Software** to see the list of software purchased for the customer.</span></span> 

5. <span data-ttu-id="fc424-279">取り消すソフトウェアの購入を見つけて、 **[キャンセル]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="fc424-279">Locate the software purchase you want to cancel, and then select **Cancel**.</span></span> <span data-ttu-id="fc424-280">ダイアログ ボックスが表示されます。</span><span class="sxs-lookup"><span data-stu-id="fc424-280">A dialog box will appear.</span></span>

6. <span data-ttu-id="fc424-281">注文番号のドロップダウン リストから、取り消し対象の正しい注文 ID 番号を選択します</span><span class="sxs-lookup"><span data-stu-id="fc424-281">From the Order number drop-down list, select the correct order ID number you want to cancel.</span></span> <span data-ttu-id="fc424-282">(注文または注文 ID 番号について詳しくは、顧客の**注文履歴**ページをご覧ください)。</span><span class="sxs-lookup"><span data-stu-id="fc424-282">(You can learn more information about an order or order ID number from the customer's **Order history** page.)</span></span>

7. <span data-ttu-id="fc424-283">取り消しに関する**重要な**メッセージに目を通したことを確認するためのチェックボックスをオンにします</span><span class="sxs-lookup"><span data-stu-id="fc424-283">Select the checkbox to acknowledge that you have read the **Important** message concerning cancellation.</span></span> <span data-ttu-id="fc424-284">(購入を取り消した後の処理については、以下の「**重要**」をご覧ください)。</span><span class="sxs-lookup"><span data-stu-id="fc424-284">(Refer to the **Important** note below to learn more about what happens after you cancel a purchase.)</span></span>

8. <span data-ttu-id="fc424-285">**[送信]** を選択して購入を取り消します。</span><span class="sxs-lookup"><span data-stu-id="fc424-285">Select **Submit** to cancel your purchase.</span></span> <span data-ttu-id="fc424-286">顧客の複数の注文を取り消す場合は、一意の注文 ID 番号ごとに手順 4 ～ 6 を繰り返す必要があります。</span><span class="sxs-lookup"><span data-stu-id="fc424-286">If you want to cancel multiple orders for a customer, you will need to perform Steps 4 through 6 again for each, unique order ID number.</span></span>

<span data-ttu-id="fc424-287">注文の取り消しを試みると、パートナー センターから他の情報が送られてくることもあります (注文番号のドロップダウン リストの下に表示されます)。</span><span class="sxs-lookup"><span data-stu-id="fc424-287">When you attempt to cancel an order, Partner Center may also give you other information (that appears below the Order number drop-down list).</span></span> <span data-ttu-id="fc424-288">この情報には次の項目が含まれていることがあります。</span><span class="sxs-lookup"><span data-stu-id="fc424-288">This information can include:</span></span>

- <span data-ttu-id="fc424-289">その注文の取り消しが可能な残り日数</span><span class="sxs-lookup"><span data-stu-id="fc424-289">How many days remain for you to cancel that particular order</span></span>

- <span data-ttu-id="fc424-290">取り消し期間を既に過ぎていて注文の取り消しができなくなっているかどうか</span><span class="sxs-lookup"><span data-stu-id="fc424-290">Whether you have already passed the cancellation window and can no longer cancel the order</span></span>

- <span data-ttu-id="fc424-291">Microsoft で取り消し要求に関する情報がさらに必要な場合、**カスタマー サポート要求** フォームへのリンクが表示されることがあります。</span><span class="sxs-lookup"><span data-stu-id="fc424-291">If we need more information about your cancellation request, you may be given a link to a **customer support request** form.</span></span>

>[!IMPORTANT]
><span data-ttu-id="fc424-292">注文の取り消しが終わると、取り消しを確認するメッセージが表示されます。</span><span class="sxs-lookup"><span data-stu-id="fc424-292">After you cancel an order, a message confirming your cancellation will appear.</span></span> <span data-ttu-id="fc424-293">ただし、取り消しがパートナー センター ダッシュボードに表示されるまで、最大 15 分の遅延が発生する場合があります。</span><span class="sxs-lookup"><span data-stu-id="fc424-293">There may be a delay of up to 15 minutes, however, before the cancellation appears on the Partner Center dashboard.</span></span> <span data-ttu-id="fc424-294">また、次の取り消し後の詳細情報にもご注意ください。</span><span class="sxs-lookup"><span data-stu-id="fc424-294">Also note the following, post-cancellation details.</span></span>

<span data-ttu-id="fc424-295">購入を取り消した後は、次のようになります。</span><span class="sxs-lookup"><span data-stu-id="fc424-295">After you cancel a purchase:</span></span>

- <span data-ttu-id="fc424-296">関連するソフトウェア キーとダウンロード リンクがすべて失効します。</span><span class="sxs-lookup"><span data-stu-id="fc424-296">All related software keys and download links will be revoked.</span></span> <span data-ttu-id="fc424-297">つまり、パートナーとパートナーの顧客はこの購入に関連するソフトウェア キーとダウンロード リンクを使用できなくなります。</span><span class="sxs-lookup"><span data-stu-id="fc424-297">This means neither you nor your customer can use the software keys and download links any longer related to this purchase.</span></span> <span data-ttu-id="fc424-298">パートナーとパートナーの顧客は、取り消されたすべてのソフトウェアの使用を中止しなければなりません。</span><span class="sxs-lookup"><span data-stu-id="fc424-298">You and your customer are responsible for discontinuing the use of all cancelled software.</span></span> <span data-ttu-id="fc424-299">さらに、取り消されたソフトウェアをアンインストールし、関連するソフトウェアのダウンロードやリンクもすべて削除しなければなりません。</span><span class="sxs-lookup"><span data-stu-id="fc424-299">You are also responsible for uninstalling the cancelled software and removing any, related software downloads and links.</span></span>

- <span data-ttu-id="fc424-300">取り消された項目は顧客のソフトウェアの詳細ページに引き続き表示されますが、アクティブ化キーは入手できなくなります。</span><span class="sxs-lookup"><span data-stu-id="fc424-300">The cancelled item will still appear on the customer's Software details page but the activation key will not be available.</span></span>

- <span data-ttu-id="fc424-301">次回の月次請求書には、取り消された注文の返金額が表示されます。</span><span class="sxs-lookup"><span data-stu-id="fc424-301">A credit for the cancelled order will appear on your next monthly invoice.</span></span> <span data-ttu-id="fc424-302">永続的ソフトウェアの場合は全額返金され、ソフトウェア サブスクリプションの場合は日割り計算で返金されます。</span><span class="sxs-lookup"><span data-stu-id="fc424-302">Perpetual software will receive a 100% credit and software subscriptions will receive a prorated credit.</span></span>

### <a name="submit-a-customer-support-request-to-cancel-a-purchase"></a><span data-ttu-id="fc424-303">購入を取り消すためのカスタマー サポート要求を送信する</span><span class="sxs-lookup"><span data-stu-id="fc424-303">Submit a customer support request to cancel a purchase</span></span>

<span data-ttu-id="fc424-304">パートナー センターからソフトウェアの購入の取り消しを試みたが、詳細な情報の提供と、カスタマー サポート要求フォームへの記入を指示された場合は、次の手順が役立つことがあります。</span><span class="sxs-lookup"><span data-stu-id="fc424-304">If you tried to cancel a software purchase via Partner Center but were told to provide more information and fill out a customer support request form, these steps may help you:</span></span>

1. <span data-ttu-id="fc424-305">購入の取り消しウィンドウから **[customer support request]** (カスタマー サポート要求) リンクを選択すると、[パートナー センターに関する問題を報告する] ページが開きます。</span><span class="sxs-lookup"><span data-stu-id="fc424-305">When you select the **customer support request** link from the Cancel purchase window, the Report a problem with Partner Center page will open.</span></span>

2. <span data-ttu-id="fc424-306">[詳細] の [問題の種類] の一覧で、 **[お客様に代わって CSP を購入/払い戻し]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="fc424-306">Under Details, in the Type of problem list, select **CSP Purchase/Refund on behalf of customers**.</span></span>

3. <span data-ttu-id="fc424-307">[影響] および [タイトル] フィールドに入力します。</span><span class="sxs-lookup"><span data-stu-id="fc424-307">Fill in the Impact and Title fields.</span></span>

4. <span data-ttu-id="fc424-308">[説明] フィールドに、次の情報を入力します。</span><span class="sxs-lookup"><span data-stu-id="fc424-308">In the Description field, provide the following:</span></span>

    - <span data-ttu-id="fc424-309">顧客のテナント GUID またはドメイン名</span><span class="sxs-lookup"><span data-stu-id="fc424-309">The customer tenant GUID or domain name</span></span>
    
    - <span data-ttu-id="fc424-310">注文 ID またはサブスクリプション ID</span><span class="sxs-lookup"><span data-stu-id="fc424-310">Order ID or Subscription ID</span></span>
    
    - <span data-ttu-id="fc424-311">払い戻し理由</span><span class="sxs-lookup"><span data-stu-id="fc424-311">Refund reason</span></span>

    - <span data-ttu-id="fc424-312">要求された数量</span><span class="sxs-lookup"><span data-stu-id="fc424-312">Amount requested</span></span>

5. <span data-ttu-id="fc424-313">[連絡先] フィールドに、パートナーの名前、メール アドレス、電話番号を入力します。</span><span class="sxs-lookup"><span data-stu-id="fc424-313">In the Contact field, enter your name, email address, and phone number.</span></span>

6. <span data-ttu-id="fc424-314">何らかの理由でファイルを添付する必要がある場合は、 **[ファイルの追加]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="fc424-314">If you need to attach a file for any reason, select **Add files**.</span></span> <span data-ttu-id="fc424-315">この手順は省略可能です。</span><span class="sxs-lookup"><span data-stu-id="fc424-315">This step is optional.</span></span>

7. <span data-ttu-id="fc424-316">終了したら、 **[送信]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="fc424-316">When you're finished, select **Submit**.</span></span>
