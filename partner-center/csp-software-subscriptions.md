---
title: CSP によるソフトウェア サブスクリプションの販売
ms.topic: how-to
ms.date: 03/08/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: CSP プログラムのパートナーがパートナー センターを使用して、顧客に代わって Azure 予約インスタンスとサーバー サブスクリプションの購入、管理、販売、および取り消しを行う方法について説明します。
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.openlocfilehash: ac6169ea6680ea0b36cd5caa3f3e8276f557bea2
ms.sourcegitcommit: 3d7d5064c5e021079ed7e6f93f03869cbf425a32
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/06/2021
ms.locfileid: "106502554"
---
# <a name="sell-software-subscriptions-through-the-cloud-solution-provider-csp-program"></a><span data-ttu-id="2dbaa-103">クラウド ソリューション プロバイダー (CSP) プログラムによりソフトウェア サブスクリプションを販売する</span><span class="sxs-lookup"><span data-stu-id="2dbaa-103">Sell software subscriptions through the Cloud Solution Provider (CSP) program</span></span>

<span data-ttu-id="2dbaa-104">**適切なロール**</span><span class="sxs-lookup"><span data-stu-id="2dbaa-104">**Appropriate roles**</span></span>

- <span data-ttu-id="2dbaa-105">管理エージェント</span><span class="sxs-lookup"><span data-stu-id="2dbaa-105">Admin agent</span></span>
- <span data-ttu-id="2dbaa-106">グローバル管理者</span><span class="sxs-lookup"><span data-stu-id="2dbaa-106">Global admin</span></span>

<span data-ttu-id="2dbaa-107">Azure 予約とサーバー サブスクリプション (Windows Server および SQL Server サブスクリプション) を使用すると、CSP プログラムのパートナーは、予測可能性と永続性がきわめて高いクラウド ワークロードをコスト効率に優れたソリューションでサポートしたいという顧客の強い要望に適切に応えることができます。</span><span class="sxs-lookup"><span data-stu-id="2dbaa-107">With Azure reservations and Server subscriptions (Windows Server and SQL Server subscriptions), partners in the CSP program can better address the fast-growing customer demand for more cost-effective solutions to support highly predictable and persistent cloud workloads.</span></span> 

<span data-ttu-id="2dbaa-108">Azure ハイブリッド特典を活用することで、パートナー センターや Azure portal から、企業顧客に代わって Azure 予約とサーバー サブスクリプションを取得、プロビジョニング、および管理できるようになりました。</span><span class="sxs-lookup"><span data-stu-id="2dbaa-108">You can now acquire, provision, and manage Azure reservations and Server subscriptions on behalf of commercial customers through Partner Center and the Azure portal by taking advantage of the Azure Hybrid Benefit.</span></span>

<span data-ttu-id="2dbaa-109">Azure ハイブリッド特典を利用すると、Windows Server ライセンスから得られる価値を拡大し、仮想マシンのコストを最大で 40% 節約できます。</span><span class="sxs-lookup"><span data-stu-id="2dbaa-109">The Azure Hybrid Benefit helps you get more value from your Windows Server licenses and save up to 40 percent on virtual machines.</span></span> <span data-ttu-id="2dbaa-110">この特典はソフトウェア アシュアランスに含まれており、Windows Server Datacenter および Standard エディションのライセンスで利用できます。</span><span class="sxs-lookup"><span data-stu-id="2dbaa-110">You can use the benefit with Windows Server Datacenter and Standard edition licenses covered with Software Assurance.</span></span> <span data-ttu-id="2dbaa-111">エディションによっては、ライセンスを変換または再利用して、低いベース コンピューティング レート (Linux 仮想マシン レートなど) で Windows Server 仮想マシンを Azure で実行できます。</span><span class="sxs-lookup"><span data-stu-id="2dbaa-111">Depending on the edition, you can convert or reuse your licenses to run Windows Server virtual machines in Azure and pay a lower base compute rate (Linux virtual machine rates, for example).</span></span>

## <a name="azure-reservations-unavailable-markets"></a><span data-ttu-id="2dbaa-112">Azure Reservations を利用できない市場</span><span class="sxs-lookup"><span data-stu-id="2dbaa-112">Azure reservations unavailable markets</span></span>

