---
title: 'AIP skaitytuvas: diegimas ir konfigūravimas'
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002278"
- "5119"
ms.openlocfilehash: d059d411aef03ca57662b71fbd7d27aecd3e0e57
ms.sourcegitcommit: c46b8df485edbd13e8bb4d1b2ba1c2821ddc9da0
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 05/23/2020
ms.locfileid: "44358101"
---
# <a name="aip-scanner-installation-and-configuration"></a><span data-ttu-id="7cc16-102">AIP skaitytuvas: diegimas ir konfigūravimas</span><span class="sxs-lookup"><span data-stu-id="7cc16-102">AIP scanner: installation and configuration</span></span>

<span data-ttu-id="7cc16-103">**Norėdami įdiegti AIP skaitytuvą, vadovaukitės rekomenduojamomis gairėmis:**</span><span class="sxs-lookup"><span data-stu-id="7cc16-103">**To install the AIP scanner, follow the recommended guidelines**:</span></span>

1. <span data-ttu-id="7cc16-104">Jei naujinate ir neatliekate švaraus diegimo, įsitikinkite, kad vadovavotės ["Azure" informacijos apsaugos skaitytuvo naujinimo](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide#upgrading-the-azure-information-protection-scanner) gairėmis ir vieningosios etikečių kliento versijos [naujinimo](https://docs.microsoft.com/azure/information-protection/rms-client/clientv2-admin-guide#upgrading-the-azure-information-protection-scanner)gairėmis, žr.</span><span class="sxs-lookup"><span data-stu-id="7cc16-104">If you are upgrading and not performing a clean installation, please make sure you have followed the guidelines for [upgrading the Azure Information Protection scanner](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide#upgrading-the-azure-information-protection-scanner) and for unified labeling client, see [upgrading the Azure Information Protection scanner](https://docs.microsoft.com/azure/information-protection/rms-client/clientv2-admin-guide#upgrading-the-azure-information-protection-scanner).</span></span>
2. <span data-ttu-id="7cc16-105">Patikrinkite, ar atitinkate visus [užkardos ir tinklo infrastruktūros parametrų reikalavimus](https://docs.microsoft.com/azure/information-protection/requirements#firewalls-and-network-infrastructure).</span><span class="sxs-lookup"><span data-stu-id="7cc16-105">Verify that you comply with all [Firewalls and network infrastructure settings requirements](https://docs.microsoft.com/azure/information-protection/requirements#firewalls-and-network-infrastructure).</span></span>
3. <span data-ttu-id="7cc16-106">Įsitikinkite, kad [jūsų strategijos nustatytos](https://docs.microsoft.com/azure/information-protection/configure-policy) kaip automatinis žymėjimas arba strategijos numatytoji etiketė.</span><span class="sxs-lookup"><span data-stu-id="7cc16-106">Make sure your [policies are set](https://docs.microsoft.com/azure/information-protection/configure-policy) to automatic labeling or have a default label in the policy.</span></span>
4. <span data-ttu-id="7cc16-107">Įsitikinkite, kad atitinkamas failo tipas yra sukonfigūruotas etiketės/apsaugos, kaip aprašyta [failų tipai palaiko Azure informacijos apsaugos klientas](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-file-types#supported-file-types-for-classification-and-protection).</span><span class="sxs-lookup"><span data-stu-id="7cc16-107">Make sure that the relevant file type is configured for label/protection as described in [File types supported by the Azure Information Protection client](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-file-types#supported-file-types-for-classification-and-protection).</span></span> <span data-ttu-id="7cc16-108">Be to, jei norite pakeisti numatytąjį veikimą, atlikite šiuos veiksmus: [Numatytojo failų apsaugos lygio keitimas](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-file-types#changing-the-default-protection-level-of-files).</span><span class="sxs-lookup"><span data-stu-id="7cc16-108">In addition, if you want to change the default behavior, follow these guidelines: [Changing the default protection level of files](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-file-types#changing-the-default-protection-level-of-files).</span></span>
5. <span data-ttu-id="7cc16-109">Patikrinkite, ar vartotojo abonementas, sukonfigūruotas paleisti skaitytuvo tarnybą, turi teisę pasiekti visas sukonfigūruotas saugyklas.</span><span class="sxs-lookup"><span data-stu-id="7cc16-109">Verify that the user account configured to run the scanner service has permissions to access all the configured repositories.</span></span>
6. <span data-ttu-id="7cc16-110">Jei vis tiek kyla problemų, eksportuokite skaitytuvo žurnalus ir pridėkite juos prie palaikymo bilieto.</span><span class="sxs-lookup"><span data-stu-id="7cc16-110">If you still experience issues, please export the scanner logs and add them to your support ticket.</span></span>

<span data-ttu-id="7cc16-111">**Eksportuoti Azure informacijos apsaugos skaitytuvas žurnalus**</span><span class="sxs-lookup"><span data-stu-id="7cc16-111">**Export Azure Information Protection Scanner logs**</span></span>

1. <span data-ttu-id="7cc16-112">Eikite į %localappdata%\Microsoft\MSIP vartotojo kontekste, kuriame veikia skaitytuvo tarnyba.</span><span class="sxs-lookup"><span data-stu-id="7cc16-112">Navigate to %localappdata%\Microsoft\MSIP under the user context running the scanner service.</span></span>
2. <span data-ttu-id="7cc16-113">Zip visą turinį pagal MSIP aplanką.</span><span class="sxs-lookup"><span data-stu-id="7cc16-113">Zip all the contents under the MSIP folder.</span></span>
3. <span data-ttu-id="7cc16-114">Įrašykite žurnalus į savo vietą ir pridėkite juos prie aptarnavimo užklausos.</span><span class="sxs-lookup"><span data-stu-id="7cc16-114">Save the logs to your choice of location, and attach them to your service request.</span></span>
4. <span data-ttu-id="7cc16-115">Taip pat galite naudoti [Export-AIPLogs -OnBehalfOf](https://docs.microsoft.com/powershell/module/azureinformationprotection/export-aiplogs?view=azureipps).</span><span class="sxs-lookup"><span data-stu-id="7cc16-115">You can also use [Export-AIPLogs -OnBehalfOf](https://docs.microsoft.com/powershell/module/azureinformationprotection/export-aiplogs?view=azureipps).</span></span>

<span data-ttu-id="7cc16-116">**Daugiau informacijos rasite**:</span><span class="sxs-lookup"><span data-stu-id="7cc16-116">**For additional information, see**:</span></span>
- [<span data-ttu-id="7cc16-117">"Azure" informacijos apsaugos skaitytuvo diegimas automatiškai klasifikuoti ir apsaugoti failus</span><span class="sxs-lookup"><span data-stu-id="7cc16-117">Deploying the Azure Information Protection scanner to automatically classify and protect files</span></span>](https://docs.microsoft.com/azure/information-protection/deploy-aip-scanner)
- [<span data-ttu-id="7cc16-118">Nustatyti ir naudoti atpažinimo ženklo parametras Set-AIPAuthentication</span><span class="sxs-lookup"><span data-stu-id="7cc16-118">Specify and use the Token parameter for Set-AIPAuthentication</span></span>](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-powershell#specify-and-use-the-token-parameter-for-set-aipauthentication)
- [<span data-ttu-id="7cc16-119">Aptikimo ciklo vykdymas ir skaitytuvo ataskaitų peržiūra</span><span class="sxs-lookup"><span data-stu-id="7cc16-119">Run a discovery cycle and view reports for the scanner</span></span>](https://docs.microsoft.com/azure/information-protection/deploy-aip-scanner#run-a-discovery-cycle-and-view-reports-for-the-scanner)
- [<span data-ttu-id="7cc16-120">"Azure" informacijos apsaugos dokumentų peržiūra</span><span class="sxs-lookup"><span data-stu-id="7cc16-120">Review Azure Information Protection documentation</span></span>](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [<span data-ttu-id="7cc16-121">"Azure" informacijos apsaugos reikalavimai</span><span class="sxs-lookup"><span data-stu-id="7cc16-121">Requirements for Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/get-started/requirements)
- [<span data-ttu-id="7cc16-122">Atsisiųskite "Azure" informacijos apsaugos klientą</span><span class="sxs-lookup"><span data-stu-id="7cc16-122">Download Azure Information Protection client</span></span>](https://www.microsoft.com/download/details.aspx?id=53018)
