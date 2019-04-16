---
title: DLP gali prireikti pasirinktinį tipas
ms.author: stephow
author: stephow-MSFT
manager: laurawi
ms.date: ''
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: cd5bac5efe3a16d32f9b695c8cb452a1eaa3a796
ms.sourcegitcommit: e87b3f691444db3b9f460c9a3109146dc7ad4f80
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 04/15/2019
ms.locfileid: "31872418"
---
# <a name="dlp-might-need-a-custom-type"></a><span data-ttu-id="ad486-102">DLP gali prireikti pasirinktinį tipas</span><span class="sxs-lookup"><span data-stu-id="ad486-102">DLP might need a custom type</span></span>

<span data-ttu-id="ad486-103">Duomenų praradimo prevencija (DLP) politiką, galite nustatyti ir apsaugoti slaptus duomenis savo organizacijoje.</span><span class="sxs-lookup"><span data-stu-id="ad486-103">With a data loss prevention (DLP) policy, you can identify and protect sensitive data in your organization.</span></span> <span data-ttu-id="ad486-104">Kai kuriais atvejais, jums gali tekti sukurti savo **pasirinktinį** slaptos informacijos tipo apsaugoti organizacijos duomenis.</span><span class="sxs-lookup"><span data-stu-id="ad486-104">In some scenarios, you might need to create your own **custom** sensitive information type to protect your organization's data.</span></span>

<span data-ttu-id="ad486-105">Pavyzdžiui, jūsų organizacijai gali tekti nustatyti ir apsaugoti darbuotojo ID ar kitus duomenis kai kurie formatu su savo org. Jei taip, skaitykite šiuos straipsnius daugiau informacijos.</span><span class="sxs-lookup"><span data-stu-id="ad486-105">For example, your organization might need to identify and protect employee IDs or other data in some format specific to your org. If so, see the following articles for more information.</span></span> 
  
 <span data-ttu-id="ad486-106">**Tinkinti įmontuota slapta informacija tipas**</span><span class="sxs-lookup"><span data-stu-id="ad486-106">**Customize a built-in sensitive information type**</span></span>
  
<span data-ttu-id="ad486-107">Jei įmontuota slapta informacija tipo būtų patenkinti savo poreikius tik keletą tweaks, galite [Tinkinti built-in slaptos informacijos tipas](https://docs.microsoft.com/en-us/office365/securitycompliance/customize-a-built-in-sensitive-information-type).</span><span class="sxs-lookup"><span data-stu-id="ad486-107">If a built-in sensitive information type would meet your needs with just a few tweaks, you can [customize a built-in sensitive information type](https://docs.microsoft.com/en-us/office365/securitycompliance/customize-a-built-in-sensitive-information-type).</span></span> <span data-ttu-id="ad486-108">Pvz., jūs galite pridėti arba pašalinti raktinius žodžius, arba pridėti ar pašalinti patvirtinančius įrodymus, pvz., dienos arba adresas.</span><span class="sxs-lookup"><span data-stu-id="ad486-108">For example, you can add or remove keywords, or add or remove supporting evidence such as a date or address.</span></span>
  
 <span data-ttu-id="ad486-109">**Sukurti pasirinktinį slaptos informacijos tipą**</span><span class="sxs-lookup"><span data-stu-id="ad486-109">**Create a custom sensitive information type**</span></span>
  
<span data-ttu-id="ad486-110">Bet jei jums reikia nustatyti ir apsaugoti visiškai kitokia slapta informacija, galite [sukurti pasirinktinį slaptos informacijos tipą](https://docs.microsoft.com/en-us/office365/securitycompliance/create-a-custom-sensitive-information-type) saugumo & atitikties centro vartotojo sąsaja.</span><span class="sxs-lookup"><span data-stu-id="ad486-110">But if you need to identify and protect a different type of sensitive information altogether, you can [create a custom sensitive information type](https://docs.microsoft.com/en-us/office365/securitycompliance/create-a-custom-sensitive-information-type) in the UI of the Security & Compliance Center.</span></span> 
  
<span data-ttu-id="ad486-111">**Sukurti pasirinktinį slaptos informacijos tipą saugumo & atitikties centro "PowerShell"**</span><span class="sxs-lookup"><span data-stu-id="ad486-111">**Create a custom sensitive information type in Security & Compliance Center PowerShell**</span></span>

<span data-ttu-id="ad486-112">Galiausiai, jei UI neteikia visų variantų jums reikia, galite [sukurti pasirinktinį slaptos informacijos tipą, saugumo & atitikties centro "PowerShell"](https://docs.microsoft.com/en-us/office365/securitycompliance/create-a-custom-sensitive-information-type-in-scc-powershell).</span><span class="sxs-lookup"><span data-stu-id="ad486-112">Finally, if the UI doesn't provide all the options you need, you can [create a custom sensitive information type in Security & Compliance Center PowerShell](https://docs.microsoft.com/en-us/office365/securitycompliance/create-a-custom-sensitive-information-type-in-scc-powershell).</span></span> <span data-ttu-id="ad486-113">Pradedant XML failą, galite naudoti visomis.</span><span class="sxs-lookup"><span data-stu-id="ad486-113">By starting with an XML file, you can use every option available.</span></span>

    