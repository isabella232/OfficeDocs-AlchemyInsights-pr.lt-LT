---
title: Perkėlimas iš AIP į MIP / vieningą žymą atitikties centre
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002278"
- "5114"
ms.openlocfilehash: 12f5f5c46edd7918618c55a8a1905f3b28643092
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 04/15/2021
ms.locfileid: "51825379"
---
# <a name="migration-from-aip-to-mipunified-labeling-in-the-compliance-center"></a><span data-ttu-id="d0ac3-102">Perkėlimas iš AIP į MIP / vieningą žymą atitikties centre</span><span class="sxs-lookup"><span data-stu-id="d0ac3-102">Migration from AIP to MIP/Unified Labeling in the Compliance Center</span></span>

<span data-ttu-id="d0ac3-103">Norėdami pereiti iš AIP etikečių į vieningąją žymą saugos ir atitikties centre, atlikite šiuos veiksmus:</span><span class="sxs-lookup"><span data-stu-id="d0ac3-103">To migrate from AIP labels to Unified Labeling in the Security and Compliance center, do the following:</span></span>

<span data-ttu-id="d0ac3-104">**Apsaugos aktyvinimas "Azure" portale**</span><span class="sxs-lookup"><span data-stu-id="d0ac3-104">**Activate protection from the Azure portal**</span></span>

