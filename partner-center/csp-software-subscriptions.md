---
title: CSP によるソフトウェア サブスクリプションの販売
ms.topic: how-to
ms.date: 01/29/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: CSP プログラムのパートナーがパートナー センターを使用して、顧客に代わって Azure 予約インスタンスとサーバー サブスクリプションの購入、管理、販売、および取り消しを行う方法について説明します。
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.openlocfilehash: 5355dd6229d22d154512be8536e5fd4ab9b900ad
ms.sourcegitcommit: 2d1f0d7bc897278ef37af6d43c1a088f5ca14807
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/08/2021
ms.locfileid: "99834858"
---
# <a name="sell-software-subscriptions-through-the-cloud-solution-provider-csp-program"></a><span data-ttu-id="b73c6-103">クラウド ソリューション プロバイダー (CSP) プログラムによりソフトウェア サブスクリプションを販売する</span><span class="sxs-lookup"><span data-stu-id="b73c6-103">Sell software subscriptions through the Cloud Solution Provider (CSP) program</span></span>

<span data-ttu-id="b73c6-104">**適用対象**</span><span class="sxs-lookup"><span data-stu-id="b73c6-104">**Applies to**</span></span>

- <span data-ttu-id="b73c6-105">クラウド ソリューション プロバイダー</span><span class="sxs-lookup"><span data-stu-id="b73c6-105">Cloud Solution Providers</span></span>

<span data-ttu-id="b73c6-106">**適切なロール**</span><span class="sxs-lookup"><span data-stu-id="b73c6-106">**Appropriate roles**</span></span>

- <span data-ttu-id="b73c6-107">管理エージェント</span><span class="sxs-lookup"><span data-stu-id="b73c6-107">Admin agent</span></span>
- <span data-ttu-id="b73c6-108">グローバル管理者</span><span class="sxs-lookup"><span data-stu-id="b73c6-108">Global admin</span></span>

<span data-ttu-id="b73c6-109">Azure 予約とサーバー サブスクリプション (Windows Server および SQL Server サブスクリプション) を使用すると、CSP プログラムのパートナーは、予測可能性と永続性の高いクラウド ワークロードを、よりコスト効率の優れたソリューションでサポートしたいという顧客の需要の急速な高まりに一層十分に応えられます。</span><span class="sxs-lookup"><span data-stu-id="b73c6-109">With Azure reservations and Server subscriptions (Windows Server and SQL Server subscriptions),partners in the CSP program can better address the fast-growing customer demand for more cost-effective solutions to support highly predictable and persistent cloud workloads.</span></span> 

<span data-ttu-id="b73c6-110">Azure ハイブリッド特典を活用することで、パートナー センターや Azure portal から、企業顧客に代わって Azure 予約とサーバー サブスクリプションを取得、プロビジョニング、および管理できるようになりました。</span><span class="sxs-lookup"><span data-stu-id="b73c6-110">You can now acquire, provision, and manage Azure reservations and Server subscriptions on behalf of commercial customers through Partner Center and the Azure portal by taking advantage of the Azure Hybrid Benefit.</span></span>

<span data-ttu-id="b73c6-111">Azure ハイブリッド特典を利用すると、Windows Server ライセンスから得られる価値を拡大し、仮想マシンのコストを最大で 40% 節約できます。</span><span class="sxs-lookup"><span data-stu-id="b73c6-111">The Azure Hybrid Benefit helps you get more value from your Windows Server licenses and save up to 40 percent on virtual machines.</span></span> <span data-ttu-id="b73c6-112">この特典はソフトウェア アシュアランスに含まれており、Windows Server Datacenter および Standard エディションのライセンスで利用できます。</span><span class="sxs-lookup"><span data-stu-id="b73c6-112">You can use the benefit with Windows Server Datacenter and Standard edition licenses covered with Software Assurance.</span></span> <span data-ttu-id="b73c6-113">エディションによっては、ライセンスを変換または再利用して、低いベース コンピューティング レート (Linux 仮想マシン レートなど) で Windows Server 仮想マシンを Azure で実行できます。</span><span class="sxs-lookup"><span data-stu-id="b73c6-113">Depending on the edition, you can convert or re-use your licenses to run Windows Server virtual machines in Azure and pay a lower base compute rate (Linux virtual machine rates, for example).</span></span>

## <a name="azure-reservations-unavailable-markets"></a><span data-ttu-id="b73c6-114">Azure Reservations を利用できない市場</span><span class="sxs-lookup"><span data-stu-id="b73c6-114">Azure reservations unavailable markets</span></span>

