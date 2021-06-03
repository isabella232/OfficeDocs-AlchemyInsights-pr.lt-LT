---
title: Įrenginio žymių arba grupių kūrimas ir valdymas
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 06/01/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11446"
- "9003537"
ms.openlocfilehash: 3a7d53beaaf830055904f0634f09a3e9e447006e
ms.sourcegitcommit: 1226e9a9601dc8fc8ec427235f3c2dd88ff84ced
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 06/02/2021
ms.locfileid: "52731669"
---
# <a name="create-and-manage-device-tags-or-groups"></a><span data-ttu-id="aa6a0-102">Įrenginio žymių arba grupių kūrimas ir valdymas</span><span class="sxs-lookup"><span data-stu-id="aa6a0-102">Create and manage device tags or groups</span></span>

<span data-ttu-id="aa6a0-103">Įtraukite žymių įrenginiuose, kad sukurtumėte loginį grupės priskyrimą.</span><span class="sxs-lookup"><span data-stu-id="aa6a0-103">Add tags on devices to create a logical group affiliation.</span></span> <span data-ttu-id="aa6a0-104">Įrenginio žymės palaiko tinkamą tinklo susiejimą, leidžia pridėti skirtingas žymes, kad užfiksuotumėte kontekstą ir įgalintumėte dinaminį sąrašo kūrimą kaip incidento dalį.</span><span class="sxs-lookup"><span data-stu-id="aa6a0-104">Device tags support proper mapping of the network, enabling you to attach different tags to capture context and to enable dynamic list creation as part of an incident.</span></span> <span data-ttu-id="aa6a0-105">Žymes galima naudoti kaip filtrą rodinyje Įrenginiai arba grupuoti įrenginius.</span><span class="sxs-lookup"><span data-stu-id="aa6a0-105">Tags can be used as a filter in Devices list view, or to group devices.</span></span> <span data-ttu-id="aa6a0-106">Daugiau informacijos apie įrenginių grupavimą žr. [Įrenginio žymių kūrimas ir valdymas](/microsoft-365/security/defender-endpoint/machine-tags).</span><span class="sxs-lookup"><span data-stu-id="aa6a0-106">For more information on device grouping, see [Create and manage device tags](/microsoft-365/security/defender-endpoint/machine-tags).</span></span>

<span data-ttu-id="aa6a0-107">Galite įtraukti žymių įrenginiuose:</span><span class="sxs-lookup"><span data-stu-id="aa6a0-107">You can add tags on devices by:</span></span>

- <span data-ttu-id="aa6a0-108">Portalo naudojimas</span><span class="sxs-lookup"><span data-stu-id="aa6a0-108">Using the portal</span></span>

- <span data-ttu-id="aa6a0-109">Registro rakto reikšmės nustatymas</span><span class="sxs-lookup"><span data-stu-id="aa6a0-109">Setting a registry key value</span></span>
 
<span data-ttu-id="aa6a0-110">**Pastaba:** Gali būti gaišties tarp to laiko, kai žymė įtraukiama į įrenginį, ir jos pasiekiamumo įrenginių sąraše ir įrenginio puslapyje.</span><span class="sxs-lookup"><span data-stu-id="aa6a0-110">**Note:** There could be latency between the time a tag is added to a device and its availability in the devices list and device page.</span></span>

<span data-ttu-id="aa6a0-111">Norėdami įtraukti įrenginio žymes naudodami API, [žr. Įrenginio žymių API įtraukimas arba pašalinimas.](/microsoft-365/security/defender-endpoint/add-or-remove-machine-tags)</span><span class="sxs-lookup"><span data-stu-id="aa6a0-111">To add device tags using API, see [Add or remove device tags API](/microsoft-365/security/defender-endpoint/add-or-remove-machine-tags).</span></span>

## <a name="add-and-manage-device-tags-using-the-portal"></a><span data-ttu-id="aa6a0-112">Įrenginio žymių įtraukimas ir valdymas naudojant portalą</span><span class="sxs-lookup"><span data-stu-id="aa6a0-112">Add and manage device tags using the portal</span></span>

1. <span data-ttu-id="aa6a0-113">Pasirinkite įrenginį, kuriame norite valdyti žymes.</span><span class="sxs-lookup"><span data-stu-id="aa6a0-113">Select the device that you want to manage tags on.</span></span> <span data-ttu-id="aa6a0-114">Galite pasirinkti arba ieškoti įrenginio bet kuriame iš šių rodinių:</span><span class="sxs-lookup"><span data-stu-id="aa6a0-114">You can select or search for a device from any of the following views:</span></span>

    - <span data-ttu-id="aa6a0-115">**Saugos operacijų ataskaitų sritis** Pasirinkite įrenginio pavadinimą iš skyriaus Populiariausi įrenginiai su aktyviais įspėjimais.</span><span class="sxs-lookup"><span data-stu-id="aa6a0-115">**Security operations dashboard** Select the device name from the Top devices with active alerts section.</span></span>
    - <span data-ttu-id="aa6a0-116">**Įspėjimų eilė** – pasirinkite įrenginio pavadinimą šalia įrenginio piktogramos iš įspėjimų eilės.</span><span class="sxs-lookup"><span data-stu-id="aa6a0-116">**Alerts queue** - Select the device name beside the device icon from the alerts queue.</span></span>
    - <span data-ttu-id="aa6a0-117">**Įrenginių** sąrašas – pasirinkite įrenginio pavadinimą iš įrenginių sąrašo.</span><span class="sxs-lookup"><span data-stu-id="aa6a0-117">**Devices list** - Select the device name from the list of devices.</span></span>
    - <span data-ttu-id="aa6a0-118">**Ieškos laukas** – išplečiamajame meniu pasirinkite Įrenginys ir įveskite įrenginio pavadinimą.</span><span class="sxs-lookup"><span data-stu-id="aa6a0-118">**Search box** - Select Device from the drop-down menu and enter the device name.</span></span>

    <span data-ttu-id="aa6a0-119">Taip pat galite patekti į įspėjimo puslapį per failo ir IP rodinius.</span><span class="sxs-lookup"><span data-stu-id="aa6a0-119">You can also get to the alert page through the file and IP views.</span></span>

1. <span data-ttu-id="aa6a0-120">Atsakymų **veiksmų** eilutėje pasirinkite Valdyti žymes.</span><span class="sxs-lookup"><span data-stu-id="aa6a0-120">Select **Manage Tags** from the row of Response actions.</span></span>

1. <span data-ttu-id="aa6a0-121">Įveskite, kad rastumėte arba sukurtumėte žymes.</span><span class="sxs-lookup"><span data-stu-id="aa6a0-121">Type to find or create tags.</span></span>

<span data-ttu-id="aa6a0-122">Žymės yra įtraukiami į įrenginio rodinį ir atsispindi įrenginių sąrašo rodinyje.</span><span class="sxs-lookup"><span data-stu-id="aa6a0-122">Tags are added to the device view and are reflected on the Devices list view.</span></span> <span data-ttu-id="aa6a0-123">Tada galite naudoti filtrą Žymės, kad pamatytumėte atitinkamą įrenginių sąrašą.</span><span class="sxs-lookup"><span data-stu-id="aa6a0-123">You can then use the Tags filter to see the relevant list of devices.</span></span>

<span data-ttu-id="aa6a0-124">Daugiau informacijos žr. [Įrenginio žymių kūrimas ir valdymas](/microsoft-365/security/defender-endpoint/machine-tags).</span><span class="sxs-lookup"><span data-stu-id="aa6a0-124">For more information, see [Create and manage device tags](/microsoft-365/security/defender-endpoint/machine-tags).</span></span>