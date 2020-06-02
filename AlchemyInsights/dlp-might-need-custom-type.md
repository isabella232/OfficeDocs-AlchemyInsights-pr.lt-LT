---
title: DLP gali reikėti pasirinktinio tipo
ms.author: pebaum
author: pebaum
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1647"
- "3200001"
ms.assetid: ''
ms.openlocfilehash: 1ec8959a479f1a8f7bfcffb55f440e8c4ab435fb
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 06/02/2020
ms.locfileid: "44507522"
---
# <a name="dlp-might-need-a-custom-type"></a><span data-ttu-id="d8f58-102">DLP gali reikėti pasirinktinio tipo</span><span class="sxs-lookup"><span data-stu-id="d8f58-102">DLP might need a custom type</span></span>

<span data-ttu-id="d8f58-103">**Svarbu**: šiais precedento neturinčiais laikais imamės veiksmų, kad užtikrintumėte„SharePoint Online“ ir „OneDrive“ paslaugų pasiekiamumą. Jei reikia daugiau informacijos, apsilankykite [„SharePoint Online“ laikinas funkcijų koregavimas](https://aka.ms/ODSPAdjustments).</span><span class="sxs-lookup"><span data-stu-id="d8f58-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="d8f58-104">**DLP gali reikėti pasirinktinio informacijos tipo**</span><span class="sxs-lookup"><span data-stu-id="d8f58-104">**DLP may require a custom information type**</span></span>

<span data-ttu-id="d8f58-105">Naudodami duomenų praradimo prevencijos (DLP) strategiją, galite identifikuoti ir apsaugoti slaptus organizacijos duomenis.</span><span class="sxs-lookup"><span data-stu-id="d8f58-105">With a data loss prevention (DLP) policy, you can identify and protect sensitive data in your organization.</span></span> <span data-ttu-id="d8f58-106">Kai kuriais atvejais gali reikėti sukurti savo **pasirinktinį** slaptos informacijos tipą, kad apsaugotumėte savo organizacijos duomenis.</span><span class="sxs-lookup"><span data-stu-id="d8f58-106">In some scenarios, you might need to create your own **custom** sensitive information type to protect your organization's data.</span></span>

<span data-ttu-id="d8f58-107">Pavyzdžiui, jūsų organizacijai gali reikėti identifikuoti ir apsaugoti darbuotojų TAPATYBĖS AR kitus duomenis tam tikru jūsų organizacijai būdingu formatu. Jei taip, daugiau informacijos rasite šiuose straipsniuose.</span><span class="sxs-lookup"><span data-stu-id="d8f58-107">For example, your organization might need to identify and protect employee IDs or other data in some format specific to your org. If so, see the following articles for more information.</span></span>
  
 <span data-ttu-id="d8f58-108">**Įtaisytojo slaptos informacijos tipo tinkinimas**</span><span class="sxs-lookup"><span data-stu-id="d8f58-108">**Customize a built-in sensitive information type**</span></span>
  
<span data-ttu-id="d8f58-109">Jei įtaisytasis slaptos informacijos tipas atitiktų jūsų poreikius vos keliais patobulinimais, galite [tinkinti įtaisytąjį slaptos informacijos tipą](https://docs.microsoft.com/microsoft-365/compliance/customize-a-built-in-sensitive-information-type).</span><span class="sxs-lookup"><span data-stu-id="d8f58-109">If a built-in sensitive information type would meet your needs with just a few tweaks, you can [customize a built-in sensitive information type](https://docs.microsoft.com/microsoft-365/compliance/customize-a-built-in-sensitive-information-type).</span></span> <span data-ttu-id="d8f58-110">Pavyzdžiui, galite pridėti arba pašalinti raktinius žodžius arba pridėti arba pašalinti patvirtinamuosius įrodymus, pvz., datą arba adresą.</span><span class="sxs-lookup"><span data-stu-id="d8f58-110">For example, you can add or remove keywords, or add or remove supporting evidence such as a date or address.</span></span>
  
 <span data-ttu-id="d8f58-111">**Pasirinktinio slaptos informacijos tipo kūrimas**</span><span class="sxs-lookup"><span data-stu-id="d8f58-111">**Create a custom sensitive information type**</span></span>
  
<span data-ttu-id="d8f58-112">Tačiau jei jums reikia nustatyti ir apsaugoti kito tipo slaptą informaciją, saugos & atitikties centro vartotojo sąsajoje galite [sukurti tinkintą slaptos informacijos tipą.](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type)</span><span class="sxs-lookup"><span data-stu-id="d8f58-112">But if you need to identify and protect a different type of sensitive information altogether, you can [create a custom sensitive information type](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type) in the UI of the Security & Compliance Center.</span></span>
  
<span data-ttu-id="d8f58-113">**Pasirinktinio slaptos informacijos tipo kūrimas saugos & atitikties centro "PowerShell"**</span><span class="sxs-lookup"><span data-stu-id="d8f58-113">**Create a custom sensitive information type in Security & Compliance Center PowerShell**</span></span>

<span data-ttu-id="d8f58-114">Galiausiai, jei vartotojo sąsaja nepateikia visų reikiamų parinkčių, galite [sukurti pasirinktinį slaptos informacijos tipą saugos & atitikties centro "PowerShell".](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type-in-scc-powershell)</span><span class="sxs-lookup"><span data-stu-id="d8f58-114">Finally, if the UI doesn't provide all the options you need, you can [create a custom sensitive information type in Security & Compliance Center PowerShell](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type-in-scc-powershell).</span></span> <span data-ttu-id="d8f58-115">Pradėdami nuo XML failo, galite naudoti kiekvieną galimą parinktį.</span><span class="sxs-lookup"><span data-stu-id="d8f58-115">By starting with an XML file, you can use every option available.</span></span>