>[!IMPORTANT]
><span data-ttu-id="2dbaa-113">次の市場では Azure Reservations を "**利用できません**"。</span><span class="sxs-lookup"><span data-stu-id="2dbaa-113">Azure reservations **are not** available in the following markets:</span></span>  
>  
> <span data-ttu-id="2dbaa-114">**利用できない市場 (アルファベット順)**</span><span class="sxs-lookup"><span data-stu-id="2dbaa-114">**Unavailable markets (in alphabetical order)**</span></span>
>
> |<span data-ttu-id="2dbaa-115">A から Gi</span><span class="sxs-lookup"><span data-stu-id="2dbaa-115">A to Gi</span></span>   | <span data-ttu-id="2dbaa-116">Gr から Pal</span><span class="sxs-lookup"><span data-stu-id="2dbaa-116">Gr to Pal</span></span>  | <span data-ttu-id="2dbaa-117">Pap から Z</span><span class="sxs-lookup"><span data-stu-id="2dbaa-117">Pap to Z</span></span> |
> |--------------------------------|-----------------------------------|------------------------------------------|
> | <span data-ttu-id="2dbaa-118">オーランド諸島</span><span class="sxs-lookup"><span data-stu-id="2dbaa-118">Aland Islands</span></span>     | <span data-ttu-id="2dbaa-119">グリーンランド</span><span class="sxs-lookup"><span data-stu-id="2dbaa-119">Greenland</span></span>     | <span data-ttu-id="2dbaa-120">パプアニューギニア</span><span class="sxs-lookup"><span data-stu-id="2dbaa-120">Papua New Guinea</span></span>     |
> | <span data-ttu-id="2dbaa-121">米領サモア</span><span class="sxs-lookup"><span data-stu-id="2dbaa-121">American Samoa</span></span>     | <span data-ttu-id="2dbaa-122">グレナダ</span><span class="sxs-lookup"><span data-stu-id="2dbaa-122">Grenada</span></span>     | <span data-ttu-id="2dbaa-123">ピトケアン島</span><span class="sxs-lookup"><span data-stu-id="2dbaa-123">Pitcairn Islands</span></span>     |
> | <span data-ttu-id="2dbaa-124">アンドラ</span><span class="sxs-lookup"><span data-stu-id="2dbaa-124">Andorra</span></span>     | <span data-ttu-id="2dbaa-125">グアドループ</span><span class="sxs-lookup"><span data-stu-id="2dbaa-125">Guadeloupe</span></span>     | <span data-ttu-id="2dbaa-126">レユニオン</span><span class="sxs-lookup"><span data-stu-id="2dbaa-126">Reunion</span></span>     |
> | <span data-ttu-id="2dbaa-127">アンギラ</span><span class="sxs-lookup"><span data-stu-id="2dbaa-127">Anguilla</span></span>     | <span data-ttu-id="2dbaa-128">グアム</span><span class="sxs-lookup"><span data-stu-id="2dbaa-128">Guam</span></span>     | <span data-ttu-id="2dbaa-129">サバ島</span><span class="sxs-lookup"><span data-stu-id="2dbaa-129">Saba</span></span>   |
> | <span data-ttu-id="2dbaa-130">南極</span><span class="sxs-lookup"><span data-stu-id="2dbaa-130">Antarctica</span></span>     | <span data-ttu-id="2dbaa-131">ガーンジー島</span><span class="sxs-lookup"><span data-stu-id="2dbaa-131">Guernsey</span></span>     | <span data-ttu-id="2dbaa-132">サン・バルテルミー</span><span class="sxs-lookup"><span data-stu-id="2dbaa-132">Saint Barthélemy</span></span>   |
> | <span data-ttu-id="2dbaa-133">アンティグア・バーブーダ</span><span class="sxs-lookup"><span data-stu-id="2dbaa-133">Antigua and Barbuda</span></span>       | <span data-ttu-id="2dbaa-134">ギニア</span><span class="sxs-lookup"><span data-stu-id="2dbaa-134">Guinea</span></span>     | <span data-ttu-id="2dbaa-135">セントルシア</span><span class="sxs-lookup"><span data-stu-id="2dbaa-135">Saint Lucia</span></span>   |
> | <span data-ttu-id="2dbaa-136">アルバ</span><span class="sxs-lookup"><span data-stu-id="2dbaa-136">Aruba</span></span>       | <span data-ttu-id="2dbaa-137">ギニアビサウ</span><span class="sxs-lookup"><span data-stu-id="2dbaa-137">Guinea-Bissau</span></span>     | <span data-ttu-id="2dbaa-138">サンマルタン島</span><span class="sxs-lookup"><span data-stu-id="2dbaa-138">Saint Martin</span></span>   |
> | <span data-ttu-id="2dbaa-139">アゼルバイジャン</span><span class="sxs-lookup"><span data-stu-id="2dbaa-139">Azerbaijan</span></span>       | <span data-ttu-id="2dbaa-140">ガイアナ</span><span class="sxs-lookup"><span data-stu-id="2dbaa-140">Guyana</span></span>     | <span data-ttu-id="2dbaa-141">サンピエール・ミクロン</span><span class="sxs-lookup"><span data-stu-id="2dbaa-141">Saint Pierre and Miquelon</span></span>   |
> | <span data-ttu-id="2dbaa-142">ベナン</span><span class="sxs-lookup"><span data-stu-id="2dbaa-142">Benin</span></span>     | <span data-ttu-id="2dbaa-143">ハイチ</span><span class="sxs-lookup"><span data-stu-id="2dbaa-143">Haiti</span></span>       | <span data-ttu-id="2dbaa-144">セントビンセントおよびグレナディーン諸島</span><span class="sxs-lookup"><span data-stu-id="2dbaa-144">Saint Vincent and the Grenadines</span></span>     |
> | <span data-ttu-id="2dbaa-145">ブータン</span><span class="sxs-lookup"><span data-stu-id="2dbaa-145">Bhutan</span></span>     | <span data-ttu-id="2dbaa-146">ハード・マクドナルド諸島</span><span class="sxs-lookup"><span data-stu-id="2dbaa-146">Heard Island and McDonald Islands</span></span>       | <span data-ttu-id="2dbaa-147">サモア</span><span class="sxs-lookup"><span data-stu-id="2dbaa-147">Samoa</span></span>     |
> | <span data-ttu-id="2dbaa-148">ボネール島</span><span class="sxs-lookup"><span data-stu-id="2dbaa-148">Bonaire</span></span>     | <span data-ttu-id="2dbaa-149">マン島</span><span class="sxs-lookup"><span data-stu-id="2dbaa-149">Isle of Man</span></span>     | <span data-ttu-id="2dbaa-150">サンマリノ</span><span class="sxs-lookup"><span data-stu-id="2dbaa-150">San Marino</span></span>     |
> | <span data-ttu-id="2dbaa-151">ブーベ島</span><span class="sxs-lookup"><span data-stu-id="2dbaa-151">Bouvet Island</span></span>     | <span data-ttu-id="2dbaa-152">ヤンマイエン島</span><span class="sxs-lookup"><span data-stu-id="2dbaa-152">Jan Mayen</span></span>     | <span data-ttu-id="2dbaa-153">サントメ・プリンシペ</span><span class="sxs-lookup"><span data-stu-id="2dbaa-153">São Tomé and Príncipe</span></span>   |
> | <span data-ttu-id="2dbaa-154">英領インド洋地域</span><span class="sxs-lookup"><span data-stu-id="2dbaa-154">British Indian Ocean Territory</span></span>       | <span data-ttu-id="2dbaa-155">ジャージー島</span><span class="sxs-lookup"><span data-stu-id="2dbaa-155">Jersey</span></span>     | <span data-ttu-id="2dbaa-156">セーシェル</span><span class="sxs-lookup"><span data-stu-id="2dbaa-156">Seychelles</span></span>   |
> | <span data-ttu-id="2dbaa-157">英領バージン諸島</span><span class="sxs-lookup"><span data-stu-id="2dbaa-157">British Virgin Islands</span></span>     | <span data-ttu-id="2dbaa-158">キリバス</span><span class="sxs-lookup"><span data-stu-id="2dbaa-158">Kiribati</span></span>       | <span data-ttu-id="2dbaa-159">シエラレオネ</span><span class="sxs-lookup"><span data-stu-id="2dbaa-159">Sierra Leone</span></span>   |
> | <span data-ttu-id="2dbaa-160">ブルキナファソ</span><span class="sxs-lookup"><span data-stu-id="2dbaa-160">Burkina Faso</span></span>     | <span data-ttu-id="2dbaa-161">コソボ</span><span class="sxs-lookup"><span data-stu-id="2dbaa-161">Kosovo</span></span>     | <span data-ttu-id="2dbaa-162">シント・ユースタティウス島</span><span class="sxs-lookup"><span data-stu-id="2dbaa-162">Sint Eustatius</span></span>     |
> | <span data-ttu-id="2dbaa-163">ブルンジ</span><span class="sxs-lookup"><span data-stu-id="2dbaa-163">Burundi</span></span>     | <span data-ttu-id="2dbaa-164">ラオス</span><span class="sxs-lookup"><span data-stu-id="2dbaa-164">Laos</span></span>     | <span data-ttu-id="2dbaa-165">シント・マールテン島</span><span class="sxs-lookup"><span data-stu-id="2dbaa-165">Sint Maarten</span></span>     |
> | <span data-ttu-id="2dbaa-166">カンボジア</span><span class="sxs-lookup"><span data-stu-id="2dbaa-166">Cambodia</span></span>     | <span data-ttu-id="2dbaa-167">レソト</span><span class="sxs-lookup"><span data-stu-id="2dbaa-167">Lesotho</span></span>     | <span data-ttu-id="2dbaa-168">ソロモン諸島</span><span class="sxs-lookup"><span data-stu-id="2dbaa-168">Solomon Islands</span></span>     |
> | <span data-ttu-id="2dbaa-169">中央アフリカ共和国</span><span class="sxs-lookup"><span data-stu-id="2dbaa-169">Central African Republic</span></span>     | <span data-ttu-id="2dbaa-170">リベリア</span><span class="sxs-lookup"><span data-stu-id="2dbaa-170">Liberia</span></span>     | <span data-ttu-id="2dbaa-171">ソマリア</span><span class="sxs-lookup"><span data-stu-id="2dbaa-171">Somalia</span></span>     |
> | <span data-ttu-id="2dbaa-172">チャド</span><span class="sxs-lookup"><span data-stu-id="2dbaa-172">Chad</span></span>     | <span data-ttu-id="2dbaa-173">マダガスカル</span><span class="sxs-lookup"><span data-stu-id="2dbaa-173">Madagascar</span></span>     | <span data-ttu-id="2dbaa-174">サウスジョージア・サウスサンドウィッチ諸島</span><span class="sxs-lookup"><span data-stu-id="2dbaa-174">South Georgia and South Sandwich Islands</span></span>     |
> | <span data-ttu-id="2dbaa-175">中国</span><span class="sxs-lookup"><span data-stu-id="2dbaa-175">China</span></span>     | <span data-ttu-id="2dbaa-176">マラウイ</span><span class="sxs-lookup"><span data-stu-id="2dbaa-176">Malawi</span></span>     | <span data-ttu-id="2dbaa-177">南スーダン</span><span class="sxs-lookup"><span data-stu-id="2dbaa-177">South Sudan</span></span>     |
> | <span data-ttu-id="2dbaa-178">クリスマス島</span><span class="sxs-lookup"><span data-stu-id="2dbaa-178">Christmas Island</span></span>     | <span data-ttu-id="2dbaa-179">モルディブ</span><span class="sxs-lookup"><span data-stu-id="2dbaa-179">Maldives</span></span>     | <span data-ttu-id="2dbaa-180">セントヘレナ、アセンションおよびトリスタンダクーニャ</span><span class="sxs-lookup"><span data-stu-id="2dbaa-180">St Helena, Ascension, Tristan da Cunha</span></span>     |
> | <span data-ttu-id="2dbaa-181">ココス諸島</span><span class="sxs-lookup"><span data-stu-id="2dbaa-181">Cocos (Keeling) Islands</span></span>     | <span data-ttu-id="2dbaa-182">マリ</span><span class="sxs-lookup"><span data-stu-id="2dbaa-182">Mali</span></span>     | <span data-ttu-id="2dbaa-183">スリナム</span><span class="sxs-lookup"><span data-stu-id="2dbaa-183">Suriname</span></span>     |
> | <span data-ttu-id="2dbaa-184">コモロ</span><span class="sxs-lookup"><span data-stu-id="2dbaa-184">Comoros</span></span>     | <span data-ttu-id="2dbaa-185">マーシャル諸島</span><span class="sxs-lookup"><span data-stu-id="2dbaa-185">Marshall Islands</span></span>     | <span data-ttu-id="2dbaa-186">スバールバル諸島</span><span class="sxs-lookup"><span data-stu-id="2dbaa-186">Svalbard</span></span>     |
> | <span data-ttu-id="2dbaa-187">コンゴ共和国</span><span class="sxs-lookup"><span data-stu-id="2dbaa-187">Congo</span></span>     | <span data-ttu-id="2dbaa-188">マルチニーク島</span><span class="sxs-lookup"><span data-stu-id="2dbaa-188">Martinique</span></span>     | <span data-ttu-id="2dbaa-189">スワジランド</span><span class="sxs-lookup"><span data-stu-id="2dbaa-189">Swaziland</span></span>     |
> | <span data-ttu-id="2dbaa-190">コンゴ民主共和国</span><span class="sxs-lookup"><span data-stu-id="2dbaa-190">Congo (DRC)</span></span>     | <span data-ttu-id="2dbaa-191">モーリタニア</span><span class="sxs-lookup"><span data-stu-id="2dbaa-191">Mauritania</span></span>     | <span data-ttu-id="2dbaa-192">ティモール・レステ</span><span class="sxs-lookup"><span data-stu-id="2dbaa-192">Timor-Leste</span></span>   |
> | <span data-ttu-id="2dbaa-193">クック諸島</span><span class="sxs-lookup"><span data-stu-id="2dbaa-193">Cook Islands</span></span>     | <span data-ttu-id="2dbaa-194">マイヨット島</span><span class="sxs-lookup"><span data-stu-id="2dbaa-194">Mayotte</span></span>     | <span data-ttu-id="2dbaa-195">トーゴ</span><span class="sxs-lookup"><span data-stu-id="2dbaa-195">Togo</span></span>   |
> | <span data-ttu-id="2dbaa-196">ジブチ</span><span class="sxs-lookup"><span data-stu-id="2dbaa-196">Djibouti</span></span>     | <span data-ttu-id="2dbaa-197">ミクロネシア</span><span class="sxs-lookup"><span data-stu-id="2dbaa-197">Micronesia</span></span>     | <span data-ttu-id="2dbaa-198">トケラウ諸島</span><span class="sxs-lookup"><span data-stu-id="2dbaa-198">Tokelau</span></span>   |
> | <span data-ttu-id="2dbaa-199">ドミニカ国</span><span class="sxs-lookup"><span data-stu-id="2dbaa-199">Dominica</span></span>     | <span data-ttu-id="2dbaa-200">モンセラット</span><span class="sxs-lookup"><span data-stu-id="2dbaa-200">Montserrat</span></span>     | <span data-ttu-id="2dbaa-201">トンガ</span><span class="sxs-lookup"><span data-stu-id="2dbaa-201">Tonga</span></span>   |
> | <span data-ttu-id="2dbaa-202">赤道ギニア</span><span class="sxs-lookup"><span data-stu-id="2dbaa-202">Equatorial Guinea</span></span>     | <span data-ttu-id="2dbaa-203">モザンビーク</span><span class="sxs-lookup"><span data-stu-id="2dbaa-203">Mozambique</span></span>     | <span data-ttu-id="2dbaa-204">タークス・カイコス諸島</span><span class="sxs-lookup"><span data-stu-id="2dbaa-204">Turks and Caicos Islands</span></span>   |
> | <span data-ttu-id="2dbaa-205">エリトリア</span><span class="sxs-lookup"><span data-stu-id="2dbaa-205">Eritrea</span></span>     | <span data-ttu-id="2dbaa-206">ミャンマー</span><span class="sxs-lookup"><span data-stu-id="2dbaa-206">Myanmar</span></span>     | <span data-ttu-id="2dbaa-207">ツバル</span><span class="sxs-lookup"><span data-stu-id="2dbaa-207">Tuvalu</span></span>   |
> | <span data-ttu-id="2dbaa-208">フォークランド諸島</span><span class="sxs-lookup"><span data-stu-id="2dbaa-208">Falkland Islands</span></span>     | <span data-ttu-id="2dbaa-209">ナウル</span><span class="sxs-lookup"><span data-stu-id="2dbaa-209">Nauru</span></span>     | <span data-ttu-id="2dbaa-210">米領小離島</span><span class="sxs-lookup"><span data-stu-id="2dbaa-210">U.S. Outlying Islands</span></span>   |
> | <span data-ttu-id="2dbaa-211">フランス領ギアナ</span><span class="sxs-lookup"><span data-stu-id="2dbaa-211">French Guiana</span></span>     | <span data-ttu-id="2dbaa-212">ニューカレドニア</span><span class="sxs-lookup"><span data-stu-id="2dbaa-212">New Caledonia</span></span>     | <span data-ttu-id="2dbaa-213">バヌアツ</span><span class="sxs-lookup"><span data-stu-id="2dbaa-213">Vanuatu</span></span>   |
> | <span data-ttu-id="2dbaa-214">フランス領ポリネシア</span><span class="sxs-lookup"><span data-stu-id="2dbaa-214">French Polynesia</span></span>     | <span data-ttu-id="2dbaa-215">ニジェール</span><span class="sxs-lookup"><span data-stu-id="2dbaa-215">Niger</span></span>     | <span data-ttu-id="2dbaa-216">バチカン市国</span><span class="sxs-lookup"><span data-stu-id="2dbaa-216">Vatican City</span></span>   |
> | <span data-ttu-id="2dbaa-217">仏領極南諸島</span><span class="sxs-lookup"><span data-stu-id="2dbaa-217">French Southern Territories</span></span>     | <span data-ttu-id="2dbaa-218">ニウエ</span><span class="sxs-lookup"><span data-stu-id="2dbaa-218">Niue</span></span>     | <span data-ttu-id="2dbaa-219">ワリス・フテュナ諸島</span><span class="sxs-lookup"><span data-stu-id="2dbaa-219">Wallis and Futuna</span></span>   |
> | <span data-ttu-id="2dbaa-220">ガボン</span><span class="sxs-lookup"><span data-stu-id="2dbaa-220">Gabon</span></span>     | <span data-ttu-id="2dbaa-221">ノーフォーク島</span><span class="sxs-lookup"><span data-stu-id="2dbaa-221">Norfolk Island</span></span>     | <span data-ttu-id="2dbaa-222">イエメン</span><span class="sxs-lookup"><span data-stu-id="2dbaa-222">Yemen</span></span>   |
> | <span data-ttu-id="2dbaa-223">ガンビア</span><span class="sxs-lookup"><span data-stu-id="2dbaa-223">Gambia</span></span>     | <span data-ttu-id="2dbaa-224">北マリアナ諸島</span><span class="sxs-lookup"><span data-stu-id="2dbaa-224">Northern Mariana Islands</span></span>     |    |
> | <span data-ttu-id="2dbaa-225">ジブラルタル</span><span class="sxs-lookup"><span data-stu-id="2dbaa-225">Gibraltar</span></span>     | <span data-ttu-id="2dbaa-226">パラオ</span><span class="sxs-lookup"><span data-stu-id="2dbaa-226">Palau</span></span>       |    |