>[!IMPORTANT]
><span data-ttu-id="b73c6-115">次の市場では Azure Reservations を "**利用できません**"。</span><span class="sxs-lookup"><span data-stu-id="b73c6-115">Azure reservations **are not** available in the following markets:</span></span>  
>  
> <span data-ttu-id="b73c6-116">**利用できない市場 (アルファベット順)**</span><span class="sxs-lookup"><span data-stu-id="b73c6-116">**Unavailable markets (in alphabetical order)**</span></span>
>
> |<span data-ttu-id="b73c6-117">A から Gi</span><span class="sxs-lookup"><span data-stu-id="b73c6-117">A to Gi</span></span>   | <span data-ttu-id="b73c6-118">Gr から Pal</span><span class="sxs-lookup"><span data-stu-id="b73c6-118">Gr to Pal</span></span>  | <span data-ttu-id="b73c6-119">Pap から Z</span><span class="sxs-lookup"><span data-stu-id="b73c6-119">Pap to Z</span></span> |
> |--------------------------------|-----------------------------------|------------------------------------------|
> | <span data-ttu-id="b73c6-120">オーランド諸島</span><span class="sxs-lookup"><span data-stu-id="b73c6-120">Aland Islands</span></span>     | <span data-ttu-id="b73c6-121">グリーンランド</span><span class="sxs-lookup"><span data-stu-id="b73c6-121">Greenland</span></span>     | <span data-ttu-id="b73c6-122">パプアニューギニア</span><span class="sxs-lookup"><span data-stu-id="b73c6-122">Papua New Guinea</span></span>     |
> | <span data-ttu-id="b73c6-123">米領サモア</span><span class="sxs-lookup"><span data-stu-id="b73c6-123">American Samoa</span></span>     | <span data-ttu-id="b73c6-124">グレナダ</span><span class="sxs-lookup"><span data-stu-id="b73c6-124">Grenada</span></span>     | <span data-ttu-id="b73c6-125">ピトケアン島</span><span class="sxs-lookup"><span data-stu-id="b73c6-125">Pitcairn Islands</span></span>     |
> | <span data-ttu-id="b73c6-126">アンドラ</span><span class="sxs-lookup"><span data-stu-id="b73c6-126">Andorra</span></span>     | <span data-ttu-id="b73c6-127">グアドループ</span><span class="sxs-lookup"><span data-stu-id="b73c6-127">Guadeloupe</span></span>     | <span data-ttu-id="b73c6-128">レユニオン</span><span class="sxs-lookup"><span data-stu-id="b73c6-128">Reunion</span></span>     |
> | <span data-ttu-id="b73c6-129">アンギラ</span><span class="sxs-lookup"><span data-stu-id="b73c6-129">Anguilla</span></span>     | <span data-ttu-id="b73c6-130">グアム</span><span class="sxs-lookup"><span data-stu-id="b73c6-130">Guam</span></span>     | <span data-ttu-id="b73c6-131">サバ島</span><span class="sxs-lookup"><span data-stu-id="b73c6-131">Saba</span></span>   |
> | <span data-ttu-id="b73c6-132">南極</span><span class="sxs-lookup"><span data-stu-id="b73c6-132">Antarctica</span></span>     | <span data-ttu-id="b73c6-133">ガーンジー島</span><span class="sxs-lookup"><span data-stu-id="b73c6-133">Guernsey</span></span>     | <span data-ttu-id="b73c6-134">サン・バルテルミー</span><span class="sxs-lookup"><span data-stu-id="b73c6-134">Saint Barthélemy</span></span>   |
> | <span data-ttu-id="b73c6-135">アンティグア・バーブーダ</span><span class="sxs-lookup"><span data-stu-id="b73c6-135">Antigua and Barbuda</span></span>       | <span data-ttu-id="b73c6-136">ギニア</span><span class="sxs-lookup"><span data-stu-id="b73c6-136">Guinea</span></span>     | <span data-ttu-id="b73c6-137">セントルシア</span><span class="sxs-lookup"><span data-stu-id="b73c6-137">Saint Lucia</span></span>   |
> | <span data-ttu-id="b73c6-138">アルバ</span><span class="sxs-lookup"><span data-stu-id="b73c6-138">Aruba</span></span>       | <span data-ttu-id="b73c6-139">ギニアビサウ</span><span class="sxs-lookup"><span data-stu-id="b73c6-139">Guinea-Bissau</span></span>     | <span data-ttu-id="b73c6-140">サンマルタン島</span><span class="sxs-lookup"><span data-stu-id="b73c6-140">Saint Martin</span></span>   |
> | <span data-ttu-id="b73c6-141">アゼルバイジャン</span><span class="sxs-lookup"><span data-stu-id="b73c6-141">Azerbaijan</span></span>       | <span data-ttu-id="b73c6-142">ガイアナ</span><span class="sxs-lookup"><span data-stu-id="b73c6-142">Guyana</span></span>     | <span data-ttu-id="b73c6-143">サンピエール・ミクロン</span><span class="sxs-lookup"><span data-stu-id="b73c6-143">Saint Pierre and Miquelon</span></span>   |
> | <span data-ttu-id="b73c6-144">ベナン</span><span class="sxs-lookup"><span data-stu-id="b73c6-144">Benin</span></span>     | <span data-ttu-id="b73c6-145">ハイチ</span><span class="sxs-lookup"><span data-stu-id="b73c6-145">Haiti</span></span>       | <span data-ttu-id="b73c6-146">セントビンセントおよびグレナディーン諸島</span><span class="sxs-lookup"><span data-stu-id="b73c6-146">Saint Vincent and the Grenadines</span></span>     |
> | <span data-ttu-id="b73c6-147">ブータン</span><span class="sxs-lookup"><span data-stu-id="b73c6-147">Bhutan</span></span>     | <span data-ttu-id="b73c6-148">ハード・マクドナルド諸島</span><span class="sxs-lookup"><span data-stu-id="b73c6-148">Heard Island and McDonald Islands</span></span>       | <span data-ttu-id="b73c6-149">サモア</span><span class="sxs-lookup"><span data-stu-id="b73c6-149">Samoa</span></span>     |
> | <span data-ttu-id="b73c6-150">ボネール島</span><span class="sxs-lookup"><span data-stu-id="b73c6-150">Bonaire</span></span>     | <span data-ttu-id="b73c6-151">マン島</span><span class="sxs-lookup"><span data-stu-id="b73c6-151">Isle of Man</span></span>     | <span data-ttu-id="b73c6-152">サンマリノ</span><span class="sxs-lookup"><span data-stu-id="b73c6-152">San Marino</span></span>     |
> | <span data-ttu-id="b73c6-153">ブーベ島</span><span class="sxs-lookup"><span data-stu-id="b73c6-153">Bouvet Island</span></span>     | <span data-ttu-id="b73c6-154">ヤンマイエン島</span><span class="sxs-lookup"><span data-stu-id="b73c6-154">Jan Mayen</span></span>     | <span data-ttu-id="b73c6-155">サントメ・プリンシペ</span><span class="sxs-lookup"><span data-stu-id="b73c6-155">São Tomé and Príncipe</span></span>   |
> | <span data-ttu-id="b73c6-156">英領インド洋地域</span><span class="sxs-lookup"><span data-stu-id="b73c6-156">British Indian Ocean Territory</span></span>       | <span data-ttu-id="b73c6-157">ジャージー島</span><span class="sxs-lookup"><span data-stu-id="b73c6-157">Jersey</span></span>     | <span data-ttu-id="b73c6-158">セーシェル</span><span class="sxs-lookup"><span data-stu-id="b73c6-158">Seychelles</span></span>   |
> | <span data-ttu-id="b73c6-159">英領バージン諸島</span><span class="sxs-lookup"><span data-stu-id="b73c6-159">British Virgin Islands</span></span>     | <span data-ttu-id="b73c6-160">キリバス</span><span class="sxs-lookup"><span data-stu-id="b73c6-160">Kiribati</span></span>       | <span data-ttu-id="b73c6-161">シエラレオネ</span><span class="sxs-lookup"><span data-stu-id="b73c6-161">Sierra Leone</span></span>   |
> | <span data-ttu-id="b73c6-162">ブルキナファソ</span><span class="sxs-lookup"><span data-stu-id="b73c6-162">Burkina Faso</span></span>     | <span data-ttu-id="b73c6-163">コソボ</span><span class="sxs-lookup"><span data-stu-id="b73c6-163">Kosovo</span></span>     | <span data-ttu-id="b73c6-164">シント・ユースタティウス島</span><span class="sxs-lookup"><span data-stu-id="b73c6-164">Sint Eustatius</span></span>     |
> | <span data-ttu-id="b73c6-165">ブルンジ</span><span class="sxs-lookup"><span data-stu-id="b73c6-165">Burundi</span></span>     | <span data-ttu-id="b73c6-166">ラオス</span><span class="sxs-lookup"><span data-stu-id="b73c6-166">Laos</span></span>     | <span data-ttu-id="b73c6-167">シント・マールテン島</span><span class="sxs-lookup"><span data-stu-id="b73c6-167">Sint Maarten</span></span>     |
> | <span data-ttu-id="b73c6-168">カンボジア</span><span class="sxs-lookup"><span data-stu-id="b73c6-168">Cambodia</span></span>     | <span data-ttu-id="b73c6-169">レソト</span><span class="sxs-lookup"><span data-stu-id="b73c6-169">Lesotho</span></span>     | <span data-ttu-id="b73c6-170">ソロモン諸島</span><span class="sxs-lookup"><span data-stu-id="b73c6-170">Solomon Islands</span></span>     |
> | <span data-ttu-id="b73c6-171">中央アフリカ共和国</span><span class="sxs-lookup"><span data-stu-id="b73c6-171">Central African Republic</span></span>     | <span data-ttu-id="b73c6-172">リベリア</span><span class="sxs-lookup"><span data-stu-id="b73c6-172">Liberia</span></span>     | <span data-ttu-id="b73c6-173">ソマリア</span><span class="sxs-lookup"><span data-stu-id="b73c6-173">Somalia</span></span>     |
> | <span data-ttu-id="b73c6-174">チャド</span><span class="sxs-lookup"><span data-stu-id="b73c6-174">Chad</span></span>     | <span data-ttu-id="b73c6-175">マダガスカル</span><span class="sxs-lookup"><span data-stu-id="b73c6-175">Madagascar</span></span>     | <span data-ttu-id="b73c6-176">サウスジョージア・サウスサンドウィッチ諸島</span><span class="sxs-lookup"><span data-stu-id="b73c6-176">South Georgia and South Sandwich Islands</span></span>     |
> | <span data-ttu-id="b73c6-177">中国</span><span class="sxs-lookup"><span data-stu-id="b73c6-177">China</span></span>     | <span data-ttu-id="b73c6-178">マラウイ</span><span class="sxs-lookup"><span data-stu-id="b73c6-178">Malawi</span></span>     | <span data-ttu-id="b73c6-179">南スーダン</span><span class="sxs-lookup"><span data-stu-id="b73c6-179">South Sudan</span></span>     |
> | <span data-ttu-id="b73c6-180">クリスマス島</span><span class="sxs-lookup"><span data-stu-id="b73c6-180">Christmas Island</span></span>     | <span data-ttu-id="b73c6-181">モルディブ</span><span class="sxs-lookup"><span data-stu-id="b73c6-181">Maldives</span></span>     | <span data-ttu-id="b73c6-182">セントヘレナ、アセンションおよびトリスタンダクーニャ</span><span class="sxs-lookup"><span data-stu-id="b73c6-182">St Helena, Ascension, Tristan da Cunha</span></span>     |
> | <span data-ttu-id="b73c6-183">ココス諸島</span><span class="sxs-lookup"><span data-stu-id="b73c6-183">Cocos (Keeling) Islands</span></span>     | <span data-ttu-id="b73c6-184">マリ</span><span class="sxs-lookup"><span data-stu-id="b73c6-184">Mali</span></span>     | <span data-ttu-id="b73c6-185">スリナム</span><span class="sxs-lookup"><span data-stu-id="b73c6-185">Suriname</span></span>     |
> | <span data-ttu-id="b73c6-186">コモロ</span><span class="sxs-lookup"><span data-stu-id="b73c6-186">Comoros</span></span>     | <span data-ttu-id="b73c6-187">マーシャル諸島</span><span class="sxs-lookup"><span data-stu-id="b73c6-187">Marshall Islands</span></span>     | <span data-ttu-id="b73c6-188">スバールバル諸島</span><span class="sxs-lookup"><span data-stu-id="b73c6-188">Svalbard</span></span>     |
> | <span data-ttu-id="b73c6-189">コンゴ共和国</span><span class="sxs-lookup"><span data-stu-id="b73c6-189">Congo</span></span>     | <span data-ttu-id="b73c6-190">マルチニーク島</span><span class="sxs-lookup"><span data-stu-id="b73c6-190">Martinique</span></span>     | <span data-ttu-id="b73c6-191">スワジランド</span><span class="sxs-lookup"><span data-stu-id="b73c6-191">Swaziland</span></span>     |
> | <span data-ttu-id="b73c6-192">コンゴ民主共和国</span><span class="sxs-lookup"><span data-stu-id="b73c6-192">Congo (DRC)</span></span>     | <span data-ttu-id="b73c6-193">モーリタニア</span><span class="sxs-lookup"><span data-stu-id="b73c6-193">Mauritania</span></span>     | <span data-ttu-id="b73c6-194">ティモール・レステ</span><span class="sxs-lookup"><span data-stu-id="b73c6-194">Timor-Leste</span></span>   |
> | <span data-ttu-id="b73c6-195">クック諸島</span><span class="sxs-lookup"><span data-stu-id="b73c6-195">Cook Islands</span></span>     | <span data-ttu-id="b73c6-196">マイヨット島</span><span class="sxs-lookup"><span data-stu-id="b73c6-196">Mayotte</span></span>     | <span data-ttu-id="b73c6-197">トーゴ</span><span class="sxs-lookup"><span data-stu-id="b73c6-197">Togo</span></span>   |
> | <span data-ttu-id="b73c6-198">ジブチ</span><span class="sxs-lookup"><span data-stu-id="b73c6-198">Djibouti</span></span>     | <span data-ttu-id="b73c6-199">ミクロネシア</span><span class="sxs-lookup"><span data-stu-id="b73c6-199">Micronesia</span></span>     | <span data-ttu-id="b73c6-200">トケラウ諸島</span><span class="sxs-lookup"><span data-stu-id="b73c6-200">Tokelau</span></span>   |
> | <span data-ttu-id="b73c6-201">ドミニカ国</span><span class="sxs-lookup"><span data-stu-id="b73c6-201">Dominica</span></span>     | <span data-ttu-id="b73c6-202">モンセラット</span><span class="sxs-lookup"><span data-stu-id="b73c6-202">Montserrat</span></span>     | <span data-ttu-id="b73c6-203">トンガ</span><span class="sxs-lookup"><span data-stu-id="b73c6-203">Tonga</span></span>   |
> | <span data-ttu-id="b73c6-204">赤道ギニア</span><span class="sxs-lookup"><span data-stu-id="b73c6-204">Equatorial Guinea</span></span>     | <span data-ttu-id="b73c6-205">モザンビーク</span><span class="sxs-lookup"><span data-stu-id="b73c6-205">Mozambique</span></span>     | <span data-ttu-id="b73c6-206">タークス・カイコス諸島</span><span class="sxs-lookup"><span data-stu-id="b73c6-206">Turks and Caicos Islands</span></span>   |
> | <span data-ttu-id="b73c6-207">エリトリア</span><span class="sxs-lookup"><span data-stu-id="b73c6-207">Eritrea</span></span>     | <span data-ttu-id="b73c6-208">ミャンマー</span><span class="sxs-lookup"><span data-stu-id="b73c6-208">Myanmar</span></span>     | <span data-ttu-id="b73c6-209">ツバル</span><span class="sxs-lookup"><span data-stu-id="b73c6-209">Tuvalu</span></span>   |
> | <span data-ttu-id="b73c6-210">フォークランド諸島</span><span class="sxs-lookup"><span data-stu-id="b73c6-210">Falkland Islands</span></span>     | <span data-ttu-id="b73c6-211">ナウル</span><span class="sxs-lookup"><span data-stu-id="b73c6-211">Nauru</span></span>     | <span data-ttu-id="b73c6-212">米領小離島</span><span class="sxs-lookup"><span data-stu-id="b73c6-212">U.S. Outlying Islands</span></span>   |
> | <span data-ttu-id="b73c6-213">フランス領ギアナ</span><span class="sxs-lookup"><span data-stu-id="b73c6-213">French Guiana</span></span>     | <span data-ttu-id="b73c6-214">ニューカレドニア</span><span class="sxs-lookup"><span data-stu-id="b73c6-214">New Caledonia</span></span>     | <span data-ttu-id="b73c6-215">バヌアツ</span><span class="sxs-lookup"><span data-stu-id="b73c6-215">Vanuatu</span></span>   |
> | <span data-ttu-id="b73c6-216">フランス領ポリネシア</span><span class="sxs-lookup"><span data-stu-id="b73c6-216">French Polynesia</span></span>     | <span data-ttu-id="b73c6-217">ニジェール</span><span class="sxs-lookup"><span data-stu-id="b73c6-217">Niger</span></span>     | <span data-ttu-id="b73c6-218">バチカン市国</span><span class="sxs-lookup"><span data-stu-id="b73c6-218">Vatican City</span></span>   |
> | <span data-ttu-id="b73c6-219">仏領極南諸島</span><span class="sxs-lookup"><span data-stu-id="b73c6-219">French Southern Territories</span></span>     | <span data-ttu-id="b73c6-220">ニウエ</span><span class="sxs-lookup"><span data-stu-id="b73c6-220">Niue</span></span>     | <span data-ttu-id="b73c6-221">ワリス・フテュナ諸島</span><span class="sxs-lookup"><span data-stu-id="b73c6-221">Wallis and Futuna</span></span>   |
> | <span data-ttu-id="b73c6-222">ガボン</span><span class="sxs-lookup"><span data-stu-id="b73c6-222">Gabon</span></span>     | <span data-ttu-id="b73c6-223">ノーフォーク島</span><span class="sxs-lookup"><span data-stu-id="b73c6-223">Norfolk Island</span></span>     | <span data-ttu-id="b73c6-224">イエメン</span><span class="sxs-lookup"><span data-stu-id="b73c6-224">Yemen</span></span>   |
> | <span data-ttu-id="b73c6-225">ガンビア</span><span class="sxs-lookup"><span data-stu-id="b73c6-225">Gambia</span></span>     | <span data-ttu-id="b73c6-226">北マリアナ諸島</span><span class="sxs-lookup"><span data-stu-id="b73c6-226">Northern Mariana Islands</span></span>     |    |
> | <span data-ttu-id="b73c6-227">ジブラルタル</span><span class="sxs-lookup"><span data-stu-id="b73c6-227">Gibraltar</span></span>     | <span data-ttu-id="b73c6-228">パラオ</span><span class="sxs-lookup"><span data-stu-id="b73c6-228">Palau</span></span>       |    |

