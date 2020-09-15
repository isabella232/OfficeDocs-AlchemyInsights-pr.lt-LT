---
title: DLP gali reikėti pasirinktinio tipo
ms.author: pebaum
author: pebaum
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1647"
- "3200001"
ms.assetid: ''
ms.openlocfilehash: 72b16d437f97de27cbdc364f022c3e2059b31ef0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47712192"
---
# <a name="dlp-might-need-a-custom-type"></a><span data-ttu-id="5668e-102">DLP gali reikėti pasirinktinio tipo</span><span class="sxs-lookup"><span data-stu-id="5668e-102">DLP might need a custom type</span></span>

<span data-ttu-id="5668e-103">**Svarbu**: šiais precedento neturinčiais laikais imamės veiksmų, kad užtikrintumėte„SharePoint Online“ ir „OneDrive“ paslaugų pasiekiamumą. Jei reikia daugiau informacijos, apsilankykite [„SharePoint Online“ laikinas funkcijų koregavimas](https://aka.ms/ODSPAdjustments).</span><span class="sxs-lookup"><span data-stu-id="5668e-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="5668e-104">**DLP gali reikalauti pasirinktinio informacijos tipo**</span><span class="sxs-lookup"><span data-stu-id="5668e-104">**DLP may require a custom information type**</span></span>

<span data-ttu-id="5668e-105">Naudodami duomenų praradimo prevencijos (DLP) strategiją, galite nustatyti ir apsaugoti svarbius organizacijos duomenis.</span><span class="sxs-lookup"><span data-stu-id="5668e-105">With a data loss prevention (DLP) policy, you can identify and protect sensitive data in your organization.</span></span> <span data-ttu-id="5668e-106">Kai kuriuose scenarijuose gali reikėti sukurti savo **pasirinktinio** slapto informacijos tipą, kad apsaugotumėte savo organizacijos duomenis.</span><span class="sxs-lookup"><span data-stu-id="5668e-106">In some scenarios, you might need to create your own **custom** sensitive information type to protect your organization's data.</span></span>

<span data-ttu-id="5668e-107">Pavyzdžiui, jūsų organizacijai gali reikėti identifikuoti ir apsaugoti darbuotojų ID arba kitus duomenis tam tikru jūsų organizacijos formatu. Jei taip, daugiau informacijos rasite tolesniuose straipsniuose.</span><span class="sxs-lookup"><span data-stu-id="5668e-107">For example, your organization might need to identify and protect employee IDs or other data in some format specific to your org. If so, see the following articles for more information.</span></span>
  
 <span data-ttu-id="5668e-108">**Įtaisytosios slaptos informacijos tipo tinkinimas**</span><span class="sxs-lookup"><span data-stu-id="5668e-108">**Customize a built-in sensitive information type**</span></span>
  
<span data-ttu-id="5668e-109">Jei įtaisytasis slaptos informacijos tipas atitinka jūsų poreikius vos keliais tweaks, galite [Tinkinti įtaisytąjį slaptą informacijos tipą](https://docs.microsoft.com/microsoft-365/compliance/customize-a-built-in-sensitive-information-type).</span><span class="sxs-lookup"><span data-stu-id="5668e-109">If a built-in sensitive information type would meet your needs with just a few tweaks, you can [customize a built-in sensitive information type](https://docs.microsoft.com/microsoft-365/compliance/customize-a-built-in-sensitive-information-type).</span></span> <span data-ttu-id="5668e-110">Pavyzdžiui, galite įtraukti arba pašalinti raktinius žodžius arba įtraukti arba pašalinti patvirtinamuosius duomenis, pvz., datą ar adresą.</span><span class="sxs-lookup"><span data-stu-id="5668e-110">For example, you can add or remove keywords, or add or remove supporting evidence such as a date or address.</span></span>
  
 <span data-ttu-id="5668e-111">**Pasirinktinio slapto informacijos tipo kūrimas**</span><span class="sxs-lookup"><span data-stu-id="5668e-111">**Create a custom sensitive information type**</span></span>
  
<span data-ttu-id="5668e-112">Tačiau jei reikia nustatyti ir apsaugoti kitą slaptą informaciją iš viso, galite [sukurti pasirinktinio slapto pobūdžio informacijos tipą](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type) saugos & atitikties centro vartotojo sąsajoje.</span><span class="sxs-lookup"><span data-stu-id="5668e-112">But if you need to identify and protect a different type of sensitive information altogether, you can [create a custom sensitive information type](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type) in the UI of the Security & Compliance Center.</span></span>
  
<span data-ttu-id="5668e-113">**Pasirinktinio slapto informacijos tipo kūrimas saugos & atitikties centro "PowerShell"**</span><span class="sxs-lookup"><span data-stu-id="5668e-113">**Create a custom sensitive information type in Security & Compliance Center PowerShell**</span></span>

<span data-ttu-id="5668e-114">Galiausiai, jei vartotojo sąsaja nepateikia visų jums reikalingų parinkčių, galite [sukurti pasirinktinio slapto informacijos tipo saugos & atitikties centro "PowerShell](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type-in-scc-powershell)".</span><span class="sxs-lookup"><span data-stu-id="5668e-114">Finally, if the UI doesn't provide all the options you need, you can [create a custom sensitive information type in Security & Compliance Center PowerShell](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type-in-scc-powershell).</span></span> <span data-ttu-id="5668e-115">Pradėdami naudoti XML failą, galite naudoti visas galimas parinktis.</span><span class="sxs-lookup"><span data-stu-id="5668e-115">By starting with an XML file, you can use every option available.</span></span>
