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
ms.openlocfilehash: 890bba57bc36c034c507e6124cd6593ef4d92af8
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932666"
---
# <a name="dlp-might-need-a-custom-type"></a><span data-ttu-id="103ff-102">DLP gali reikėti pasirinktinio tipo</span><span class="sxs-lookup"><span data-stu-id="103ff-102">DLP might need a custom type</span></span>

<span data-ttu-id="103ff-103">**Svarbu:** daugelis "SharePoint Online" ir "OneDrive" klientų vykdo verslui svarbias taikomąsias programas pagal fone vykdomą tarnybą.</span><span class="sxs-lookup"><span data-stu-id="103ff-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="103ff-104">Tai apima turinio perkėlimą, duomenų praradimo prevenciją (DLP) ir atsarginių kopijų kūrimo sprendimus.</span><span class="sxs-lookup"><span data-stu-id="103ff-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="103ff-105">Šiais precedento neturinčiais laikais imamės veiksmų, kad užtikrintume, jog "SharePoint Online" ir "OneDrive" paslaugos būtų labai prieinamos ir patikimos jūsų vartotojams, kurie labiau nei bet kada priklauso nuo paslaugos nuotoliniuose darbo scenarijuose.</span><span class="sxs-lookup"><span data-stu-id="103ff-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="103ff-106">Siekdami šio tikslo, darbo dienos valandomis įdiegėme griežtesnius buferizavimo apribojimus fonines programas (migraciją, DLP ir atsarginius sprendimus).</span><span class="sxs-lookup"><span data-stu-id="103ff-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="103ff-107">Turėtumėte tikėtis, kad šios programos pasieks labai ribotą pralaidumą šiais laikais.</span><span class="sxs-lookup"><span data-stu-id="103ff-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="103ff-108">Tačiau regiono vakaro ir savaitgalio valandomis paslauga bus paruošta apdoroti žymiai didesnį užklausų iš foninių programų apimtį.</span><span class="sxs-lookup"><span data-stu-id="103ff-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="103ff-109">**DLP gali reikėti pasirinktinio informacijos tipo**</span><span class="sxs-lookup"><span data-stu-id="103ff-109">**DLP may require a custom information type**</span></span>

<span data-ttu-id="103ff-110">Naudodami duomenų praradimo prevencijos (DLP) strategiją, galite identifikuoti ir apsaugoti slaptus organizacijos duomenis.</span><span class="sxs-lookup"><span data-stu-id="103ff-110">With a data loss prevention (DLP) policy, you can identify and protect sensitive data in your organization.</span></span> <span data-ttu-id="103ff-111">Kai kuriais atvejais gali reikėti sukurti savo **pasirinktinį** slaptos informacijos tipą, kad apsaugotumėte savo organizacijos duomenis.</span><span class="sxs-lookup"><span data-stu-id="103ff-111">In some scenarios, you might need to create your own **custom** sensitive information type to protect your organization's data.</span></span>

<span data-ttu-id="103ff-112">Pavyzdžiui, jūsų organizacijai gali reikėti identifikuoti ir apsaugoti darbuotojų TAPATYBĖS AR kitus duomenis tam tikru jūsų organizacijai būdingu formatu. Jei taip, daugiau informacijos rasite šiuose straipsniuose.</span><span class="sxs-lookup"><span data-stu-id="103ff-112">For example, your organization might need to identify and protect employee IDs or other data in some format specific to your org. If so, see the following articles for more information.</span></span>
  
 <span data-ttu-id="103ff-113">**Įtaisytojo slaptos informacijos tipo tinkinimas**</span><span class="sxs-lookup"><span data-stu-id="103ff-113">**Customize a built-in sensitive information type**</span></span>
  
<span data-ttu-id="103ff-114">Jei įtaisytasis slaptos informacijos tipas atitiktų jūsų poreikius vos keliais patobulinimais, galite [tinkinti įtaisytąjį slaptos informacijos tipą](https://docs.microsoft.com/office365/securitycompliance/customize-a-built-in-sensitive-information-type).</span><span class="sxs-lookup"><span data-stu-id="103ff-114">If a built-in sensitive information type would meet your needs with just a few tweaks, you can [customize a built-in sensitive information type](https://docs.microsoft.com/office365/securitycompliance/customize-a-built-in-sensitive-information-type).</span></span> <span data-ttu-id="103ff-115">Pavyzdžiui, galite pridėti arba pašalinti raktinius žodžius arba pridėti arba pašalinti patvirtinamuosius įrodymus, pvz., datą arba adresą.</span><span class="sxs-lookup"><span data-stu-id="103ff-115">For example, you can add or remove keywords, or add or remove supporting evidence such as a date or address.</span></span>
  
 <span data-ttu-id="103ff-116">**Pasirinktinio slaptos informacijos tipo kūrimas**</span><span class="sxs-lookup"><span data-stu-id="103ff-116">**Create a custom sensitive information type**</span></span>
  
<span data-ttu-id="103ff-117">Tačiau jei jums reikia nustatyti ir apsaugoti kito tipo slaptą informaciją, saugos & atitikties centro vartotojo sąsajoje galite [sukurti tinkintą slaptos informacijos tipą.](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type)</span><span class="sxs-lookup"><span data-stu-id="103ff-117">But if you need to identify and protect a different type of sensitive information altogether, you can [create a custom sensitive information type](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type) in the UI of the Security & Compliance Center.</span></span>
  
<span data-ttu-id="103ff-118">**Pasirinktinio slaptos informacijos tipo kūrimas saugos & atitikties centro "PowerShell"**</span><span class="sxs-lookup"><span data-stu-id="103ff-118">**Create a custom sensitive information type in Security & Compliance Center PowerShell**</span></span>

<span data-ttu-id="103ff-119">Galiausiai, jei vartotojo sąsaja nepateikia visų reikiamų parinkčių, galite [sukurti pasirinktinį slaptos informacijos tipą saugos & atitikties centro "PowerShell".](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type-in-scc-powershell)</span><span class="sxs-lookup"><span data-stu-id="103ff-119">Finally, if the UI doesn't provide all the options you need, you can [create a custom sensitive information type in Security & Compliance Center PowerShell](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type-in-scc-powershell).</span></span> <span data-ttu-id="103ff-120">Pradėdami nuo XML failo, galite naudoti kiekvieną galimą parinktį.</span><span class="sxs-lookup"><span data-stu-id="103ff-120">By starting with an XML file, you can use every option available.</span></span>