1. <span data-ttu-id="d0ac3-105">Jei to dar nepadarėte, atidarykite naują naršyklės langą ir prisijunkite [prie "Azure" portalo](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#signing-in-to-the-azure-portal).</span><span class="sxs-lookup"><span data-stu-id="d0ac3-105">If you haven't already done so, open a new browser window and [sign in to the Azure portal](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#signing-in-to-the-azure-portal).</span></span> <span data-ttu-id="d0ac3-106">Eikite į **"Azure" informacijos apsaugos ašmenį.**</span><span class="sxs-lookup"><span data-stu-id="d0ac3-106">Navigate to the **Azure Information Protection** blade.</span></span> <span data-ttu-id="d0ac3-107">Pvz., koncentratoriaus meniu spustelėkite **Visos tarnybos** ir pradėkite **vesti informaciją** lauke Filtras.</span><span class="sxs-lookup"><span data-stu-id="d0ac3-107">For example, on the hub menu, click **All services** and start typing **Information** in the Filter box.</span></span> <span data-ttu-id="d0ac3-108">Pasirinkite **"Azure" informacijos apsauga**.</span><span class="sxs-lookup"><span data-stu-id="d0ac3-108">Select **Azure Information Protection**.</span></span> <span data-ttu-id="d0ac3-109">Jei anksčiau nepriėjote prie "Azure" informacijos apsaugos ašmenų, žr. vienkartinę papildomą šio disko pridėjimo į portalą veiksmus. [](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#to-access-the-azure-information-protection-blade-for-the-first-time)</span><span class="sxs-lookup"><span data-stu-id="d0ac3-109">If you haven't accessed the Azure Information Protection blade before, see the one-time [additional steps](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#to-access-the-azure-information-protection-blade-for-the-first-time) to add this blade to the portal.</span></span> <span data-ttu-id="d0ac3-110">Norėdami atidaryti "Azure" informacijos apsaugos ašmenį, turite turėti ["Azure Information Protection Premium" planą](https://www.microsoft.com/cloud-platform/azure-information-protection-pricing) arba "Office 365" planą, kuriame yra teisių valdymas.</span><span class="sxs-lookup"><span data-stu-id="d0ac3-110">To open the Azure Information Protection blade, you must have either an [Azure Information Protection Premium plan](https://www.microsoft.com/cloud-platform/azure-information-protection-pricing) or an Office 365 plan that includes Rights Management.</span></span> <span data-ttu-id="d0ac3-111">Jei turite vieną iš šių prenumeratų, bet matote pranešimą, kad negalima rasti galiojančios prenumeratos, kreipkitės į ["Microsoft" palaikymo](https://docs.microsoft.com/azure/information-protection/get-started/information-support#to-contact-microsoft-support) tarnybą arba naudokite standartinius palaikymo kanalus.</span><span class="sxs-lookup"><span data-stu-id="d0ac3-111">If you have one of these subscriptions but see a message that a valid subscription cannot be found, [contact Microsoft Support](https://docs.microsoft.com/azure/information-protection/get-started/information-support#to-contact-microsoft-support) or use your standard support channels.</span></span>

2. <span data-ttu-id="d0ac3-112">Raskite **meniu parinktis** Valdyti ir pasirinkite Apsaugos **aktyvinimas**.</span><span class="sxs-lookup"><span data-stu-id="d0ac3-112">Locate the **Manage** menu options, and select **Protection activation**.</span></span> <span data-ttu-id="d0ac3-113">Spustelėkite **Aktyvinti**, tada patvirtinkite savo veiksmą.</span><span class="sxs-lookup"><span data-stu-id="d0ac3-113">Click **Activate**, and then confirm your action.</span></span> <span data-ttu-id="d0ac3-114">Kai aktyvinimas bus baigtas, informacijos juostoje bus **sėkmingai rodoma Aktyvinimas.**</span><span class="sxs-lookup"><span data-stu-id="d0ac3-114">When activation is complete, the information bar displays **Activation finished successfully**.</span></span>

<span data-ttu-id="d0ac3-115">**"Azure" informacijos apsaugos etikečių perkėlimas į "Office 365" & atitikties centrą**</span><span class="sxs-lookup"><span data-stu-id="d0ac3-115">**Migrate Azure Information Protection labels to Office 365 Security & Compliance Center**</span></span>

1. <span data-ttu-id="d0ac3-116">Įsitikinkite, kad esate prisijungę kaip vartotojas su visuotinio administratoriaus teisėmis.</span><span class="sxs-lookup"><span data-stu-id="d0ac3-116">Make sure you are logged in as a user with Global Administrator permission.</span></span>

2. <span data-ttu-id="d0ac3-117">Eikite į **"Azure" informacijos apsaugos ašmenį.**</span><span class="sxs-lookup"><span data-stu-id="d0ac3-117">Navigate to the **Azure Information Protection** blade.</span></span>

3. <span data-ttu-id="d0ac3-118">Meniu **valdymo parinktis** pasirinkite **Vieningasis ženklinimas**.</span><span class="sxs-lookup"><span data-stu-id="d0ac3-118">From the **Manage** menu option, select **Unified labeling**.</span></span>

4. <span data-ttu-id="d0ac3-119">**"Azure" informacijos apsaugos – vieningosios etikečių ašmenyse** spustelėkite **Aktyvinti ir** vykdykite internetinius nurodymus.</span><span class="sxs-lookup"><span data-stu-id="d0ac3-119">On the **Azure Information Protection - Unified labeling** blade, click **Activate** and follow the online instructions.</span></span>

<span data-ttu-id="d0ac3-120">**Pastaba:** patikrinkite, ar turite atitinkamas teises prieš suaktyvindami saugos & centro perkėlimą.</span><span class="sxs-lookup"><span data-stu-id="d0ac3-120">**Note**: Verify that you have the appropriate permissions before activating the Security & Compliance Center Migration.</span></span> <span data-ttu-id="d0ac3-121">Daugiau informacijos žr. šiuose straipsniuose:</span><span class="sxs-lookup"><span data-stu-id="d0ac3-121">See these articles for more info:</span></span>

1. [<span data-ttu-id="d0ac3-122">Ar turite būti visuotinis administratorius, kad sukonfigūruotų "Azure" informacijos apsaugą, ar galiu perduoti kitiems administratoriams?</span><span class="sxs-lookup"><span data-stu-id="d0ac3-122">Do you need to be a global admin to configure Azure Information Protection, or can I delegate to other administrators?</span></span>](https://docs.microsoft.com/azure/information-protection/faqs#do-you-need-to-be-a-global-admin-to-configure-azure-information-protection-or-can-i-delegate-to-other-administrators)

2. [<span data-ttu-id="d0ac3-123">Svarbi informacija apie administravimo vaidmenis po perkėlimo į saugos & atitikties centrą.</span><span class="sxs-lookup"><span data-stu-id="d0ac3-123">Important information about administrative roles after migrating to Security & Compliance Center.</span></span>](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels#important-information-about-administrative-roles)

<span data-ttu-id="d0ac3-124">Daugiau informacijos apie AIP į vieningą etikečių perkėlimą į saugos ir atitikties centrą žr. [Etikečių perkėlimas](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels).</span><span class="sxs-lookup"><span data-stu-id="d0ac3-124">For more information on the AIP to Unified Labeling migration to Security and Compliance Center, see [Migrate labels](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels).</span></span>
