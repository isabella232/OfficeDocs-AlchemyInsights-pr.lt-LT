---
title: DLP gali reikėti pasirinktinio tipo
ms.author: pebaum
author: pebaum
manager: laurawi
ms.date: ''
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1647"
- "3200001"
ms.assetid: ''
ms.openlocfilehash: 87fcb5c3cc9ccd525265097b66d9d9b3a85c5feb
ms.sourcegitcommit: d108a2da2f5dab05246e30b5108cca5173e09051
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 03/26/2020
ms.locfileid: "42977278"
---
# <a name="dlp-might-need-a-custom-type"></a><span data-ttu-id="46144-102">DLP gali reikėti pasirinktinio tipo</span><span class="sxs-lookup"><span data-stu-id="46144-102">DLP might need a custom type</span></span>

<span data-ttu-id="46144-103">**Svarbu:** šiais precedento neturinčiais laikais imamės veiksmų, kad užtikrintume, jog "SharePoint Online" ir "OneDrive" paslaugos išliktų labai pasiekiamos – daugiau informacijos rasite ["SharePoint Online" laikinieji funkcijų koregavimai.](https://aka.ms/ODSPAdjustments)</span><span class="sxs-lookup"><span data-stu-id="46144-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="46144-104">**DLP gali reikėti pasirinktinio informacijos tipo**</span><span class="sxs-lookup"><span data-stu-id="46144-104">**DLP may require a custom information type**</span></span>

<span data-ttu-id="46144-105">Naudodami duomenų praradimo prevencijos (DLP) strategiją, galite identifikuoti ir apsaugoti slaptus organizacijos duomenis.</span><span class="sxs-lookup"><span data-stu-id="46144-105">With a data loss prevention (DLP) policy, you can identify and protect sensitive data in your organization.</span></span> <span data-ttu-id="46144-106">Kai kuriais atvejais gali reikėti sukurti savo **pasirinktinį** slaptos informacijos tipą, kad apsaugotumėte savo organizacijos duomenis.</span><span class="sxs-lookup"><span data-stu-id="46144-106">In some scenarios, you might need to create your own **custom** sensitive information type to protect your organization's data.</span></span>

<span data-ttu-id="46144-107">Pavyzdžiui, jūsų organizacijai gali reikėti identifikuoti ir apsaugoti darbuotojų TAPATYBĖS AR kitus duomenis tam tikru jūsų organizacijai būdingu formatu. Jei taip, daugiau informacijos rasite šiuose straipsniuose.</span><span class="sxs-lookup"><span data-stu-id="46144-107">For example, your organization might need to identify and protect employee IDs or other data in some format specific to your org. If so, see the following articles for more information.</span></span>
  
 <span data-ttu-id="46144-108">**Įtaisytojo slaptos informacijos tipo tinkinimas**</span><span class="sxs-lookup"><span data-stu-id="46144-108">**Customize a built-in sensitive information type**</span></span>
  
<span data-ttu-id="46144-109">Jei įtaisytasis slaptos informacijos tipas atitiktų jūsų poreikius vos keliais patobulinimais, galite [tinkinti įtaisytąjį slaptos informacijos tipą](https://docs.microsoft.com/office365/securitycompliance/customize-a-built-in-sensitive-information-type).</span><span class="sxs-lookup"><span data-stu-id="46144-109">If a built-in sensitive information type would meet your needs with just a few tweaks, you can [customize a built-in sensitive information type](https://docs.microsoft.com/office365/securitycompliance/customize-a-built-in-sensitive-information-type).</span></span> <span data-ttu-id="46144-110">Pavyzdžiui, galite pridėti arba pašalinti raktinius žodžius arba pridėti arba pašalinti patvirtinamuosius įrodymus, pvz., datą arba adresą.</span><span class="sxs-lookup"><span data-stu-id="46144-110">For example, you can add or remove keywords, or add or remove supporting evidence such as a date or address.</span></span>
  
 <span data-ttu-id="46144-111">**Pasirinktinio slaptos informacijos tipo kūrimas**</span><span class="sxs-lookup"><span data-stu-id="46144-111">**Create a custom sensitive information type**</span></span>
  
<span data-ttu-id="46144-112">Tačiau jei jums reikia nustatyti ir apsaugoti kito tipo slaptą informaciją, saugos & atitikties centro vartotojo sąsajoje galite [sukurti tinkintą slaptos informacijos tipą.](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type)</span><span class="sxs-lookup"><span data-stu-id="46144-112">But if you need to identify and protect a different type of sensitive information altogether, you can [create a custom sensitive information type](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type) in the UI of the Security & Compliance Center.</span></span>
  
<span data-ttu-id="46144-113">**Pasirinktinio slaptos informacijos tipo kūrimas saugos & atitikties centro "PowerShell"**</span><span class="sxs-lookup"><span data-stu-id="46144-113">**Create a custom sensitive information type in Security & Compliance Center PowerShell**</span></span>

<span data-ttu-id="46144-114">Galiausiai, jei vartotojo sąsaja nepateikia visų reikiamų parinkčių, galite [sukurti pasirinktinį slaptos informacijos tipą saugos & atitikties centro "PowerShell".](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type-in-scc-powershell)</span><span class="sxs-lookup"><span data-stu-id="46144-114">Finally, if the UI doesn't provide all the options you need, you can [create a custom sensitive information type in Security & Compliance Center PowerShell](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type-in-scc-powershell).</span></span> <span data-ttu-id="46144-115">Pradėdami nuo XML failo, galite naudoti kiekvieną galimą parinktį.</span><span class="sxs-lookup"><span data-stu-id="46144-115">By starting with an XML file, you can use every option available.</span></span>
