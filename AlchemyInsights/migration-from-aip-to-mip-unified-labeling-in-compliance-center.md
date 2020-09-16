---
title: Perkėlimas iš Ail į MIK/suvienodintas žymėjimas atitikties centre
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002278"
- "5114"
ms.openlocfilehash: 7157eada10db2443f64fb7925f408359275d75eb
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47674334"
---
# <a name="migration-from-aip-to-mipunified-labeling-in-the-compliance-center"></a><span data-ttu-id="444c8-102">Perkėlimas iš Ail į MIK/suvienodintas žymėjimas atitikties centre</span><span class="sxs-lookup"><span data-stu-id="444c8-102">Migration from AIP to MIP/Unified Labeling in the Compliance Center</span></span>

<span data-ttu-id="444c8-103">Norėdami perkelti iš Ail etikečių į saugos ir atitikties centro suvienodintą ženklinimą, atlikite šiuos veiksmus:</span><span class="sxs-lookup"><span data-stu-id="444c8-103">To migrate from AIP labels to Unified Labeling in the Security and Compliance center, do the following:</span></span>

<span data-ttu-id="444c8-104">**Apsaugos aktyvinimas iš "Azure" portalo**</span><span class="sxs-lookup"><span data-stu-id="444c8-104">**Activate protection from the Azure portal**</span></span>

