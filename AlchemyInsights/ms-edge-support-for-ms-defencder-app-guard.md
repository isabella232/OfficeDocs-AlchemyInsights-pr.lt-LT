---
title: "\"Microsoft Edge\" palaikymas, skirtas \"Microsoft Defender\" taikomosios programos apsaugai"
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/05/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004024"
- "7090"
ms.openlocfilehash: 65cbc867ea7d1c73ca2906f51f72aa3376f31b5d
ms.sourcegitcommit: 2e4a5153e530bf15744a52e982eeb0d99757e9d2
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 12/04/2020
ms.locfileid: "49584017"
---
# <a name="microsoft-edges-support-for-microsoft-defender-application-guard"></a><span data-ttu-id="46250-102">"Microsoft Edge" palaikymas, skirtas "Microsoft Defender" taikomosios programos apsaugai</span><span class="sxs-lookup"><span data-stu-id="46250-102">Microsoft Edge's support for Microsoft Defender Application Guard</span></span>

<span data-ttu-id="46250-103">Skirtas "Windows 10" ir "Microsoft Edge", taikomosios programos apsauga naudoja aparatūros izoliacijos metodą, leidžiantį vartotojui naršyti nepatikimą svetainę iš izoliuoto, "Hyper-V"-įgalinto konteinerio, atskirto nuo pagrindinio kompiuterio operacinės sistemos.</span><span class="sxs-lookup"><span data-stu-id="46250-103">Designed for Windows 10 and Microsoft Edge, Application Guard uses a hardware-isolation approach that lets a user navigate an untrusted site from inside an isolated, Hyper-V–enabled container, separated from the host operating system.</span></span>

<span data-ttu-id="46250-104">Įmonės administratorius apibrėžia patikimų svetainių, debesies išteklių ir vidinių tinklų sąrašą.</span><span class="sxs-lookup"><span data-stu-id="46250-104">An enterprise admin defines a list of trusted websites, cloud resources, and internal networks.</span></span> <span data-ttu-id="46250-105">Kai vartotojas apsilanko svetainėje, kurios nėra sąraše, "Microsoft Edge" atidarys vietą konteineryje.</span><span class="sxs-lookup"><span data-stu-id="46250-105">When a user visits a site that's not on the list, Microsoft Edge will open the site in the container.</span></span> <span data-ttu-id="46250-106">Tai reiškia, kad jei svetainė tampa kenkėjiška, pagrindinis kompiuteris liks apsaugotas, o užpuolikas negalės gauti įmonės duomenų.</span><span class="sxs-lookup"><span data-stu-id="46250-106">This means that if the site turns out to be malicious, the host PC will remain protected and the attacker won't get to the enterprise data.</span></span>

<span data-ttu-id="46250-107">Konteinerio plėtinių diegimas palaikomas kaip "Microsoft Edge" 81 versija ir jį galima valdyti naudojant strategiją.</span><span class="sxs-lookup"><span data-stu-id="46250-107">Installation of extensions in the container is supported as of Microsoft Edge version 81, and it can be controlled via a policy.</span></span> <span data-ttu-id="46250-108">UpdateURL adresas, kuris bus naudojamas ExtensionInstallForcelist strategijoje, turi būti įtrauktas kaip neutralus šaltinis tinklo izoliacijos strategijose, kurias naudoja taikomosios programos sargyba.</span><span class="sxs-lookup"><span data-stu-id="46250-108">The updateURL address that gets used in the ExtensionInstallForcelist policy should be added as a Neutral Resource in the Network Isolation policies used by Application Guard.</span></span>

<span data-ttu-id="46250-109">Daugiau informacijos ieškokite " [Microsoft Edge" palaikymas, skirtas "Microsoft Defender" taikomosios programos apsaugai](https://go.microsoft.com/fwlink/?linkid=2134229).</span><span class="sxs-lookup"><span data-stu-id="46250-109">For more info, see [Microsoft Edge support for Microsoft Defender Application Guard](https://go.microsoft.com/fwlink/?linkid=2134229).</span></span>