## <a name="buy-software-subscriptions-on-behalf-of-customers"></a><span data-ttu-id="b73c6-229">顧客に代わってソフトウェア サブスクリプションを購入する</span><span class="sxs-lookup"><span data-stu-id="b73c6-229">Buy software subscriptions on behalf of customers</span></span>

<span data-ttu-id="b73c6-230">顧客に代わってソフトウェア サブスクリプションを購入するには、次の操作を行います。</span><span class="sxs-lookup"><span data-stu-id="b73c6-230">To buy software subscriptions on behalf of a customer:</span></span>

1. <span data-ttu-id="b73c6-231">パートナー センター [ダッシュボード](https://partner.microsoft.com/dashboard)にサインインします。</span><span class="sxs-lookup"><span data-stu-id="b73c6-231">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="b73c6-232">パートナー センター メニューから **[顧客]** を選択し、一覧から顧客を選びます。</span><span class="sxs-lookup"><span data-stu-id="b73c6-232">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

3. <span data-ttu-id="b73c6-233">顧客の詳細ページから、 **[製品の追加]** を選択した後、画面の指示に従って注文を作成して支払います。</span><span class="sxs-lookup"><span data-stu-id="b73c6-233">From the customer's detail page, select **Add products**, and then follow the on-screen instructions to create and pay for your order.</span></span> <span data-ttu-id="b73c6-234">オーストラリアとブラジルを除き、すべての商用顧客向け価格には税は含まれません。</span><span class="sxs-lookup"><span data-stu-id="b73c6-234">All commercial pricing excludes tax with the exception of Australia and Brazil.</span></span> <span data-ttu-id="b73c6-235">オーストラリアとブラジルの場合は、価格に税が含まれています。</span><span class="sxs-lookup"><span data-stu-id="b73c6-235">For Australia and Brazil, the price includes tax.</span></span>

## <a name="activate-and-manage-software-subscriptions"></a><span data-ttu-id="b73c6-236">ソフトウェア サブスクリプションのライセンス認証と管理</span><span class="sxs-lookup"><span data-stu-id="b73c6-236">Activate and manage software subscriptions</span></span>

<span data-ttu-id="b73c6-237">パートナーがソフトウェアを購入した後、顧客はそれをダウンロードする必要があります。</span><span class="sxs-lookup"><span data-stu-id="b73c6-237">Once you've purchased your software, your customers need to download it.</span></span> <span data-ttu-id="b73c6-238">この場合、次の手順を実行します。</span><span class="sxs-lookup"><span data-stu-id="b73c6-238">Use the following procedure to do this.</span></span>

>[!NOTE]
><span data-ttu-id="b73c6-239">キーとダウンロードへのリンクを取得するには、管理エージェントである必要があります。</span><span class="sxs-lookup"><span data-stu-id="b73c6-239">You must be an Admin agent to obtain the link to keys and downloads.</span></span>

1. <span data-ttu-id="b73c6-240">顧客の詳細ページに移動し、 **[ソフトウェア]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="b73c6-240">Go to your customer's detail page and then select **Software**.</span></span> <span data-ttu-id="b73c6-241">顧客に代わって購入したすべてのソフトウェアの一覧が表示されます。</span><span class="sxs-lookup"><span data-stu-id="b73c6-241">You'll see a list of all the software you've purchased on behalf of the customer.</span></span>
2. <span data-ttu-id="b73c6-242">**[Link to Software product keys and downloads]\(ソフトウェアのプロダクト キーとダウンロードへのリンク\)** から "ディープ リンク" をコピーし、顧客とリンクを共有します。</span><span class="sxs-lookup"><span data-stu-id="b73c6-242">Copy the "deep link" from **Link to Software product keys and downloads** and share the link with your customer.</span></span> <span data-ttu-id="b73c6-243">顧客がこのリンクを選択すると、プロダクト キーをダウンロードして取得できるよう、Microsoft 管理センターにリダイレクトされます。</span><span class="sxs-lookup"><span data-stu-id="b73c6-243">When they select this link, they'll be redirected to the Microsoft Admin Center to download and obtain their product keys.</span></span>

>[!NOTE]
><span data-ttu-id="b73c6-244">Microsoft 管理センターでプロダクト キーを参照したり、情報をダウンロードしたりできるのは、顧客だけです。</span><span class="sxs-lookup"><span data-stu-id="b73c6-244">Only customers can see the product keys and download information in the Microsoft Admin Center.</span></span> <span data-ttu-id="b73c6-245">パートナーがこの情報を見ることはできません。</span><span class="sxs-lookup"><span data-stu-id="b73c6-245">Partners cannot see this information.</span></span>

<span data-ttu-id="b73c6-246">パートナーまたはその顧客がライセンス キーのダウンロードについての詳細を確認したい場合は、[ソフトウェアと製品のライセンス キーのダウンロード](https://go.microsoft.com/fwlink/p/?linkid=2152525)に関するページを参照してください。</span><span class="sxs-lookup"><span data-stu-id="b73c6-246">If you or your customers want to learn more about downloading license keys, see [Download software and product license keys](https://go.microsoft.com/fwlink/p/?linkid=2152525).</span></span>

## <a name="server-subscription-download-and-license-keys-available-through-microsoft-365-admin-center-for-customers"></a><span data-ttu-id="b73c6-247">Microsoft 365 管理センターで顧客向けに使用できるサーバー サブスクリプションのダウンロードとライセンス キー</span><span class="sxs-lookup"><span data-stu-id="b73c6-247">Server subscription download and license keys available through Microsoft 365 Admin Center for customers</span></span> 

<span data-ttu-id="b73c6-248">顧客は CSP サーバー サブスクリプションのライセンス キーとダウンロードを Microsoft 365 管理センターから入手できます。</span><span class="sxs-lookup"><span data-stu-id="b73c6-248">Your customers will be able to get CSP server subscription license keys and downloads from Microsoft 365 Admin Center.</span></span> <span data-ttu-id="b73c6-249">CSP サーバー サブスクリプションのライセンス キーとダウンロードを確認するには、顧客は、Microsoft 365 管理センターにアクセスして、 **[請求] > 自分の製品 > [ソフトウェア] タブ** に移動する必要があります。詳細については、[[請求] の下の [ソフトウェア] タブ](/microsoft-365/admin/whats-new-in-preview#billing--subscriptions)をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="b73c6-249">To see their CSP server subscription license keys and downloads, customer must go to Microsoft 365 Admin Center > **Billing > Your products > Software tab**. For more details refer [Software Tab under Billing](/microsoft-365/admin/whats-new-in-preview#billing--subscriptions).</span></span>  

## <a name="view-activity-for-software-key-access-and-software-downloads"></a><span data-ttu-id="b73c6-250">ソフトウェア キーへのアクセスとソフトウェアのダウンロードに関するアクティビティを表示する</span><span class="sxs-lookup"><span data-stu-id="b73c6-250">View activity for software key access and software downloads</span></span>

<span data-ttu-id="b73c6-251">監査またはコンプライアンスの目的で、サーバー サブスクリプションのソフトウェア キーにアクセスしたか、サーバー サブスクリプション ソフトウェアをダウンロードしたユーザーの一覧を確認することが必要な場合があります。</span><span class="sxs-lookup"><span data-stu-id="b73c6-251">For auditing or compliance purposes, you may need to check a list of users who have either accessed Server subscription software keys or downloaded Server subscription software.</span></span> <span data-ttu-id="b73c6-252">この情報にアクセスするには、以下の手順を実行します。</span><span class="sxs-lookup"><span data-stu-id="b73c6-252">Use the procedure below to access this information.</span></span> 

>[!NOTE]
><span data-ttu-id="b73c6-253">これらのアクティビティ ログを表示するには、グローバル管理者、アカウント管理者、紹介管理者、またはマーケティング コンテンツ管理者になる必要があります。</span><span class="sxs-lookup"><span data-stu-id="b73c6-253">You must be a Global administrator, Account admin, Referral admin, or Marketing content admin to see these activity logs.</span></span> 

1. <span data-ttu-id="b73c6-254">パートナー センター [ダッシュボード](https://partner.microsoft.com/dashboard)にサインインします。</span><span class="sxs-lookup"><span data-stu-id="b73c6-254">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="b73c6-255">右上隅にある歯車アイコンを選択します。</span><span class="sxs-lookup"><span data-stu-id="b73c6-255">Select the gear icon from the upper right corner.</span></span>

3. <span data-ttu-id="b73c6-256">メニューで、 **[アクティビティ ログ]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="b73c6-256">In the menu, select **Activity log**.</span></span>

4. <span data-ttu-id="b73c6-257">表示するアクティビティの日付範囲を入力します。</span><span class="sxs-lookup"><span data-stu-id="b73c6-257">Enter the date range for the activity you want to see.</span></span> <span data-ttu-id="b73c6-258">アクティビティ ログに、指定した期間にソフトウェア キーにアクセスしたか、ソフトウェアをダウンロードしたユーザーの一覧が表示されます。</span><span class="sxs-lookup"><span data-stu-id="b73c6-258">The activity log will display a list of users who have either accessed software keys or downloaded software during the time you specified.</span></span> 

## <a name="cancel-a-purchase"></a><span data-ttu-id="b73c6-259">購入を取り消す</span><span class="sxs-lookup"><span data-stu-id="b73c6-259">Cancel a purchase</span></span>

<span data-ttu-id="b73c6-260">購入日から 60 日以内であればソフトウェア購入を取り消すことができます。</span><span class="sxs-lookup"><span data-stu-id="b73c6-260">You can cancel a software purchase within 60 days of the purchase date.</span></span> <span data-ttu-id="b73c6-261">この最初の 60 日以内に取り消した場合は、中途解約料がかかりません。</span><span class="sxs-lookup"><span data-stu-id="b73c6-261">If you cancel within this first 60-day period, you will not be charged an early termination fee.</span></span> <span data-ttu-id="b73c6-262">60 日を過ぎると、購入の取り消しができなくなります</span><span class="sxs-lookup"><span data-stu-id="b73c6-262">After 60 days, you can no longer cancel a purchase.</span></span> <span data-ttu-id="b73c6-263">(この取り消し規則の主な制限については、「注意」をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="b73c6-263">(See Note for key restrictions to this cancellation rule.</span></span> <span data-ttu-id="b73c6-264">ソフトウェアの購入を取り消した後の処理については、これらの手順の後にある「重要」もご覧ください。)</span><span class="sxs-lookup"><span data-stu-id="b73c6-264">To learn about what happens after you cancel a software purchase, see also Important note after these steps.)</span></span> 

>[!NOTE]
><span data-ttu-id="b73c6-265">購入を取り消すための次の手順は、購入後の最初の 60 日以内など、特定の取り消し期間内に取り消しの対象となったソフトウェアにのみ適用されます。</span><span class="sxs-lookup"><span data-stu-id="b73c6-265">The following steps to cancel a purchase apply only to software that qualifies for cancellation within a specific cancellation window, such as within the first 60 days after purchase.</span></span> <span data-ttu-id="b73c6-266">また、これらの手順は、Azure の SUSE Linux または RedHat ソフトウェア プランには適用されません。</span><span class="sxs-lookup"><span data-stu-id="b73c6-266">These steps also do not apply to a SUSE Linux or RedHat software plan in Azure.</span></span> <span data-ttu-id="b73c6-267">現時点では、SUSE または RedHat ソフトウェア プランのキャンセルや交換はできません。</span><span class="sxs-lookup"><span data-stu-id="b73c6-267">At this time, you cannot cancel or exchange a SUSE or RedHat software plan.</span></span> <span data-ttu-id="b73c6-268">SUSE Linux または RedHat プランの使用方法について詳しくは、[こちらをご覧ください](/azure/virtual-machines/linux/prepay-suse-software-charges)。</span><span class="sxs-lookup"><span data-stu-id="b73c6-268">[Learn more](/azure/virtual-machines/linux/prepay-suse-software-charges) about using SUSE Linux or RedHat plans.</span></span>

<span data-ttu-id="b73c6-269">購入をキャンセルするには、次の手順に従います。</span><span class="sxs-lookup"><span data-stu-id="b73c6-269">Follow the steps below to cancel a purchase:</span></span>

>[!NOTE]
><span data-ttu-id="b73c6-270">購入を取り消すには、管理エージェントである必要があります。</span><span class="sxs-lookup"><span data-stu-id="b73c6-270">You must be an Admin agent to cancel a purchase.</span></span> <span data-ttu-id="b73c6-271">次の手順では、パートナー センター ダッシュボードで購入を取り消す方法について説明します。</span><span class="sxs-lookup"><span data-stu-id="b73c6-271">The following steps describe how to cancel a purchase in the Partner Center dashboard.</span></span> <span data-ttu-id="b73c6-272">この操作は、[パートナー センター API](/partner-center/develop/cancel-software-purchases) を使用して行うこともできます。</span><span class="sxs-lookup"><span data-stu-id="b73c6-272">You can also do this using the [Partner Center API](/partner-center/develop/cancel-software-purchases).</span></span>

1. <span data-ttu-id="b73c6-273">取り消しプロセスを開始する前に、次のものが揃っていることを確認してください。</span><span class="sxs-lookup"><span data-stu-id="b73c6-273">Before you start the cancellation process, make sure you have the following:</span></span>

    - <span data-ttu-id="b73c6-274">顧客の名前、テナント GUID、またはドメイン名</span><span class="sxs-lookup"><span data-stu-id="b73c6-274">The customer's name, tenant GUID or domain name</span></span>

    - <span data-ttu-id="b73c6-275">取り消す製品の名称</span><span class="sxs-lookup"><span data-stu-id="b73c6-275">The name of the product you want to cancel</span></span>
    
    - <span data-ttu-id="b73c6-276">注文 ID</span><span class="sxs-lookup"><span data-stu-id="b73c6-276">The Order ID</span></span>

2. <span data-ttu-id="b73c6-277">パートナー センター [ダッシュボード](https://partner.microsoft.com/dashboard)にサインインします。</span><span class="sxs-lookup"><span data-stu-id="b73c6-277">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

3. <span data-ttu-id="b73c6-278">パートナー センター メニューから **[顧客]** を選択し、一覧から顧客を選びます。</span><span class="sxs-lookup"><span data-stu-id="b73c6-278">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

4. <span data-ttu-id="b73c6-279">顧客の詳細ページで、 **[ソフトウェア]** を選択して、顧客用に購入したソフトウェアの一覧を表示します。</span><span class="sxs-lookup"><span data-stu-id="b73c6-279">On the customer's details page, select **Software** to see the list of software purchased for the customer.</span></span> 

5. <span data-ttu-id="b73c6-280">取り消すソフトウェアの購入を見つけて、 **[キャンセル]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="b73c6-280">Locate the software purchase you want to cancel, and then select **Cancel**.</span></span> <span data-ttu-id="b73c6-281">ダイアログ ボックスが表示されます。</span><span class="sxs-lookup"><span data-stu-id="b73c6-281">A dialog box will appear.</span></span>

6. <span data-ttu-id="b73c6-282">注文番号のドロップダウン リストから、取り消し対象の正しい注文 ID 番号を選択します</span><span class="sxs-lookup"><span data-stu-id="b73c6-282">From the Order number drop-down list, select the correct order ID number you want to cancel.</span></span> <span data-ttu-id="b73c6-283">(注文または注文 ID 番号について詳しくは、顧客の **注文履歴** ページをご覧ください)。</span><span class="sxs-lookup"><span data-stu-id="b73c6-283">(You can learn more information about an order or order ID number from the customer's **Order history** page.)</span></span>

7. <span data-ttu-id="b73c6-284">取り消しに関する **重要な** メッセージに目を通したことを確認するためのチェックボックスをオンにします</span><span class="sxs-lookup"><span data-stu-id="b73c6-284">Select the checkbox to acknowledge that you have read the **Important** message concerning cancellation.</span></span> <span data-ttu-id="b73c6-285">(購入を取り消した後の処理については、以下の「**重要**」をご覧ください)。</span><span class="sxs-lookup"><span data-stu-id="b73c6-285">(Refer to the **Important** note below to learn more about what happens after you cancel a purchase.)</span></span>

8. <span data-ttu-id="b73c6-286">**[送信]** を選択して購入を取り消します。</span><span class="sxs-lookup"><span data-stu-id="b73c6-286">Select **Submit** to cancel your purchase.</span></span> <span data-ttu-id="b73c6-287">顧客の複数の注文を取り消す場合は、一意の注文 ID 番号ごとに手順 4 ～ 6 を繰り返す必要があります。</span><span class="sxs-lookup"><span data-stu-id="b73c6-287">If you want to cancel multiple orders for a customer, you will need to perform Steps 4 through 6 again for each, unique order ID number.</span></span>

<span data-ttu-id="b73c6-288">注文の取り消しを試みると、パートナー センターから他の情報が送られてくることもあります (注文番号のドロップダウン リストの下に表示されます)。</span><span class="sxs-lookup"><span data-stu-id="b73c6-288">When you attempt to cancel an order, Partner Center may also give you other information (that appears below the Order number drop-down list).</span></span> <span data-ttu-id="b73c6-289">この情報には次の項目が含まれていることがあります。</span><span class="sxs-lookup"><span data-stu-id="b73c6-289">This information can include:</span></span>

- <span data-ttu-id="b73c6-290">その注文の取り消しが可能な残り日数</span><span class="sxs-lookup"><span data-stu-id="b73c6-290">How many days remain for you to cancel that particular order</span></span>

- <span data-ttu-id="b73c6-291">取り消し期間を既に過ぎていて注文の取り消しができなくなっているかどうか</span><span class="sxs-lookup"><span data-stu-id="b73c6-291">Whether you have already passed the cancellation window and can no longer cancel the order</span></span>

- <span data-ttu-id="b73c6-292">Microsoft で取り消し要求に関する情報がさらに必要な場合、**カスタマー サポート要求** フォームへのリンクが表示されることがあります。</span><span class="sxs-lookup"><span data-stu-id="b73c6-292">If we need more information about your cancellation request, you may be given a link to a **customer support request** form.</span></span>

>[!IMPORTANT]
><span data-ttu-id="b73c6-293">注文の取り消しが終わると、取り消しを確認するメッセージが表示されます。</span><span class="sxs-lookup"><span data-stu-id="b73c6-293">After you cancel an order, a message confirming your cancellation will appear.</span></span> <span data-ttu-id="b73c6-294">ただし、取り消しがパートナー センター ダッシュボードに表示されるまで、最大 15 分の遅延が発生する場合があります。</span><span class="sxs-lookup"><span data-stu-id="b73c6-294">There may be a delay of up to 15 minutes, however, before the cancellation appears on the Partner Center dashboard.</span></span> 

### <a name="post-cancellation-details"></a><span data-ttu-id="b73c6-295">取り消した後の詳細</span><span class="sxs-lookup"><span data-stu-id="b73c6-295">Post-cancellation details</span></span>

<span data-ttu-id="b73c6-296">購入を取り消した後は、次のようになります。</span><span class="sxs-lookup"><span data-stu-id="b73c6-296">After you cancel a purchase:</span></span>

- <span data-ttu-id="b73c6-297">関連するソフトウェア キーとダウンロード リンクがすべて失効します。</span><span class="sxs-lookup"><span data-stu-id="b73c6-297">All related software keys and download links will be revoked.</span></span> <span data-ttu-id="b73c6-298">つまり、パートナーとパートナーの顧客はこの購入に関連するソフトウェア キーとダウンロード リンクを使用できなくなります。</span><span class="sxs-lookup"><span data-stu-id="b73c6-298">This means neither you nor your customer can use the software keys and download links any longer related to this purchase.</span></span> <span data-ttu-id="b73c6-299">パートナーとパートナーの顧客は、取り消されたすべてのソフトウェアの使用を中止しなければなりません。</span><span class="sxs-lookup"><span data-stu-id="b73c6-299">You and your customer are responsible for discontinuing the use of all canceled software.</span></span> <span data-ttu-id="b73c6-300">さらに、取り消されたソフトウェアをアンインストールし、関連するソフトウェアのダウンロードやリンクもすべて削除しなければなりません。</span><span class="sxs-lookup"><span data-stu-id="b73c6-300">You are also responsible for uninstalling the canceled software and removing any, related software downloads and links.</span></span>

- <span data-ttu-id="b73c6-301">取り消された項目は顧客のソフトウェアの詳細ページに引き続き表示されますが、アクティブ化キーは利用できなくなります。</span><span class="sxs-lookup"><span data-stu-id="b73c6-301">The canceled item will still appear on the customer's Software details page but the activation key will not be available.</span></span>

- <span data-ttu-id="b73c6-302">次回の月次請求書には、取り消された注文の返金額が表示されます。</span><span class="sxs-lookup"><span data-stu-id="b73c6-302">A credit for the canceled order will appear on your next monthly invoice.</span></span> <span data-ttu-id="b73c6-303">永続的ソフトウェアの場合は全額返金され、ソフトウェア サブスクリプションの場合は日割り計算で返金されます。</span><span class="sxs-lookup"><span data-stu-id="b73c6-303">Perpetual software will receive a 100% credit and software subscriptions will receive a prorated credit.</span></span>

### <a name="submit-a-customer-support-request-to-cancel-a-purchase"></a><span data-ttu-id="b73c6-304">購入を取り消すためのカスタマー サポート要求を送信する</span><span class="sxs-lookup"><span data-stu-id="b73c6-304">Submit a customer support request to cancel a purchase</span></span>

<span data-ttu-id="b73c6-305">パートナー センターからソフトウェアの購入の取り消しを試みたが、詳細な情報の提供と、カスタマー サポート要求フォームへの記入を指示された場合は、次の手順が役立つことがあります。</span><span class="sxs-lookup"><span data-stu-id="b73c6-305">If you tried to cancel a software purchase via Partner Center but were told to provide more information and fill out a customer support request form, these steps may help you:</span></span>

1. <span data-ttu-id="b73c6-306">[購入を取り消す] ウィンドウから **[customer support request]\(カスタマー サポート要求\)** リンクを選択すると、 **[パートナー センターに関する問題を報告する]** ページが開きます。</span><span class="sxs-lookup"><span data-stu-id="b73c6-306">When you select the **customer support request** link from the Cancel purchase window, the **Report a problem with Partner Center** page will open.</span></span>

2. <span data-ttu-id="b73c6-307">**[詳細]** の [問題の種類] の一覧で、 **[お客様に代わって CSP を購入/払い戻し]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="b73c6-307">Under **Details**, in the Type of problem list, select **CSP Purchase/Refund on behalf of customers**.</span></span>

3. <span data-ttu-id="b73c6-308">[影響] および [タイトル] フィールドに入力します。</span><span class="sxs-lookup"><span data-stu-id="b73c6-308">Fill in the Impact and Title fields.</span></span>

4. <span data-ttu-id="b73c6-309">[説明] フィールドに、次の情報を入力します。</span><span class="sxs-lookup"><span data-stu-id="b73c6-309">In the Description field, provide the following:</span></span>

    - <span data-ttu-id="b73c6-310">顧客のテナント GUID またはドメイン名</span><span class="sxs-lookup"><span data-stu-id="b73c6-310">The customer tenant GUID or domain name</span></span>
    
    - <span data-ttu-id="b73c6-311">注文 ID またはサブスクリプション ID</span><span class="sxs-lookup"><span data-stu-id="b73c6-311">Order ID or Subscription ID</span></span>
    
    - <span data-ttu-id="b73c6-312">払い戻し理由</span><span class="sxs-lookup"><span data-stu-id="b73c6-312">Refund reason</span></span>

    - <span data-ttu-id="b73c6-313">要求された数量</span><span class="sxs-lookup"><span data-stu-id="b73c6-313">Amount requested</span></span>

5. <span data-ttu-id="b73c6-314">[連絡先] フィールドに、パートナーの名前、メール アドレス、電話番号を入力します。</span><span class="sxs-lookup"><span data-stu-id="b73c6-314">In the Contact field, enter your name, email address, and phone number.</span></span>

6. <span data-ttu-id="b73c6-315">何らかの理由でファイルを添付する必要がある場合は、 **[ファイルの追加]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="b73c6-315">If you need to attach a file for any reason, select **Add files**.</span></span> <span data-ttu-id="b73c6-316">この手順は省略可能です。</span><span class="sxs-lookup"><span data-stu-id="b73c6-316">This step is optional.</span></span>

7. <span data-ttu-id="b73c6-317">終了したら、 **[送信]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="b73c6-317">When you're finished, select **Submit**.</span></span>

## <a name="next-steps"></a><span data-ttu-id="b73c6-318">次の手順</span><span class="sxs-lookup"><span data-stu-id="b73c6-318">Next steps</span></span>

- [<span data-ttu-id="b73c6-319">パートナー センターを使用して、コマーシャル マーケットプレース製品のサブスクリプションを顧客に販売する</span><span class="sxs-lookup"><span data-stu-id="b73c6-319">Use Partner Center to sell customers subscriptions to commercial marketplace products</span></span>](sell-marketplace-products.md)
 
- [<span data-ttu-id="b73c6-320">パートナー センターで顧客に Azure サブスクリプションを割り当てる</span><span class="sxs-lookup"><span data-stu-id="b73c6-320">Assigning Azure subscriptions to customers in Partner Center</span></span>](assign-azure-subscriptions.md)