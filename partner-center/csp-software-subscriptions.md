---
title: CSP によるソフトウェア サブスクリプションの販売
ms.topic: article
ms.date: 06/18/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: CSP プログラムのパートナーがパートナー センターを使用して、顧客に代わって Azure 予約インスタンスとサーバー サブスクリプションの購入、管理、販売、および取り消しを行う方法について説明します。
author: LauraBrenner
ms.author: labrenne
keywords: クラウド ソリューション プロバイダー, CSP, クラウド ベースのサービス, Azure, Azure RI, Windows Server, SQL Server, ソフトウェア サブスクリプション, ソフトウェアの取り消し
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.openlocfilehash: 46d64a72ded1e9b165a84ede50c0baf695a816b7
ms.sourcegitcommit: 11325c74d0c41316fb143beda603177241403b8c
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/23/2020
ms.locfileid: "85267189"
---
# <a name="sell-software-subscriptions-through-the-cloud-solution-provider-csp-program"></a><span data-ttu-id="03b2f-104">クラウド ソリューション プロバイダー (CSP) プログラムによりソフトウェア サブスクリプションを販売する</span><span class="sxs-lookup"><span data-stu-id="03b2f-104">Sell software subscriptions through the Cloud Solution Provider (CSP) program</span></span>

<span data-ttu-id="03b2f-105">**適用対象**</span><span class="sxs-lookup"><span data-stu-id="03b2f-105">**Applies to**</span></span>

- <span data-ttu-id="03b2f-106">クラウド ソリューション プロバイダー</span><span class="sxs-lookup"><span data-stu-id="03b2f-106">Cloud Solution Providers</span></span>

<span data-ttu-id="03b2f-107">**適切なロール**</span><span class="sxs-lookup"><span data-stu-id="03b2f-107">**Appropriate roles**</span></span>

- <span data-ttu-id="03b2f-108">管理エージェント</span><span class="sxs-lookup"><span data-stu-id="03b2f-108">Admin agent</span></span>
- <span data-ttu-id="03b2f-109">グローバル管理者</span><span class="sxs-lookup"><span data-stu-id="03b2f-109">Global admin</span></span>

<span data-ttu-id="03b2f-110">Azure 予約とサーバー サブスクリプション (Windows Server および SQL Server サブスクリプション) を使用すると、CSP プログラムのパートナーは、予測可能性と永続性の高いクラウド ワークロードを、よりコスト効率の優れたソリューションでサポートしたいという顧客の需要の急速な高まりに一層十分に応えられます。</span><span class="sxs-lookup"><span data-stu-id="03b2f-110">With Azure reservations and Server subscriptions (Windows Server and SQL Server subscriptions),partners in the CSP program can better address the fast-growing customer demand for more cost-effective solutions to support highly predictable and persistent cloud workloads.</span></span> 

<span data-ttu-id="03b2f-111">Azure ハイブリッド特典を活用することで、パートナー センターや Azure portal から、企業顧客に代わって Azure 予約とサーバー サブスクリプションを取得、プロビジョニング、および管理できるようになりました。</span><span class="sxs-lookup"><span data-stu-id="03b2f-111">You can now acquire, provision, and manage Azure reservations and Server subscriptions on behalf of commercial customers through Partner Center and the Azure portal by taking advantage of the Azure Hybrid Benefit.</span></span>

<span data-ttu-id="03b2f-112">Azure ハイブリッド特典を利用すると、Windows Server ライセンスから得られる価値を拡大し、仮想マシンのコストを最大で 40% 節約できます。</span><span class="sxs-lookup"><span data-stu-id="03b2f-112">The Azure Hybrid Benefit helps you get more value from your Windows Server licenses and save up to 40 percent on virtual machines.</span></span> <span data-ttu-id="03b2f-113">この特典はソフトウェア アシュアランスに含まれており、Windows Server Datacenter および Standard エディションのライセンスで利用できます。</span><span class="sxs-lookup"><span data-stu-id="03b2f-113">You can use the benefit with Windows Server Datacenter and Standard edition licenses covered with Software Assurance.</span></span> <span data-ttu-id="03b2f-114">エディションによっては、ライセンスを変換または再利用して、低いベース コンピューティング レート (Linux 仮想マシン レートなど) で Windows Server 仮想マシンを Azure で実行できます。</span><span class="sxs-lookup"><span data-stu-id="03b2f-114">Depending on the edition, you can convert or re-use your licenses to run Windows Server virtual machines in Azure and pay a lower base compute rate (Linux virtual machine rates, for example).</span></span>

## <a name="azure-reservations-unavailable-markets"></a><span data-ttu-id="03b2f-115">Azure Reservations を利用できない市場</span><span class="sxs-lookup"><span data-stu-id="03b2f-115">Azure reservations unavailable markets</span></span>