1. <span data-ttu-id="444c8-105">Jei to dar nepadarėte, atidarykite naują naršyklės langą ir [Prisijunkite prie "Azure" portalo](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#signing-in-to-the-azure-portal).</span><span class="sxs-lookup"><span data-stu-id="444c8-105">If you haven't already done so, open a new browser window and [sign in to the Azure portal](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#signing-in-to-the-azure-portal).</span></span> <span data-ttu-id="444c8-106">Pereikite prie " **Azure" informacijos apsaugos** ašmenų.</span><span class="sxs-lookup"><span data-stu-id="444c8-106">Navigate to the **Azure Information Protection** blade.</span></span> <span data-ttu-id="444c8-107">Pvz., meniu koncentratorius spustelėkite **Visos tarnybos** ir pradėkite vesti **informaciją** lauke filtras.</span><span class="sxs-lookup"><span data-stu-id="444c8-107">For example, on the hub menu, click **All services** and start typing **Information** in the Filter box.</span></span> <span data-ttu-id="444c8-108">Pasirinkite **Azure informacijos apsauga**.</span><span class="sxs-lookup"><span data-stu-id="444c8-108">Select **Azure Information Protection**.</span></span> <span data-ttu-id="444c8-109">Jei anksčiau neprisijungėte prie "Azure" informacijos apsaugos disko, peržiūrėkite [papildomus veiksmus](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#to-access-the-azure-information-protection-blade-for-the-first-time) , kad įtrauktumėte šį diską į portalą.</span><span class="sxs-lookup"><span data-stu-id="444c8-109">If you haven't accessed the Azure Information Protection blade before, see the one-time [additional steps](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#to-access-the-azure-information-protection-blade-for-the-first-time) to add this blade to the portal.</span></span> <span data-ttu-id="444c8-110">Norėdami atidaryti "Azure" informacijos apsaugos diską, turite turėti " [Azure" informacijos apsaugos priemokų planą](https://www.microsoft.com/cloud-platform/azure-information-protection-pricing) arba "Office 365" planą, apimantį teisių valdymą.</span><span class="sxs-lookup"><span data-stu-id="444c8-110">To open the Azure Information Protection blade, you must have either an [Azure Information Protection Premium plan](https://www.microsoft.com/cloud-platform/azure-information-protection-pricing) or an Office 365 plan that includes Rights Management.</span></span> <span data-ttu-id="444c8-111">Jei turite vieną iš šių prenumeratų, bet matote pranešimą, kad nepavyksta rasti galiojančios prenumeratos, [kreipkitės į "Microsoft" palaikymo tarnybą](https://docs.microsoft.com/azure/information-protection/get-started/information-support#to-contact-microsoft-support) arba naudokite standartinius palaikymo kanalus.</span><span class="sxs-lookup"><span data-stu-id="444c8-111">If you have one of these subscriptions but see a message that a valid subscription cannot be found, [contact Microsoft Support](https://docs.microsoft.com/azure/information-protection/get-started/information-support#to-contact-microsoft-support) or use your standard support channels.</span></span>

2. <span data-ttu-id="444c8-112">Raskite meniu **tvarkyti** parinktis ir pasirinkite **apsaugos aktyvinimas**.</span><span class="sxs-lookup"><span data-stu-id="444c8-112">Locate the **Manage** menu options, and select **Protection activation**.</span></span> <span data-ttu-id="444c8-113">Spustelėkite **Aktyvinti**, tada patvirtinkite savo veiksmą.</span><span class="sxs-lookup"><span data-stu-id="444c8-113">Click **Activate**, and then confirm your action.</span></span> <span data-ttu-id="444c8-114">Kai aktyvinimas baigtas, informacijos juostoje rodoma **sėkmingai baigta aktyvinti**.</span><span class="sxs-lookup"><span data-stu-id="444c8-114">When activation is complete, the information bar displays **Activation finished successfully**.</span></span>

<span data-ttu-id="444c8-115">**"Azure" informacijos apsaugos žymų perkėlimas į "Office 365" saugos & atitikties centras**</span><span class="sxs-lookup"><span data-stu-id="444c8-115">**Migrate Azure Information Protection labels to Office 365 Security & Compliance Center**</span></span>

1. <span data-ttu-id="444c8-116">Įsitikinkite, kad esate prisijungęs kaip vartotojas su visuotinio administratoriaus teisėmis.</span><span class="sxs-lookup"><span data-stu-id="444c8-116">Make sure you are logged in as a user with Global Administrator permission.</span></span>

2. <span data-ttu-id="444c8-117">Pereikite prie " **Azure" informacijos apsaugos** ašmenų.</span><span class="sxs-lookup"><span data-stu-id="444c8-117">Navigate to the **Azure Information Protection** blade.</span></span>

3. <span data-ttu-id="444c8-118">Meniu **valdyti** parinktį pasirinkite **Bendrasis žymėjimas**.</span><span class="sxs-lookup"><span data-stu-id="444c8-118">From the **Manage** menu option, select **Unified labeling**.</span></span>

4. <span data-ttu-id="444c8-119">" **Azure" informacijos apsauga – bendrasis etiketės** peilis spustelėkite **Aktyvinti** ir vykdykite internetines instrukcijas.</span><span class="sxs-lookup"><span data-stu-id="444c8-119">On the **Azure Information Protection - Unified labeling** blade, click **Activate** and follow the online instructions.</span></span>

<span data-ttu-id="444c8-120">**Pastaba**: patikrinkite, ar turite atitinkamas teises prieš suaktyvindami saugos & atitikties centro perkėlimą.</span><span class="sxs-lookup"><span data-stu-id="444c8-120">**Note**: Verify that you have the appropriate permissions before activating the Security & Compliance Center Migration.</span></span> <span data-ttu-id="444c8-121">Daugiau informacijos ieškokite šiuose straipsniuose:</span><span class="sxs-lookup"><span data-stu-id="444c8-121">See these articles for more info:</span></span>

1. [<span data-ttu-id="444c8-122">Ar reikia būti visuotiniu administratoriumi, kad sukonfigūruotumėte Azure informacijos apsaugą arba galėčiau perduoti kitiems administratoriams?</span><span class="sxs-lookup"><span data-stu-id="444c8-122">Do you need to be a global admin to configure Azure Information Protection, or can I delegate to other administrators?</span></span>](https://docs.microsoft.com/azure/information-protection/faqs#do-you-need-to-be-a-global-admin-to-configure-azure-information-protection-or-can-i-delegate-to-other-administrators)

2. [<span data-ttu-id="444c8-123">Svarbi informacija apie administracinius vaidmenis perkėlus į saugos & atitikties centrą.</span><span class="sxs-lookup"><span data-stu-id="444c8-123">Important information about administrative roles after migrating to Security & Compliance Center.</span></span>](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels#important-information-about-administrative-roles)

<span data-ttu-id="444c8-124">Daugiau informacijos apie PPK, kad būtų galima suvienodinti perkėlimo į saugos ir atitikties centrą, ieškokite [etikečių perkėlimas](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels).</span><span class="sxs-lookup"><span data-stu-id="444c8-124">For more information on the AIP to Unified Labeling migration to Security and Compliance Center, see [Migrate labels](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels).</span></span>