## <a name="buy-software-subscriptions-on-behalf-of-customers"></a><span data-ttu-id="2dbaa-227">顧客に代わってソフトウェア サブスクリプションを購入する</span><span class="sxs-lookup"><span data-stu-id="2dbaa-227">Buy software subscriptions on behalf of customers</span></span>

<span data-ttu-id="2dbaa-228">顧客に代わってソフトウェア サブスクリプションを購入するには、次の操作を行います。</span><span class="sxs-lookup"><span data-stu-id="2dbaa-228">To buy software subscriptions on behalf of a customer:</span></span>

1. <span data-ttu-id="2dbaa-229">パートナー センター [ダッシュボード](https://partner.microsoft.com/dashboard)にサインインします。</span><span class="sxs-lookup"><span data-stu-id="2dbaa-229">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="2dbaa-230">パートナー センター メニューから **[顧客]** を選択し、一覧から顧客を選びます。</span><span class="sxs-lookup"><span data-stu-id="2dbaa-230">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

3. <span data-ttu-id="2dbaa-231">顧客の詳細ページから、 **[製品の追加]** を選択した後、画面の指示に従って注文を作成して支払います。</span><span class="sxs-lookup"><span data-stu-id="2dbaa-231">From the customer's detail page, select **Add products**, and then follow the on-screen instructions to create and pay for your order.</span></span> <span data-ttu-id="2dbaa-232">オーストラリアとブラジルを除き、すべての商用顧客向け価格には税は含まれません。</span><span class="sxs-lookup"><span data-stu-id="2dbaa-232">All commercial pricing excludes tax with the exception of Australia and Brazil.</span></span> <span data-ttu-id="2dbaa-233">オーストラリアとブラジルの場合は、価格に税が含まれています。</span><span class="sxs-lookup"><span data-stu-id="2dbaa-233">For Australia and Brazil, the price includes tax.</span></span>

## <a name="activate-and-manage-software-subscriptions"></a><span data-ttu-id="2dbaa-234">ソフトウェア サブスクリプションのライセンス認証と管理</span><span class="sxs-lookup"><span data-stu-id="2dbaa-234">Activate and manage software subscriptions</span></span>

<span data-ttu-id="2dbaa-235">ソフトウェアを購入した後、パートナーおよびお客様はソフトウェアをダウンロードする必要があります (パートナー センターを利用しているパートナー、Microsoft 365 管理センターを利用しているお客様)。</span><span class="sxs-lookup"><span data-stu-id="2dbaa-235">Once you've purchased your software, you or your customers need to download it (partners using Partner Center; customers using the Microsoft 365 Admin Center).</span></span> <span data-ttu-id="2dbaa-236">この場合、次の手順を実行します。</span><span class="sxs-lookup"><span data-stu-id="2dbaa-236">Use the following procedure to do this.</span></span> <span data-ttu-id="2dbaa-237">リンクのコピーとソフトウェアのダウンロードに関連するリスクを理解することが重要です。</span><span class="sxs-lookup"><span data-stu-id="2dbaa-237">It’s important to understand the risks associated with copying links and downloading software.</span></span> <span data-ttu-id="2dbaa-238">詳しくは、[Partner Center New Commerce Operations Guide](https://partner.microsoft.com/resources/detail/partner-center-new-commerce-operations-guide-pdf) の **パートナー センターを使用してカスタマー ソフトウェアのダウンロードとライセンス キーを取得する方法** に関するページを参照してください。</span><span class="sxs-lookup"><span data-stu-id="2dbaa-238">For more information, see **Using Partner Center to obtain customer software downloads and license keys** in the [Partner Center New Commerce Operations Guide](https://partner.microsoft.com/resources/detail/partner-center-new-commerce-operations-guide-pdf).</span></span>

>[!NOTE]
><span data-ttu-id="2dbaa-239">キーとダウンロードへのリンクを取得するには、パートナー センターの管理エージェントである必要があります。</span><span class="sxs-lookup"><span data-stu-id="2dbaa-239">You must be an Admin agent in Partner Center to obtain the link to keys and downloads.</span></span>

1. <span data-ttu-id="2dbaa-240">顧客の詳細ページに移動し、 **[ソフトウェア]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="2dbaa-240">Go to your customer's detail page, and then select **Software**.</span></span> <span data-ttu-id="2dbaa-241">顧客に代わって購入したすべてのソフトウェアの一覧が表示されます。</span><span class="sxs-lookup"><span data-stu-id="2dbaa-241">You'll see a list of all the software you've purchased on behalf of the customer.</span></span>

2. <span data-ttu-id="2dbaa-242">製品の **バージョン**、**言語**、**ビット** を選択し、 **[キーとダウンロードの取得]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="2dbaa-242">Choose product **version**, **language**, **bit**, and select **Get keys and downloads**.</span></span> 

3. <span data-ttu-id="2dbaa-243">**[キーの取得]** を選択すると、ポップアップ ダイアログ ボックスに 32 桁の生成結果が表示され、コピーして顧客に送信することができます。</span><span class="sxs-lookup"><span data-stu-id="2dbaa-243">Choose **Get Key** to display the 32-digit product in a pop-up dialog box which you can copy and send to the customer.</span></span> 

4. <span data-ttu-id="2dbaa-244">**[ダウンロード]** を選択してビットをダウンロードします。</span><span class="sxs-lookup"><span data-stu-id="2dbaa-244">Choose **Download** to download the bits.</span></span> 

5. <span data-ttu-id="2dbaa-245">ビットのダウンロードへのリンクを顧客に送信する場合は、 **[リンクのコピー]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="2dbaa-245">Choose **Copy Link** if you want to send the customer the link to the bits download.</span></span> 

6. <span data-ttu-id="2dbaa-246">また、ソフトウェアの注文を **キャンセル** し、100% のクレジットを受け取ることもできます (60 日のキャンセル ポリシー期間内に行った場合)。</span><span class="sxs-lookup"><span data-stu-id="2dbaa-246">You can also **Cancel** the software order and receive 100% credit (if done within the 60 days cancellation policy period).</span></span>

>[!NOTE]
><span data-ttu-id="2dbaa-247">Microsoft 365 管理センターでプロダクト キーを参照し、情報をダウンロードするためのアクセス権があるのは、顧客だけです (グローバル管理者ロールが必要)。</span><span class="sxs-lookup"><span data-stu-id="2dbaa-247">Only customers have access to see the product keys and download information in the Microsoft 365 Admin Center (Global Admin role required).</span></span> <span data-ttu-id="2dbaa-248">パートナーがこの情報を確認するには、パートナー センターを使用する必要があります。</span><span class="sxs-lookup"><span data-stu-id="2dbaa-248">Partners must use Partner Center to see this information.</span></span>

## <a name="server-subscription-download-and-license-keys-available-through-microsoft-365-admin-center-for-customers"></a><span data-ttu-id="2dbaa-249">Microsoft 365 管理センターで顧客向けに使用できるサーバー サブスクリプションのダウンロードとライセンス キー</span><span class="sxs-lookup"><span data-stu-id="2dbaa-249">Server subscription download and license keys available through Microsoft 365 Admin Center for customers</span></span> 

<span data-ttu-id="2dbaa-250">顧客は CSP サーバー サブスクリプションのライセンス キーとダウンロードを Microsoft 365 管理センターから入手できます。</span><span class="sxs-lookup"><span data-stu-id="2dbaa-250">Your customers will be able to get CSP server subscription license keys and downloads from Microsoft 365 Admin Center.</span></span> <span data-ttu-id="2dbaa-251">CSP サーバー サブスクリプションのライセンス キーとダウンロードを確認するには、顧客は、Microsoft 365 管理センターにアクセスして、 **[請求] > 自分の製品 > [ソフトウェア] タブ** に移動する必要があります。詳細については、[[請求] の下の [ソフトウェア] タブ](/microsoft-365/admin/whats-new-in-preview#billing--subscriptions)をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="2dbaa-251">To see their CSP server subscription license keys and downloads, customer must go to Microsoft 365 Admin Center > **Billing > Your products > Software tab**. For more details, see [Software Tab under Billing](/microsoft-365/admin/whats-new-in-preview#billing--subscriptions).</span></span>  

## <a name="view-activity-for-software-key-access-and-software-downloads"></a><span data-ttu-id="2dbaa-252">ソフトウェア キーへのアクセスとソフトウェアのダウンロードに関するアクティビティを表示する</span><span class="sxs-lookup"><span data-stu-id="2dbaa-252">View activity for software key access and software downloads</span></span>

<span data-ttu-id="2dbaa-253">監査またはコンプライアンスの目的で、サーバー サブスクリプションのソフトウェア キーにアクセスしたか、サーバー サブスクリプション ソフトウェアをダウンロードしたユーザーの一覧を確認することが必要な場合があります。</span><span class="sxs-lookup"><span data-stu-id="2dbaa-253">For auditing or compliance purposes, you may need to check a list of users who have either accessed Server subscription software keys or downloaded Server subscription software.</span></span> <span data-ttu-id="2dbaa-254">この情報にアクセスするには、以下の手順を実行します。</span><span class="sxs-lookup"><span data-stu-id="2dbaa-254">Use the procedure below to access this information.</span></span> 

>[!NOTE]
><span data-ttu-id="2dbaa-255">これらのアクティビティ ログを表示するには、グローバル管理者、アカウント管理者、紹介管理者、またはマーケティング コンテンツ管理者になる必要があります。</span><span class="sxs-lookup"><span data-stu-id="2dbaa-255">You must be a Global administrator, Account admin, Referral admin, or Marketing content admin to see these activity logs.</span></span> 

1. <span data-ttu-id="2dbaa-256">パートナー センター [ダッシュボード](https://partner.microsoft.com/dashboard)にサインインします。</span><span class="sxs-lookup"><span data-stu-id="2dbaa-256">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="2dbaa-257">右上隅にある歯車アイコンを選択します。</span><span class="sxs-lookup"><span data-stu-id="2dbaa-257">Select the gear icon from the upper right corner.</span></span>

3. <span data-ttu-id="2dbaa-258">メニューで、 **[アクティビティ ログ]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="2dbaa-258">In the menu, select **Activity log**.</span></span>

4. <span data-ttu-id="2dbaa-259">表示するアクティビティの日付範囲を入力します。</span><span class="sxs-lookup"><span data-stu-id="2dbaa-259">Enter the date range for the activity you want to see.</span></span> <span data-ttu-id="2dbaa-260">アクティビティ ログに、指定した期間にソフトウェア キーにアクセスしたか、ソフトウェアをダウンロードしたユーザーの一覧が表示されます。</span><span class="sxs-lookup"><span data-stu-id="2dbaa-260">The activity log will display a list of users who have either accessed software keys or downloaded software during the time you specified.</span></span> 

## <a name="cancel-a-purchase"></a><span data-ttu-id="2dbaa-261">購入を取り消す</span><span class="sxs-lookup"><span data-stu-id="2dbaa-261">Cancel a purchase</span></span>

<span data-ttu-id="2dbaa-262">購入日から 60 日以内であればソフトウェア購入を取り消すことができます。</span><span class="sxs-lookup"><span data-stu-id="2dbaa-262">You can cancel a software purchase within 60 days of the purchase date.</span></span> <span data-ttu-id="2dbaa-263">この最初の 60 日以内に取り消した場合は、中途解約料がかかりません。</span><span class="sxs-lookup"><span data-stu-id="2dbaa-263">If you cancel within this first 60-day period, you will not be charged an early termination fee.</span></span> <span data-ttu-id="2dbaa-264">60 日を過ぎると、購入の取り消しができなくなります</span><span class="sxs-lookup"><span data-stu-id="2dbaa-264">After 60 days, you can no longer cancel a purchase.</span></span> <span data-ttu-id="2dbaa-265">(この取り消し規則の主な制限については、「注意」をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="2dbaa-265">(See Note for key restrictions to this cancellation rule.</span></span> <span data-ttu-id="2dbaa-266">ソフトウェアの購入を取り消した後の処理については、これらの手順の後にある「重要」もご覧ください。)</span><span class="sxs-lookup"><span data-stu-id="2dbaa-266">To learn about what happens after you cancel a software purchase, see also Important note after these steps.)</span></span> 

>[!NOTE]
><span data-ttu-id="2dbaa-267">購入を取り消すための次の手順は、購入後の最初の 60 日以内など、特定の取り消し期間内に取り消しの対象となったソフトウェアにのみ適用されます。</span><span class="sxs-lookup"><span data-stu-id="2dbaa-267">The following steps to cancel a purchase apply only to software that qualifies for cancellation within a specific cancellation window, such as within the first 60 days after purchase.</span></span> <span data-ttu-id="2dbaa-268">また、これらの手順は、Azure の SUSE Linux または RedHat ソフトウェア プランには適用されません。</span><span class="sxs-lookup"><span data-stu-id="2dbaa-268">These steps also do not apply to a SUSE Linux or RedHat software plan in Azure.</span></span> <span data-ttu-id="2dbaa-269">現時点では、SUSE または RedHat ソフトウェア プランのキャンセルや交換はできません。</span><span class="sxs-lookup"><span data-stu-id="2dbaa-269">At this time, you cannot cancel or exchange a SUSE or RedHat software plan.</span></span> <span data-ttu-id="2dbaa-270">SUSE Linux または RedHat プランの使用方法について詳しくは、[こちらをご覧ください](/azure/virtual-machines/linux/prepay-suse-software-charges)。</span><span class="sxs-lookup"><span data-stu-id="2dbaa-270">[Learn more](/azure/virtual-machines/linux/prepay-suse-software-charges) about using SUSE Linux or RedHat plans.</span></span>

<span data-ttu-id="2dbaa-271">購入をキャンセルするには、次の手順に従います。</span><span class="sxs-lookup"><span data-stu-id="2dbaa-271">Follow the steps below to cancel a purchase:</span></span>

>[!NOTE]
><span data-ttu-id="2dbaa-272">購入を取り消すには、管理エージェントである必要があります。</span><span class="sxs-lookup"><span data-stu-id="2dbaa-272">You must be an Admin agent to cancel a purchase.</span></span> <span data-ttu-id="2dbaa-273">次の手順では、パートナー センター ダッシュボードで購入を取り消す方法について説明します。</span><span class="sxs-lookup"><span data-stu-id="2dbaa-273">The following steps describe how to cancel a purchase in the Partner Center dashboard.</span></span> <span data-ttu-id="2dbaa-274">この操作は、[パートナー センター API](/partner-center/develop/cancel-software-purchases) を使用して行うこともできます。</span><span class="sxs-lookup"><span data-stu-id="2dbaa-274">You can also do this using the [Partner Center API](/partner-center/develop/cancel-software-purchases).</span></span>

1. <span data-ttu-id="2dbaa-275">取り消しプロセスを開始する前に、次のものが揃っていることを確認してください。</span><span class="sxs-lookup"><span data-stu-id="2dbaa-275">Before you start the cancellation process, make sure you have the following:</span></span>

    - <span data-ttu-id="2dbaa-276">顧客の名前、テナント GUID、またはドメイン名</span><span class="sxs-lookup"><span data-stu-id="2dbaa-276">The customer's name, tenant GUID, or domain name</span></span>

    - <span data-ttu-id="2dbaa-277">取り消す製品の名称</span><span class="sxs-lookup"><span data-stu-id="2dbaa-277">The name of the product you want to cancel</span></span>
    
    - <span data-ttu-id="2dbaa-278">注文 ID</span><span class="sxs-lookup"><span data-stu-id="2dbaa-278">The Order ID</span></span>

2. <span data-ttu-id="2dbaa-279">パートナー センター [ダッシュボード](https://partner.microsoft.com/dashboard)にサインインします。</span><span class="sxs-lookup"><span data-stu-id="2dbaa-279">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

3. <span data-ttu-id="2dbaa-280">パートナー センター メニューから **[顧客]** を選択し、一覧から顧客を選びます。</span><span class="sxs-lookup"><span data-stu-id="2dbaa-280">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

4. <span data-ttu-id="2dbaa-281">顧客の詳細ページで、 **[ソフトウェア]** を選択して、顧客用に購入したソフトウェアの一覧を表示します。</span><span class="sxs-lookup"><span data-stu-id="2dbaa-281">On the customer's details page, select **Software** to see the list of software purchased for the customer.</span></span> 

5. <span data-ttu-id="2dbaa-282">取り消すソフトウェアの購入を見つけて、 **[キャンセル]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="2dbaa-282">Locate the software purchase you want to cancel, and then select **Cancel**.</span></span> <span data-ttu-id="2dbaa-283">ダイアログ ボックスが表示されます。</span><span class="sxs-lookup"><span data-stu-id="2dbaa-283">A dialog box will appear.</span></span>

6. <span data-ttu-id="2dbaa-284">注文番号のドロップダウン リストから、取り消し対象の正しい注文 ID 番号を選択します</span><span class="sxs-lookup"><span data-stu-id="2dbaa-284">From the Order number drop-down list, select the correct order ID number you want to cancel.</span></span> <span data-ttu-id="2dbaa-285">(注文または注文 ID 番号について詳しくは、顧客の **注文履歴** ページをご覧ください)。</span><span class="sxs-lookup"><span data-stu-id="2dbaa-285">(You can learn more information about an order or order ID number from the customer's **Order history** page.)</span></span>

7. <span data-ttu-id="2dbaa-286">取り消しに関する **重要な** メッセージに目を通したことを確認するためのチェックボックスをオンにします</span><span class="sxs-lookup"><span data-stu-id="2dbaa-286">Select the checkbox to acknowledge that you have read the **Important** message concerning cancellation.</span></span> <span data-ttu-id="2dbaa-287">(購入を取り消した後の処理については、以下の「**重要**」をご覧ください)。</span><span class="sxs-lookup"><span data-stu-id="2dbaa-287">(Refer to the **Important** note below to learn more about what happens after you cancel a purchase.)</span></span>

8. <span data-ttu-id="2dbaa-288">**[送信]** を選択して購入を取り消します。</span><span class="sxs-lookup"><span data-stu-id="2dbaa-288">Select **Submit** to cancel your purchase.</span></span> <span data-ttu-id="2dbaa-289">顧客の複数の注文を取り消す場合は、一意の注文 ID 番号ごとに手順 4 ～ 6 を繰り返す必要があります。</span><span class="sxs-lookup"><span data-stu-id="2dbaa-289">If you want to cancel multiple orders for a customer, you will need to perform Steps 4 through 6 again for each, unique order ID number.</span></span>

<span data-ttu-id="2dbaa-290">注文の取り消しを試みると、パートナー センターから他の情報が送られてくることもあります (注文番号のドロップダウン リストの下に表示されます)。</span><span class="sxs-lookup"><span data-stu-id="2dbaa-290">When you attempt to cancel an order, Partner Center may also give you other information (that appears below the Order number drop-down list).</span></span> <span data-ttu-id="2dbaa-291">この情報には次の項目が含まれていることがあります。</span><span class="sxs-lookup"><span data-stu-id="2dbaa-291">This information can include:</span></span>

- <span data-ttu-id="2dbaa-292">その注文の取り消しが可能な残り日数</span><span class="sxs-lookup"><span data-stu-id="2dbaa-292">How many days remain for you to cancel that particular order</span></span>

- <span data-ttu-id="2dbaa-293">取り消し期間を既に過ぎていて注文の取り消しができなくなっているかどうか</span><span class="sxs-lookup"><span data-stu-id="2dbaa-293">Whether you have already passed the cancellation window and can no longer cancel the order</span></span>

- <span data-ttu-id="2dbaa-294">Microsoft で取り消し要求に関する情報がさらに必要な場合、**カスタマー サポート要求** フォームへのリンクが表示されることがあります。</span><span class="sxs-lookup"><span data-stu-id="2dbaa-294">If we need more information about your cancellation request, you may be given a link to a **customer support request** form.</span></span>

>[!IMPORTANT]
><span data-ttu-id="2dbaa-295">注文の取り消しが終わると、取り消しを確認するメッセージが表示されます。</span><span class="sxs-lookup"><span data-stu-id="2dbaa-295">After you cancel an order, a message confirming your cancellation will appear.</span></span> <span data-ttu-id="2dbaa-296">ただし、取り消しがパートナー センター ダッシュボードに表示されるまで、最大 15 分の遅延が発生する場合があります。</span><span class="sxs-lookup"><span data-stu-id="2dbaa-296">There may be a delay of up to 15 minutes, however, before the cancellation appears on the Partner Center dashboard.</span></span> 

### <a name="post-cancellation-details"></a><span data-ttu-id="2dbaa-297">取り消した後の詳細</span><span class="sxs-lookup"><span data-stu-id="2dbaa-297">Post-cancellation details</span></span>

<span data-ttu-id="2dbaa-298">購入を取り消した後は、次のようになります。</span><span class="sxs-lookup"><span data-stu-id="2dbaa-298">After you cancel a purchase:</span></span>

- <span data-ttu-id="2dbaa-299">関連するソフトウェア キーとダウンロード リンクがすべて失効します。</span><span class="sxs-lookup"><span data-stu-id="2dbaa-299">All related software keys and download links will be revoked.</span></span> <span data-ttu-id="2dbaa-300">つまり、パートナーとパートナーの顧客はこの購入に関連するソフトウェア キーとダウンロード リンクを使用できなくなります。</span><span class="sxs-lookup"><span data-stu-id="2dbaa-300">This means neither you nor your customer can use the software keys and download links any longer related to this purchase.</span></span> <span data-ttu-id="2dbaa-301">パートナーとパートナーの顧客は、取り消されたすべてのソフトウェアの使用を中止しなければなりません。</span><span class="sxs-lookup"><span data-stu-id="2dbaa-301">You and your customer are responsible for discontinuing the use of all canceled software.</span></span> <span data-ttu-id="2dbaa-302">さらに、取り消されたソフトウェアをアンインストールし、関連するソフトウェアのダウンロードやリンクもすべて削除しなければなりません。</span><span class="sxs-lookup"><span data-stu-id="2dbaa-302">You are also responsible for uninstalling the canceled software and removing any, related software downloads and links.</span></span>

- <span data-ttu-id="2dbaa-303">取り消された項目は顧客のソフトウェアの詳細ページに引き続き表示されますが、アクティブ化キーは利用できなくなります。</span><span class="sxs-lookup"><span data-stu-id="2dbaa-303">The canceled item will still appear on the customer's Software details page but the activation key will not be available.</span></span>

- <span data-ttu-id="2dbaa-304">次回の月次請求書には、取り消された注文の返金額が表示されます。</span><span class="sxs-lookup"><span data-stu-id="2dbaa-304">A credit for the canceled order will appear on your next monthly invoice.</span></span> <span data-ttu-id="2dbaa-305">永続的ソフトウェアの場合は全額返金され、ソフトウェア サブスクリプションの場合は日割り計算で返金されます。</span><span class="sxs-lookup"><span data-stu-id="2dbaa-305">Perpetual software will receive a 100% credit and software subscriptions will receive a prorated credit.</span></span>

### <a name="submit-a-customer-support-request-to-cancel-a-purchase"></a><span data-ttu-id="2dbaa-306">購入を取り消すためのカスタマー サポート要求を送信する</span><span class="sxs-lookup"><span data-stu-id="2dbaa-306">Submit a customer support request to cancel a purchase</span></span>

<span data-ttu-id="2dbaa-307">パートナー センターからソフトウェアの購入の取り消しを試みたが、詳細な情報の提供と、カスタマー サポート要求フォームへの記入を指示された場合は、次の手順が役立つことがあります。</span><span class="sxs-lookup"><span data-stu-id="2dbaa-307">If you tried to cancel a software purchase via Partner Center but were told to provide more information and fill out a customer support request form, these steps may help you:</span></span>

1. <span data-ttu-id="2dbaa-308">[購入を取り消す] ウィンドウから **[customer support request]\(カスタマー サポート要求\)** リンクを選択すると、 **[パートナー センターに関する問題を報告する]** ページが開きます。</span><span class="sxs-lookup"><span data-stu-id="2dbaa-308">When you select the **customer support request** link from the Cancel purchase window, the **Report a problem with Partner Center** page will open.</span></span>

2. <span data-ttu-id="2dbaa-309">**[詳細]** の [問題の種類] の一覧で、 **[お客様に代わって CSP を購入/払い戻し]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="2dbaa-309">Under **Details**, in the Type of problem list, select **CSP Purchase/Refund on behalf of customers**.</span></span>

3. <span data-ttu-id="2dbaa-310">[影響] および [タイトル] フィールドに入力します。</span><span class="sxs-lookup"><span data-stu-id="2dbaa-310">Fill in the Impact and Title fields.</span></span>

4. <span data-ttu-id="2dbaa-311">[説明] フィールドに、次の情報を入力します。</span><span class="sxs-lookup"><span data-stu-id="2dbaa-311">In the Description field, provide the following:</span></span>

    - <span data-ttu-id="2dbaa-312">顧客のテナント GUID またはドメイン名</span><span class="sxs-lookup"><span data-stu-id="2dbaa-312">The customer tenant GUID or domain name</span></span>
    
    - <span data-ttu-id="2dbaa-313">注文 ID またはサブスクリプション ID</span><span class="sxs-lookup"><span data-stu-id="2dbaa-313">Order ID or Subscription ID</span></span>
    
    - <span data-ttu-id="2dbaa-314">払い戻し理由</span><span class="sxs-lookup"><span data-stu-id="2dbaa-314">Refund reason</span></span>

    - <span data-ttu-id="2dbaa-315">要求された数量</span><span class="sxs-lookup"><span data-stu-id="2dbaa-315">Amount requested</span></span>

5. <span data-ttu-id="2dbaa-316">[連絡先] フィールドに、パートナーの名前、メール アドレス、電話番号を入力します。</span><span class="sxs-lookup"><span data-stu-id="2dbaa-316">In the Contact field, enter your name, email address, and phone number.</span></span>

6. <span data-ttu-id="2dbaa-317">何らかの理由でファイルを添付する必要がある場合は、 **[ファイルの追加]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="2dbaa-317">If you need to attach a file for any reason, select **Add files**.</span></span> <span data-ttu-id="2dbaa-318">この手順は省略可能です。</span><span class="sxs-lookup"><span data-stu-id="2dbaa-318">This step is optional.</span></span>

7. <span data-ttu-id="2dbaa-319">終了したら、 **[送信]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="2dbaa-319">When you're finished, select **Submit**.</span></span>

## <a name="next-steps"></a><span data-ttu-id="2dbaa-320">次の手順</span><span class="sxs-lookup"><span data-stu-id="2dbaa-320">Next steps</span></span>

- [<span data-ttu-id="2dbaa-321">パートナー センターを使用して、コマーシャル マーケットプレース製品のサブスクリプションを顧客に販売する</span><span class="sxs-lookup"><span data-stu-id="2dbaa-321">Use Partner Center to sell customers subscriptions to commercial marketplace products</span></span>](sell-marketplace-products.md)
 
- [<span data-ttu-id="2dbaa-322">パートナー センターで顧客に Azure サブスクリプションを割り当てる</span><span class="sxs-lookup"><span data-stu-id="2dbaa-322">Assigning Azure subscriptions to customers in Partner Center</span></span>](assign-azure-subscriptions.md)