>[!IMPORTANT]
><span data-ttu-id="03b2f-116">次の市場では Azure Reservations を "**利用できません**"。</span><span class="sxs-lookup"><span data-stu-id="03b2f-116">Azure reservations **are not** available in the following markets:</span></span>  
>  
> <span data-ttu-id="03b2f-117">**利用できない市場 (アルファベット順)**</span><span class="sxs-lookup"><span data-stu-id="03b2f-117">**Unavailable markets (in alphabetical order)**</span></span>
>
> |<span data-ttu-id="03b2f-118">A から Gi</span><span class="sxs-lookup"><span data-stu-id="03b2f-118">A to Gi</span></span>   | <span data-ttu-id="03b2f-119">Gr から Pal</span><span class="sxs-lookup"><span data-stu-id="03b2f-119">Gr to Pal</span></span>  | <span data-ttu-id="03b2f-120">Pap から Z</span><span class="sxs-lookup"><span data-stu-id="03b2f-120">Pap to Z</span></span> |
> |--------------------------------|-----------------------------------|------------------------------------------|
> | <span data-ttu-id="03b2f-121">オーランド諸島</span><span class="sxs-lookup"><span data-stu-id="03b2f-121">Aland Islands</span></span>     | <span data-ttu-id="03b2f-122">グリーンランド</span><span class="sxs-lookup"><span data-stu-id="03b2f-122">Greenland</span></span>     | <span data-ttu-id="03b2f-123">パプアニューギニア</span><span class="sxs-lookup"><span data-stu-id="03b2f-123">Papua New Guinea</span></span>     |
> | <span data-ttu-id="03b2f-124">米領サモア</span><span class="sxs-lookup"><span data-stu-id="03b2f-124">American Samoa</span></span>     | <span data-ttu-id="03b2f-125">グレナダ</span><span class="sxs-lookup"><span data-stu-id="03b2f-125">Grenada</span></span>     | <span data-ttu-id="03b2f-126">ピトケアン島</span><span class="sxs-lookup"><span data-stu-id="03b2f-126">Pitcairn Islands</span></span>     |
> | <span data-ttu-id="03b2f-127">アンドラ</span><span class="sxs-lookup"><span data-stu-id="03b2f-127">Andorra</span></span>     | <span data-ttu-id="03b2f-128">グアドループ</span><span class="sxs-lookup"><span data-stu-id="03b2f-128">Guadeloupe</span></span>     | <span data-ttu-id="03b2f-129">レユニオン</span><span class="sxs-lookup"><span data-stu-id="03b2f-129">Reunion</span></span>     |
> | <span data-ttu-id="03b2f-130">アンギラ</span><span class="sxs-lookup"><span data-stu-id="03b2f-130">Anguilla</span></span>     | <span data-ttu-id="03b2f-131">グアム</span><span class="sxs-lookup"><span data-stu-id="03b2f-131">Guam</span></span>     | <span data-ttu-id="03b2f-132">サバ島</span><span class="sxs-lookup"><span data-stu-id="03b2f-132">Saba</span></span>   |
> | <span data-ttu-id="03b2f-133">南極</span><span class="sxs-lookup"><span data-stu-id="03b2f-133">Antarctica</span></span>     | <span data-ttu-id="03b2f-134">ガーンジー島</span><span class="sxs-lookup"><span data-stu-id="03b2f-134">Guernsey</span></span>     | <span data-ttu-id="03b2f-135">サン・バルテルミー</span><span class="sxs-lookup"><span data-stu-id="03b2f-135">Saint Barthélemy</span></span>   |
> | <span data-ttu-id="03b2f-136">アンティグア・バーブーダ</span><span class="sxs-lookup"><span data-stu-id="03b2f-136">Antigua and Barbuda</span></span>       | <span data-ttu-id="03b2f-137">ギニア</span><span class="sxs-lookup"><span data-stu-id="03b2f-137">Guinea</span></span>     | <span data-ttu-id="03b2f-138">セントルシア</span><span class="sxs-lookup"><span data-stu-id="03b2f-138">Saint Lucia</span></span>   |
> | <span data-ttu-id="03b2f-139">アルバ</span><span class="sxs-lookup"><span data-stu-id="03b2f-139">Aruba</span></span>       | <span data-ttu-id="03b2f-140">ギニアビサウ</span><span class="sxs-lookup"><span data-stu-id="03b2f-140">Guinea-Bissau</span></span>     | <span data-ttu-id="03b2f-141">サンマルタン島</span><span class="sxs-lookup"><span data-stu-id="03b2f-141">Saint Martin</span></span>   |
> | <span data-ttu-id="03b2f-142">アゼルバイジャン</span><span class="sxs-lookup"><span data-stu-id="03b2f-142">Azerbaijan</span></span>       | <span data-ttu-id="03b2f-143">ガイアナ</span><span class="sxs-lookup"><span data-stu-id="03b2f-143">Guyana</span></span>     | <span data-ttu-id="03b2f-144">サンピエール・ミクロン</span><span class="sxs-lookup"><span data-stu-id="03b2f-144">Saint Pierre and Miquelon</span></span>   |
> | <span data-ttu-id="03b2f-145">ベナン</span><span class="sxs-lookup"><span data-stu-id="03b2f-145">Benin</span></span>     | <span data-ttu-id="03b2f-146">ハイチ</span><span class="sxs-lookup"><span data-stu-id="03b2f-146">Haiti</span></span>       | <span data-ttu-id="03b2f-147">セントビンセントおよびグレナディーン諸島</span><span class="sxs-lookup"><span data-stu-id="03b2f-147">Saint Vincent and the Grenadines</span></span>     |
> | <span data-ttu-id="03b2f-148">ブータン</span><span class="sxs-lookup"><span data-stu-id="03b2f-148">Bhutan</span></span>     | <span data-ttu-id="03b2f-149">ハード・マクドナルド諸島</span><span class="sxs-lookup"><span data-stu-id="03b2f-149">Heard Island and McDonald Islands</span></span>       | <span data-ttu-id="03b2f-150">サモア</span><span class="sxs-lookup"><span data-stu-id="03b2f-150">Samoa</span></span>     |
> | <span data-ttu-id="03b2f-151">ボネール島</span><span class="sxs-lookup"><span data-stu-id="03b2f-151">Bonaire</span></span>     | <span data-ttu-id="03b2f-152">マン島</span><span class="sxs-lookup"><span data-stu-id="03b2f-152">Isle of Man</span></span>     | <span data-ttu-id="03b2f-153">サンマリノ</span><span class="sxs-lookup"><span data-stu-id="03b2f-153">San Marino</span></span>     |
> | <span data-ttu-id="03b2f-154">ブーベ島</span><span class="sxs-lookup"><span data-stu-id="03b2f-154">Bouvet Island</span></span>     | <span data-ttu-id="03b2f-155">ヤンマイエン島</span><span class="sxs-lookup"><span data-stu-id="03b2f-155">Jan Mayen</span></span>     | <span data-ttu-id="03b2f-156">サントメ・プリンシペ</span><span class="sxs-lookup"><span data-stu-id="03b2f-156">São Tomé and Príncipe</span></span>   |
> | <span data-ttu-id="03b2f-157">英領インド洋地域</span><span class="sxs-lookup"><span data-stu-id="03b2f-157">British Indian Ocean Territory</span></span>       | <span data-ttu-id="03b2f-158">ジャージー島</span><span class="sxs-lookup"><span data-stu-id="03b2f-158">Jersey</span></span>     | <span data-ttu-id="03b2f-159">セーシェル</span><span class="sxs-lookup"><span data-stu-id="03b2f-159">Seychelles</span></span>   |
> | <span data-ttu-id="03b2f-160">英領バージン諸島</span><span class="sxs-lookup"><span data-stu-id="03b2f-160">British Virgin Islands</span></span>     | <span data-ttu-id="03b2f-161">キリバス</span><span class="sxs-lookup"><span data-stu-id="03b2f-161">Kiribati</span></span>       | <span data-ttu-id="03b2f-162">シエラレオネ</span><span class="sxs-lookup"><span data-stu-id="03b2f-162">Sierra Leone</span></span>   |
> | <span data-ttu-id="03b2f-163">ブルキナファソ</span><span class="sxs-lookup"><span data-stu-id="03b2f-163">Burkina Faso</span></span>     | <span data-ttu-id="03b2f-164">コソボ</span><span class="sxs-lookup"><span data-stu-id="03b2f-164">Kosovo</span></span>     | <span data-ttu-id="03b2f-165">シント・ユースタティウス島</span><span class="sxs-lookup"><span data-stu-id="03b2f-165">Sint Eustatius</span></span>     |
> | <span data-ttu-id="03b2f-166">ブルンジ</span><span class="sxs-lookup"><span data-stu-id="03b2f-166">Burundi</span></span>     | <span data-ttu-id="03b2f-167">ラオス</span><span class="sxs-lookup"><span data-stu-id="03b2f-167">Laos</span></span>     | <span data-ttu-id="03b2f-168">シント・マールテン島</span><span class="sxs-lookup"><span data-stu-id="03b2f-168">Sint Maarten</span></span>     |
> | <span data-ttu-id="03b2f-169">カンボジア</span><span class="sxs-lookup"><span data-stu-id="03b2f-169">Cambodia</span></span>     | <span data-ttu-id="03b2f-170">レソト</span><span class="sxs-lookup"><span data-stu-id="03b2f-170">Lesotho</span></span>     | <span data-ttu-id="03b2f-171">ソロモン諸島</span><span class="sxs-lookup"><span data-stu-id="03b2f-171">Solomon Islands</span></span>     |
> | <span data-ttu-id="03b2f-172">中央アフリカ共和国</span><span class="sxs-lookup"><span data-stu-id="03b2f-172">Central African Republic</span></span>     | <span data-ttu-id="03b2f-173">リベリア</span><span class="sxs-lookup"><span data-stu-id="03b2f-173">Liberia</span></span>     | <span data-ttu-id="03b2f-174">ソマリア</span><span class="sxs-lookup"><span data-stu-id="03b2f-174">Somalia</span></span>     |
> | <span data-ttu-id="03b2f-175">チャド</span><span class="sxs-lookup"><span data-stu-id="03b2f-175">Chad</span></span>     | <span data-ttu-id="03b2f-176">マダガスカル</span><span class="sxs-lookup"><span data-stu-id="03b2f-176">Madagascar</span></span>     | <span data-ttu-id="03b2f-177">サウスジョージア・サウスサンドウィッチ諸島</span><span class="sxs-lookup"><span data-stu-id="03b2f-177">South Georgia and South Sandwich Islands</span></span>     |
> | <span data-ttu-id="03b2f-178">中国</span><span class="sxs-lookup"><span data-stu-id="03b2f-178">China</span></span>     | <span data-ttu-id="03b2f-179">マラウイ</span><span class="sxs-lookup"><span data-stu-id="03b2f-179">Malawi</span></span>     | <span data-ttu-id="03b2f-180">南スーダン</span><span class="sxs-lookup"><span data-stu-id="03b2f-180">South Sudan</span></span>     |
> | <span data-ttu-id="03b2f-181">クリスマス島</span><span class="sxs-lookup"><span data-stu-id="03b2f-181">Christmas Island</span></span>     | <span data-ttu-id="03b2f-182">モルディブ</span><span class="sxs-lookup"><span data-stu-id="03b2f-182">Maldives</span></span>     | <span data-ttu-id="03b2f-183">セントヘレナ、アセンションおよびトリスタンダクーニャ</span><span class="sxs-lookup"><span data-stu-id="03b2f-183">St Helena, Ascension, Tristan da Cunha</span></span>     |
> | <span data-ttu-id="03b2f-184">ココス諸島</span><span class="sxs-lookup"><span data-stu-id="03b2f-184">Cocos (Keeling) Islands</span></span>     | <span data-ttu-id="03b2f-185">マリ</span><span class="sxs-lookup"><span data-stu-id="03b2f-185">Mali</span></span>     | <span data-ttu-id="03b2f-186">スリナム</span><span class="sxs-lookup"><span data-stu-id="03b2f-186">Suriname</span></span>     |
> | <span data-ttu-id="03b2f-187">コモロ</span><span class="sxs-lookup"><span data-stu-id="03b2f-187">Comoros</span></span>     | <span data-ttu-id="03b2f-188">マーシャル諸島</span><span class="sxs-lookup"><span data-stu-id="03b2f-188">Marshall Islands</span></span>     | <span data-ttu-id="03b2f-189">スバールバル諸島</span><span class="sxs-lookup"><span data-stu-id="03b2f-189">Svalbard</span></span>     |
> | <span data-ttu-id="03b2f-190">コンゴ共和国</span><span class="sxs-lookup"><span data-stu-id="03b2f-190">Congo</span></span>     | <span data-ttu-id="03b2f-191">マルチニーク島</span><span class="sxs-lookup"><span data-stu-id="03b2f-191">Martinique</span></span>     | <span data-ttu-id="03b2f-192">スワジランド</span><span class="sxs-lookup"><span data-stu-id="03b2f-192">Swaziland</span></span>     |
> | <span data-ttu-id="03b2f-193">コンゴ民主共和国</span><span class="sxs-lookup"><span data-stu-id="03b2f-193">Congo (DRC)</span></span>     | <span data-ttu-id="03b2f-194">モーリタニア</span><span class="sxs-lookup"><span data-stu-id="03b2f-194">Mauritania</span></span>     | <span data-ttu-id="03b2f-195">ティモール・レステ</span><span class="sxs-lookup"><span data-stu-id="03b2f-195">Timor-Leste</span></span>   |
> | <span data-ttu-id="03b2f-196">クック諸島</span><span class="sxs-lookup"><span data-stu-id="03b2f-196">Cook Islands</span></span>     | <span data-ttu-id="03b2f-197">マイヨット島</span><span class="sxs-lookup"><span data-stu-id="03b2f-197">Mayotte</span></span>     | <span data-ttu-id="03b2f-198">トーゴ</span><span class="sxs-lookup"><span data-stu-id="03b2f-198">Togo</span></span>   |
> | <span data-ttu-id="03b2f-199">ジブチ</span><span class="sxs-lookup"><span data-stu-id="03b2f-199">Djibouti</span></span>     | <span data-ttu-id="03b2f-200">ミクロネシア</span><span class="sxs-lookup"><span data-stu-id="03b2f-200">Micronesia</span></span>     | <span data-ttu-id="03b2f-201">トケラウ諸島</span><span class="sxs-lookup"><span data-stu-id="03b2f-201">Tokelau</span></span>   |
> | <span data-ttu-id="03b2f-202">ドミニカ国</span><span class="sxs-lookup"><span data-stu-id="03b2f-202">Dominica</span></span>     | <span data-ttu-id="03b2f-203">モンセラット</span><span class="sxs-lookup"><span data-stu-id="03b2f-203">Montserrat</span></span>     | <span data-ttu-id="03b2f-204">トンガ</span><span class="sxs-lookup"><span data-stu-id="03b2f-204">Tonga</span></span>   |
> | <span data-ttu-id="03b2f-205">赤道ギニア</span><span class="sxs-lookup"><span data-stu-id="03b2f-205">Equatorial Guinea</span></span>     | <span data-ttu-id="03b2f-206">モザンビーク</span><span class="sxs-lookup"><span data-stu-id="03b2f-206">Mozambique</span></span>     | <span data-ttu-id="03b2f-207">タークス・カイコス諸島</span><span class="sxs-lookup"><span data-stu-id="03b2f-207">Turks and Caicos Islands</span></span>   |
> | <span data-ttu-id="03b2f-208">エリトリア</span><span class="sxs-lookup"><span data-stu-id="03b2f-208">Eritrea</span></span>     | <span data-ttu-id="03b2f-209">ミャンマー</span><span class="sxs-lookup"><span data-stu-id="03b2f-209">Myanmar</span></span>     | <span data-ttu-id="03b2f-210">ツバル</span><span class="sxs-lookup"><span data-stu-id="03b2f-210">Tuvalu</span></span>   |
> | <span data-ttu-id="03b2f-211">フォークランド諸島</span><span class="sxs-lookup"><span data-stu-id="03b2f-211">Falkland Islands</span></span>     | <span data-ttu-id="03b2f-212">ナウル</span><span class="sxs-lookup"><span data-stu-id="03b2f-212">Nauru</span></span>     | <span data-ttu-id="03b2f-213">米領小離島</span><span class="sxs-lookup"><span data-stu-id="03b2f-213">U.S. Outlying Islands</span></span>   |
> | <span data-ttu-id="03b2f-214">フランス領ギアナ</span><span class="sxs-lookup"><span data-stu-id="03b2f-214">French Guiana</span></span>     | <span data-ttu-id="03b2f-215">ニューカレドニア</span><span class="sxs-lookup"><span data-stu-id="03b2f-215">New Caledonia</span></span>     | <span data-ttu-id="03b2f-216">バヌアツ</span><span class="sxs-lookup"><span data-stu-id="03b2f-216">Vanuatu</span></span>   |
> | <span data-ttu-id="03b2f-217">フランス領ポリネシア</span><span class="sxs-lookup"><span data-stu-id="03b2f-217">French Polynesia</span></span>     | <span data-ttu-id="03b2f-218">ニジェール</span><span class="sxs-lookup"><span data-stu-id="03b2f-218">Niger</span></span>     | <span data-ttu-id="03b2f-219">バチカン市国</span><span class="sxs-lookup"><span data-stu-id="03b2f-219">Vatican City</span></span>   |
> | <span data-ttu-id="03b2f-220">仏領極南諸島</span><span class="sxs-lookup"><span data-stu-id="03b2f-220">French Southern Territories</span></span>     | <span data-ttu-id="03b2f-221">ニウエ</span><span class="sxs-lookup"><span data-stu-id="03b2f-221">Niue</span></span>     | <span data-ttu-id="03b2f-222">ワリス・フテュナ諸島</span><span class="sxs-lookup"><span data-stu-id="03b2f-222">Wallis and Futuna</span></span>   |
> | <span data-ttu-id="03b2f-223">ガボン</span><span class="sxs-lookup"><span data-stu-id="03b2f-223">Gabon</span></span>     | <span data-ttu-id="03b2f-224">ノーフォーク島</span><span class="sxs-lookup"><span data-stu-id="03b2f-224">Norfolk Island</span></span>     | <span data-ttu-id="03b2f-225">イエメン</span><span class="sxs-lookup"><span data-stu-id="03b2f-225">Yemen</span></span>   |
> | <span data-ttu-id="03b2f-226">ガンビア</span><span class="sxs-lookup"><span data-stu-id="03b2f-226">Gambia</span></span>     | <span data-ttu-id="03b2f-227">北マリアナ諸島</span><span class="sxs-lookup"><span data-stu-id="03b2f-227">Northern Mariana Islands</span></span>     |    |
> | <span data-ttu-id="03b2f-228">ジブラルタル</span><span class="sxs-lookup"><span data-stu-id="03b2f-228">Gibraltar</span></span>     | <span data-ttu-id="03b2f-229">パラオ</span><span class="sxs-lookup"><span data-stu-id="03b2f-229">Palau</span></span>       |    |

## <a name="buy-software-subscriptions-on-behalf-of-customers"></a><span data-ttu-id="03b2f-230">顧客に代わってソフトウェア サブスクリプションを購入する</span><span class="sxs-lookup"><span data-stu-id="03b2f-230">Buy software subscriptions on behalf of customers</span></span>

<span data-ttu-id="03b2f-231">顧客に代わってソフトウェア サブスクリプションを購入するには、次の操作を行います。</span><span class="sxs-lookup"><span data-stu-id="03b2f-231">To buy software subscriptions on behalf of a customer:</span></span>

1. <span data-ttu-id="03b2f-232">パートナー センター [ダッシュボード](https://partner.microsoft.com/dashboard)にサインインします。</span><span class="sxs-lookup"><span data-stu-id="03b2f-232">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="03b2f-233">パートナー センター メニューから **[顧客]** を選択し、一覧から顧客を選びます。</span><span class="sxs-lookup"><span data-stu-id="03b2f-233">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

3. <span data-ttu-id="03b2f-234">顧客の詳細ページから、 **[製品の追加]** を選択した後、画面の指示に従って注文を作成して支払います。</span><span class="sxs-lookup"><span data-stu-id="03b2f-234">From the customer's detail page, select **Add products**, and then follow the on-screen instructions to create and pay for your order.</span></span> <span data-ttu-id="03b2f-235">オーストラリアとブラジルを除き、すべての商用顧客向け価格には税は含まれません。</span><span class="sxs-lookup"><span data-stu-id="03b2f-235">All commercial pricing excludes tax with the exception of Australia and Brazil.</span></span> <span data-ttu-id="03b2f-236">オーストラリアとブラジルの場合は、価格に税が含まれています。</span><span class="sxs-lookup"><span data-stu-id="03b2f-236">For Australia and Brazil, the price includes tax.</span></span>

## <a name="activate-and-manage-software-subscriptions"></a><span data-ttu-id="03b2f-237">ソフトウェア サブスクリプションのライセンス認証と管理</span><span class="sxs-lookup"><span data-stu-id="03b2f-237">Activate and manage software subscriptions</span></span>

<span data-ttu-id="03b2f-238">ソフトウェア サブスクリプションを購入した後は、次の手順に従ってダウンロードします。</span><span class="sxs-lookup"><span data-stu-id="03b2f-238">After you purchase the software subscription, follow the steps below to download it.</span></span>

>[!NOTE]
><span data-ttu-id="03b2f-239">ソフトウェアをダウンロードしてライセンス認証キーを取得するには、管理エージェントである必要があります。</span><span class="sxs-lookup"><span data-stu-id="03b2f-239">You must be an Admin agent to download software and get activation keys.</span></span>

1. <span data-ttu-id="03b2f-240">パートナー センター [ダッシュボード](https://partner.microsoft.com/dashboard)にサインインします。</span><span class="sxs-lookup"><span data-stu-id="03b2f-240">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="03b2f-241">パートナー センター メニューから **[顧客]** を選択し、一覧から顧客を選びます。</span><span class="sxs-lookup"><span data-stu-id="03b2f-241">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

3. <span data-ttu-id="03b2f-242">顧客の詳細ページに移動し、 **[ソフトウェア]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="03b2f-242">Go to your customer's detail page and then select **Software**.</span></span> <span data-ttu-id="03b2f-243">顧客に代わって購入したすべてのソフトウェアの一覧が表示されます。</span><span class="sxs-lookup"><span data-stu-id="03b2f-243">You'll see a list of all the software you've purchased on behalf of the customer.</span></span> 

4. <span data-ttu-id="03b2f-244">ダウンロードする製品を展開します。</span><span class="sxs-lookup"><span data-stu-id="03b2f-244">Expand the product you want to download.</span></span> <span data-ttu-id="03b2f-245">**[製品の選択]** フィールドで、目的の **[バージョン]** 、 **[言語]** 、 **[ファイルの種類/OS]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="03b2f-245">In the **Select product** field, select the **Version**, **Language**, and **File type/OS** that you want.</span></span> 

5. <span data-ttu-id="03b2f-246">**[送信]** 選択して特定の製品を表示します。</span><span class="sxs-lookup"><span data-stu-id="03b2f-246">Select **Submit** to display the specific products.</span></span> 

6. <span data-ttu-id="03b2f-247">**[キーとダウンロードの取得]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="03b2f-247">Select **Get keys and downloads**.</span></span> 

7. <span data-ttu-id="03b2f-248">**[ダウンロード]** を選択してダウンロードを開始するか、 **[リンクのコピー]** を選択してリンクをコピーし、顧客に送信します。</span><span class="sxs-lookup"><span data-stu-id="03b2f-248">Select **Download** to begin downloading, or select **Copy link** to copy the link and send it to the customer.</span></span> 

>[!NOTE]
><span data-ttu-id="03b2f-249">このリンクは、2 週間後または 50 回のダウンロードのどちらか早い方のタイミングで期限切れになります。</span><span class="sxs-lookup"><span data-stu-id="03b2f-249">This link will expire after two weeks or 50 downloads, whichever comes first.</span></span> <span data-ttu-id="03b2f-250">リンクが期限切れになった場合は、このページに戻り、 **[キーとダウンロードの取得]** をもう一度選択して、2 週間または 50 回のダウンロードを再び有効にします。</span><span class="sxs-lookup"><span data-stu-id="03b2f-250">Once the link expires, return to this page and select **Get keys and downloads** again to enable another two weeks or 50 downloads.</span></span> <span data-ttu-id="03b2f-251">この操作は、必要な回数だけ行うことができます。</span><span class="sxs-lookup"><span data-stu-id="03b2f-251">You can do this as many times as you need to.</span></span> 

## <a name="server-subscription-download-and-license-keys-available-through-microsoft-365-admin-center-for-customers"></a><span data-ttu-id="03b2f-252">Microsoft 365 管理センターで顧客向けに使用できるサーバー サブスクリプションのダウンロードとライセンス キー</span><span class="sxs-lookup"><span data-stu-id="03b2f-252">Server subscription download and license keys available through Microsoft 365 Admin Center for customers</span></span> 

<span data-ttu-id="03b2f-253">顧客は CSP サーバー サブスクリプションのライセンス キーとダウンロードを Microsoft 365 管理センターから入手できます。</span><span class="sxs-lookup"><span data-stu-id="03b2f-253">Your customers will be able to get CSP server subscription license keys and downloads from Microsoft 365 Admin Center.</span></span> <span data-ttu-id="03b2f-254">CSP サーバー サブスクリプションのライセンス キーとダウンロードを確認するには、顧客は、Microsoft 365 管理センターにアクセスして、 **[請求] > 自分の製品 > [ソフトウェア] タブ**に移動する必要があります。詳細については、[[請求] の下の [ソフトウェア] タブ](https://docs.microsoft.com/microsoft-365/admin/whats-new-in-preview?view=o365-worldwide#billing--subscriptions)をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="03b2f-254">To see their CSP server subscription license keys and downloads, customer must go to Microsoft 365 Admin Center > **Billing > Your products > Software tab**. For more details refer [Software Tab under Billing](https://docs.microsoft.com/microsoft-365/admin/whats-new-in-preview?view=o365-worldwide#billing--subscriptions).</span></span>  

## <a name="view-activity-for-software-key-access-and-software-downloads"></a><span data-ttu-id="03b2f-255">ソフトウェア キーへのアクセスとソフトウェアのダウンロードに関するアクティビティを表示する</span><span class="sxs-lookup"><span data-stu-id="03b2f-255">View activity for software key access and software downloads</span></span>

<span data-ttu-id="03b2f-256">監査またはコンプライアンスの目的で、サーバー サブスクリプションのソフトウェア キーにアクセスしたか、サーバー サブスクリプション ソフトウェアをダウンロードしたユーザーの一覧を確認することが必要な場合があります。</span><span class="sxs-lookup"><span data-stu-id="03b2f-256">For auditing or compliance purposes, you may need to check a list of users who have either accessed Server subscription software keys or downloaded Server subscription software.</span></span> <span data-ttu-id="03b2f-257">この情報にアクセスするには、以下の手順を実行します。</span><span class="sxs-lookup"><span data-stu-id="03b2f-257">Use the procedure below to access this information.</span></span> 

>[!NOTE]
><span data-ttu-id="03b2f-258">これらのアクティビティ ログを表示するには、グローバル管理者、アカウント管理者、紹介管理者、またはマーケティング コンテンツ管理者になる必要があります。</span><span class="sxs-lookup"><span data-stu-id="03b2f-258">You must be a Global administrator, Account admin, Referral admin, or Marketing content admin to see these activity logs.</span></span> 

1. <span data-ttu-id="03b2f-259">パートナー センター [ダッシュボード](https://partner.microsoft.com/dashboard)にサインインします。</span><span class="sxs-lookup"><span data-stu-id="03b2f-259">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="03b2f-260">右上隅にある歯車アイコンを選択します。</span><span class="sxs-lookup"><span data-stu-id="03b2f-260">Select the gear icon from the upper right corner.</span></span>

3. <span data-ttu-id="03b2f-261">メニューで、 **[アクティビティ ログ]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="03b2f-261">In the menu, select **Activity log**.</span></span>

4. <span data-ttu-id="03b2f-262">表示するアクティビティの日付範囲を入力します。</span><span class="sxs-lookup"><span data-stu-id="03b2f-262">Enter the date range for the activity you want to see.</span></span> <span data-ttu-id="03b2f-263">アクティビティ ログに、指定した期間にソフトウェア キーにアクセスしたか、ソフトウェアをダウンロードしたユーザーの一覧が表示されます。</span><span class="sxs-lookup"><span data-stu-id="03b2f-263">The activity log will display a list of users who have either accessed software keys or downloaded software during the time you specified.</span></span> 

## <a name="cancel-a-purchase"></a><span data-ttu-id="03b2f-264">購入を取り消す</span><span class="sxs-lookup"><span data-stu-id="03b2f-264">Cancel a purchase</span></span>

<span data-ttu-id="03b2f-265">購入日から 60 日以内であればソフトウェア購入を取り消すことができます。</span><span class="sxs-lookup"><span data-stu-id="03b2f-265">You can cancel a software purchase within 60 days of the purchase date.</span></span> <span data-ttu-id="03b2f-266">この最初の 60 日以内に取り消した場合は、中途解約料がかかりません。</span><span class="sxs-lookup"><span data-stu-id="03b2f-266">If you cancel within this first 60-day period, you will not be charged an early termination fee.</span></span> <span data-ttu-id="03b2f-267">60 日を過ぎると、購入の取り消しができなくなります</span><span class="sxs-lookup"><span data-stu-id="03b2f-267">After 60 days, you can no longer cancel a purchase.</span></span> <span data-ttu-id="03b2f-268">(この取り消し規則の主な制限については、「注意」をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="03b2f-268">(See Note for key restrictions to this cancellation rule.</span></span> <span data-ttu-id="03b2f-269">ソフトウェアの購入を取り消した後の処理については、これらの手順の後にある「重要」もご覧ください。)</span><span class="sxs-lookup"><span data-stu-id="03b2f-269">To learn about what happens after you cancel a software purchase, see also Important note after these steps.)</span></span> 

>[!NOTE]
><span data-ttu-id="03b2f-270">購入を取り消すための次の手順は、購入後の最初の 60 日以内など、特定の取り消し期間内に取り消しの対象となったソフトウェアにのみ適用されます。</span><span class="sxs-lookup"><span data-stu-id="03b2f-270">The following steps to cancel a purchase apply only to software that qualifies for cancellation within a specific cancellation window, such as within the first 60 days after purchase.</span></span> <span data-ttu-id="03b2f-271">また、これらの手順は、Azure の SUSE Linux または RedHat ソフトウェア プランには適用されません。</span><span class="sxs-lookup"><span data-stu-id="03b2f-271">These steps also do not apply to a SUSE Linux or RedHat software plan in Azure.</span></span> <span data-ttu-id="03b2f-272">現時点では、SUSE または RedHat ソフトウェア プランのキャンセルや交換はできません。</span><span class="sxs-lookup"><span data-stu-id="03b2f-272">At this time, you cannot cancel or exchange a SUSE or RedHat software plan.</span></span> <span data-ttu-id="03b2f-273">SUSE Linux または RedHat プランの使用方法について詳しくは、[こちらをご覧ください](https://docs.microsoft.com/azure/virtual-machines/linux/prepay-suse-software-charges)。</span><span class="sxs-lookup"><span data-stu-id="03b2f-273">[Learn more](https://docs.microsoft.com/azure/virtual-machines/linux/prepay-suse-software-charges) about using SUSE Linux or RedHat plans.</span></span>

<span data-ttu-id="03b2f-274">購入をキャンセルするには、次の手順に従います。</span><span class="sxs-lookup"><span data-stu-id="03b2f-274">Follow the steps below to cancel a purchase:</span></span>

>[!NOTE]
><span data-ttu-id="03b2f-275">購入を取り消すには、管理エージェントである必要があります。</span><span class="sxs-lookup"><span data-stu-id="03b2f-275">You must be an Admin agent to cancel a purchase.</span></span> <span data-ttu-id="03b2f-276">次の手順では、パートナー センター ダッシュボードで購入を取り消す方法について説明します。</span><span class="sxs-lookup"><span data-stu-id="03b2f-276">The following steps describe how to cancel a purchase in the Partner Center dashboard.</span></span> <span data-ttu-id="03b2f-277">この操作は、[パートナー センター API](https://docs.microsoft.com/partner-center/develop/cancel-software-purchases) を使用して行うこともできます。</span><span class="sxs-lookup"><span data-stu-id="03b2f-277">You can also do this using the [Partner Center API](https://docs.microsoft.com/partner-center/develop/cancel-software-purchases).</span></span>

1. <span data-ttu-id="03b2f-278">取り消しプロセスを開始する前に、次のものが揃っていることを確認してください。</span><span class="sxs-lookup"><span data-stu-id="03b2f-278">Before you start the cancellation process, make sure you have the following:</span></span>

    - <span data-ttu-id="03b2f-279">顧客の名前、テナント GUID、またはドメイン名</span><span class="sxs-lookup"><span data-stu-id="03b2f-279">The customer's name, tenant GUID or domain name</span></span>

    - <span data-ttu-id="03b2f-280">取り消す製品の名称</span><span class="sxs-lookup"><span data-stu-id="03b2f-280">The name of the product you want to cancel</span></span>
    
    - <span data-ttu-id="03b2f-281">注文 ID</span><span class="sxs-lookup"><span data-stu-id="03b2f-281">The Order ID</span></span>

2. <span data-ttu-id="03b2f-282">パートナー センター [ダッシュボード](https://partner.microsoft.com/dashboard)にサインインします。</span><span class="sxs-lookup"><span data-stu-id="03b2f-282">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

3. <span data-ttu-id="03b2f-283">パートナー センター メニューから **[顧客]** を選択し、一覧から顧客を選びます。</span><span class="sxs-lookup"><span data-stu-id="03b2f-283">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

4. <span data-ttu-id="03b2f-284">顧客の詳細ページで、 **[ソフトウェア]** を選択して、顧客に代わって購入したソフトウェアの一覧を表示します。</span><span class="sxs-lookup"><span data-stu-id="03b2f-284">On the customer’s details page, select **Software** to see the list of software purchased for the customer.</span></span> 

5. <span data-ttu-id="03b2f-285">取り消すソフトウェアの購入を見つけて、 **[キャンセル]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="03b2f-285">Locate the software purchase you want to cancel, and then select **Cancel**.</span></span> <span data-ttu-id="03b2f-286">ダイアログ ボックスが表示されます。</span><span class="sxs-lookup"><span data-stu-id="03b2f-286">A dialog box will appear.</span></span>

6. <span data-ttu-id="03b2f-287">注文番号のドロップダウン リストから、取り消し対象の正しい注文 ID 番号を選択します</span><span class="sxs-lookup"><span data-stu-id="03b2f-287">From the Order number drop-down list, select the correct order ID number you want to cancel.</span></span> <span data-ttu-id="03b2f-288">(注文または注文 ID 番号について詳しくは、顧客の**注文履歴**ページをご覧ください)。</span><span class="sxs-lookup"><span data-stu-id="03b2f-288">(You can learn more information about an order or order ID number from the customer's **Order history** page.)</span></span>

7. <span data-ttu-id="03b2f-289">取り消しに関する**重要な**メッセージに目を通したことを確認するためのチェックボックスをオンにします</span><span class="sxs-lookup"><span data-stu-id="03b2f-289">Select the checkbox to acknowledge that you have read the **Important** message concerning cancellation.</span></span> <span data-ttu-id="03b2f-290">(購入を取り消した後の処理については、以下の「**重要**」をご覧ください)。</span><span class="sxs-lookup"><span data-stu-id="03b2f-290">(Refer to the **Important** note below to learn more about what happens after you cancel a purchase.)</span></span>

8. <span data-ttu-id="03b2f-291">**[送信]** を選択して購入を取り消します。</span><span class="sxs-lookup"><span data-stu-id="03b2f-291">Select **Submit** to cancel your purchase.</span></span> <span data-ttu-id="03b2f-292">顧客の複数の注文を取り消す場合は、一意の注文 ID 番号ごとに手順 4 ～ 6 を繰り返す必要があります。</span><span class="sxs-lookup"><span data-stu-id="03b2f-292">If you want to cancel multiple orders for a customer, you will need to perform Steps 4 through 6 again for each, unique order ID number.</span></span>

<span data-ttu-id="03b2f-293">注文の取り消しを試みると、パートナー センターから他の情報が送られてくることもあります (注文番号のドロップダウン リストの下に表示されます)。</span><span class="sxs-lookup"><span data-stu-id="03b2f-293">When you attempt to cancel an order, Partner Center may also give you other information (that appears below the Order number drop-down list).</span></span> <span data-ttu-id="03b2f-294">この情報には次の項目が含まれていることがあります。</span><span class="sxs-lookup"><span data-stu-id="03b2f-294">This information can include:</span></span>

- <span data-ttu-id="03b2f-295">その注文の取り消しが可能な残り日数</span><span class="sxs-lookup"><span data-stu-id="03b2f-295">How many days remain for you to cancel that particular order</span></span>

- <span data-ttu-id="03b2f-296">取り消し期間を既に過ぎていて注文の取り消しができなくなっているかどうか</span><span class="sxs-lookup"><span data-stu-id="03b2f-296">Whether you have already passed the cancellation window and can no longer cancel the order</span></span>

- <span data-ttu-id="03b2f-297">Microsoft で取り消し要求に関する情報がさらに必要な場合、**カスタマー サポート要求** フォームへのリンクが表示されることがあります。</span><span class="sxs-lookup"><span data-stu-id="03b2f-297">If we need more information about your cancellation request, you may be given a link to a **customer support request** form.</span></span>

>[!IMPORTANT]
><span data-ttu-id="03b2f-298">注文の取り消しが終わると、取り消しを確認するメッセージが表示されます。</span><span class="sxs-lookup"><span data-stu-id="03b2f-298">After you cancel an order, a message confirming your cancellation will appear.</span></span> <span data-ttu-id="03b2f-299">ただし、取り消しがパートナー センター ダッシュボードに表示されるまで、最大 15 分の遅延が発生する場合があります。</span><span class="sxs-lookup"><span data-stu-id="03b2f-299">There may be a delay of up to 15 minutes, however, before the cancellation appears on the Partner Center dashboard.</span></span> 

### <a name="post-cancellation-details"></a><span data-ttu-id="03b2f-300">取り消した後の詳細</span><span class="sxs-lookup"><span data-stu-id="03b2f-300">Post-cancellation details</span></span>

<span data-ttu-id="03b2f-301">購入を取り消した後は、次のようになります。</span><span class="sxs-lookup"><span data-stu-id="03b2f-301">After you cancel a purchase:</span></span>

- <span data-ttu-id="03b2f-302">関連するソフトウェア キーとダウンロード リンクがすべて失効します。</span><span class="sxs-lookup"><span data-stu-id="03b2f-302">All related software keys and download links will be revoked.</span></span> <span data-ttu-id="03b2f-303">つまり、パートナーとパートナーの顧客はこの購入に関連するソフトウェア キーとダウンロード リンクを使用できなくなります。</span><span class="sxs-lookup"><span data-stu-id="03b2f-303">This means neither you nor your customer can use the software keys and download links any longer related to this purchase.</span></span> <span data-ttu-id="03b2f-304">パートナーとパートナーの顧客は、取り消されたすべてのソフトウェアの使用を中止しなければなりません。</span><span class="sxs-lookup"><span data-stu-id="03b2f-304">You and your customer are responsible for discontinuing the use of all canceled software.</span></span> <span data-ttu-id="03b2f-305">さらに、取り消されたソフトウェアをアンインストールし、関連するソフトウェアのダウンロードやリンクもすべて削除しなければなりません。</span><span class="sxs-lookup"><span data-stu-id="03b2f-305">You are also responsible for uninstalling the canceled software and removing any, related software downloads and links.</span></span>

- <span data-ttu-id="03b2f-306">取り消された項目は顧客のソフトウェアの詳細ページに引き続き表示されますが、アクティブ化キーは利用できなくなります。</span><span class="sxs-lookup"><span data-stu-id="03b2f-306">The canceled item will still appear on the customer's Software details page but the activation key will not be available.</span></span>

- <span data-ttu-id="03b2f-307">次回の月次請求書には、取り消された注文の返金額が表示されます。</span><span class="sxs-lookup"><span data-stu-id="03b2f-307">A credit for the canceled order will appear on your next monthly invoice.</span></span> <span data-ttu-id="03b2f-308">永続的ソフトウェアの場合は全額返金され、ソフトウェア サブスクリプションの場合は日割り計算で返金されます。</span><span class="sxs-lookup"><span data-stu-id="03b2f-308">Perpetual software will receive a 100% credit and software subscriptions will receive a prorated credit.</span></span>

### <a name="submit-a-customer-support-request-to-cancel-a-purchase"></a><span data-ttu-id="03b2f-309">購入を取り消すためのカスタマー サポート要求を送信する</span><span class="sxs-lookup"><span data-stu-id="03b2f-309">Submit a customer support request to cancel a purchase</span></span>

<span data-ttu-id="03b2f-310">パートナー センターからソフトウェアの購入の取り消しを試みたが、詳細な情報の提供と、カスタマー サポート要求フォームへの記入を指示された場合は、次の手順が役立つことがあります。</span><span class="sxs-lookup"><span data-stu-id="03b2f-310">If you tried to cancel a software purchase via Partner Center but were told to provide more information and fill out a customer support request form, these steps may help you:</span></span>

1. <span data-ttu-id="03b2f-311">[購入を取り消す] ウィンドウから **[customer support request]\(カスタマー サポート要求\)** リンクを選択すると、 **[パートナー センターに関する問題を報告する]** ページが開きます。</span><span class="sxs-lookup"><span data-stu-id="03b2f-311">When you select the **customer support request** link from the Cancel purchase window, the **Report a problem with Partner Center** page will open.</span></span>

2. <span data-ttu-id="03b2f-312">**[詳細]** の [問題の種類] の一覧で、 **[お客様に代わって CSP を購入/払い戻し]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="03b2f-312">Under **Details**, in the Type of problem list, select **CSP Purchase/Refund on behalf of customers**.</span></span>

3. <span data-ttu-id="03b2f-313">[影響] および [タイトル] フィールドに入力します。</span><span class="sxs-lookup"><span data-stu-id="03b2f-313">Fill in the Impact and Title fields.</span></span>

4. <span data-ttu-id="03b2f-314">[説明] フィールドに、次の情報を入力します。</span><span class="sxs-lookup"><span data-stu-id="03b2f-314">In the Description field, provide the following:</span></span>

    - <span data-ttu-id="03b2f-315">顧客のテナント GUID またはドメイン名</span><span class="sxs-lookup"><span data-stu-id="03b2f-315">The customer tenant GUID or domain name</span></span>
    
    - <span data-ttu-id="03b2f-316">注文 ID またはサブスクリプション ID</span><span class="sxs-lookup"><span data-stu-id="03b2f-316">Order ID or Subscription ID</span></span>
    
    - <span data-ttu-id="03b2f-317">払い戻し理由</span><span class="sxs-lookup"><span data-stu-id="03b2f-317">Refund reason</span></span>

    - <span data-ttu-id="03b2f-318">要求された数量</span><span class="sxs-lookup"><span data-stu-id="03b2f-318">Amount requested</span></span>

5. <span data-ttu-id="03b2f-319">[連絡先] フィールドに、パートナーの名前、メール アドレス、電話番号を入力します。</span><span class="sxs-lookup"><span data-stu-id="03b2f-319">In the Contact field, enter your name, email address, and phone number.</span></span>

6. <span data-ttu-id="03b2f-320">何らかの理由でファイルを添付する必要がある場合は、 **[ファイルの追加]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="03b2f-320">If you need to attach a file for any reason, select **Add files**.</span></span> <span data-ttu-id="03b2f-321">この手順は省略可能です。</span><span class="sxs-lookup"><span data-stu-id="03b2f-321">This step is optional.</span></span>

7. <span data-ttu-id="03b2f-322">終了したら、 **[送信]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="03b2f-322">When you're finished, select **Submit**.</span></span>

## <a name="next-steps"></a><span data-ttu-id="03b2f-323">次の手順</span><span class="sxs-lookup"><span data-stu-id="03b2f-323">Next steps</span></span>

- [<span data-ttu-id="03b2f-324">パートナー センターを使用して、コマーシャル マーケットプレース製品のサブスクリプションを顧客に販売する</span><span class="sxs-lookup"><span data-stu-id="03b2f-324">Use Partner Center to sell customers subscriptions to commercial marketplace products</span></span>](sell-marketplace-products.md)
 
- [<span data-ttu-id="03b2f-325">パートナー センターで顧客に Azure サブスクリプションを割り当てる</span><span class="sxs-lookup"><span data-stu-id="03b2f-325">Assigning Azure subscriptions to customers in Partner Center</span></span>](assign-azure-subscriptions.md)