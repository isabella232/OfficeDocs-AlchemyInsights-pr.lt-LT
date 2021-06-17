---
title: "\"Microsoft Intune\" naudojimas žiniatinklio prieigai valdyti \"Microsoft Edge\", skirtame \"iOS\" ir \"Android\""
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003846"
- "6895"
- "9006502"
- "11144"
ms.openlocfilehash: a6c6f9563933b7cf6b71c4758c29ffd94617c4be
ms.sourcegitcommit: 7a406a3d4680662e81f0056454f7e25fb2f52504
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 06/17/2021
ms.locfileid: "52989682"
---
# <a name="use-microsoft-intune-to-manage-web-access-in-microsoft-edge-for-ios-and-android"></a><span data-ttu-id="7c5f1-102">"Microsoft Intune" naudojimas žiniatinklio prieigai valdyti "Microsoft Edge", skirtame "iOS" ir "Android"</span><span class="sxs-lookup"><span data-stu-id="7c5f1-102">Use Microsoft Intune to manage web access in Microsoft Edge for iOS and Android</span></span>

<span data-ttu-id="7c5f1-103">"Microsoft Edge", skirta "iOS" ir "Android", leidžia vartotojui naršyti žiniatinklyje iš kelių visiškai atskirų profilių.</span><span class="sxs-lookup"><span data-stu-id="7c5f1-103">Microsoft Edge for iOS and Android lets a user browse the web from multiple, completely separate profiles.</span></span>

<span data-ttu-id="7c5f1-104">Plačiausios "Microsoft 365" duomenų apsaugos galimybės tampa prieinamos, kai prenumeruojate "Enterprise Mobility + Security" paketą, kuriame yra "Microsoft Intune" ir "Azure Active Directory Premium" funkcijos, pvz., sąlyginė prieiga.</span><span class="sxs-lookup"><span data-stu-id="7c5f1-104">The broadest protection capabilities for Microsoft 365 data become available when you subscribe to the Enterprise Mobility + Security suite, which includes Microsoft Intune and Azure Active Directory Premium features, such as conditional access.</span></span> <span data-ttu-id="7c5f1-105">Bent jau norite įdiegti sąlyginės prieigos strategiją, kuri (1) leidžia vartotojams prisijungti iš mobiliųjų įrenginių į "Microsoft Edge", skirtą "iOS" ir "Android", ir kad (2) įgyvendina "Microsoft Intune" programų apsaugos strategiją, kuri suteikia apsaugotą naršymo patirtį.</span><span class="sxs-lookup"><span data-stu-id="7c5f1-105">At a minimum, you’ll want to deploy a conditional access policy that (1) lets users connect from mobile devices to Microsoft Edge for iOS and Android and that (2) implements a Microsoft Intune app-protection policy that provides a protected browsing experience.</span></span>

<span data-ttu-id="7c5f1-106">Norėdami suprasti, kaip galite naudoti sąlyginę prieigą ir strategijas, žr.:</span><span class="sxs-lookup"><span data-stu-id="7c5f1-106">To understand how you can use conditional access and policies, see:</span></span>

[<span data-ttu-id="7c5f1-107">Taikyti "Azure Active Directory" sąlyginės prieigos strategijas</span><span class="sxs-lookup"><span data-stu-id="7c5f1-107">Apply Azure Active Directory conditional access policies</span></span>](https://go.microsoft.com/fwlink/?linkid=2132481)

[<span data-ttu-id="7c5f1-108">"Microsoft Intune" programų apsaugos strategijų kūrimas</span><span class="sxs-lookup"><span data-stu-id="7c5f1-108">Create Microsoft Intune app protection policies</span></span>](https://go.microsoft.com/fwlink/?linkid=2132651)

[<span data-ttu-id="7c5f1-109">Bendrosios a sign-on naudojimas "Azure Active Directory" prijungtoms žiniatinklio programoms strategijos apsaugotose naršyklėse</span><span class="sxs-lookup"><span data-stu-id="7c5f1-109">Use single sign-on for Azure Active Directory–connected web apps in policy-protected browsers</span></span>](https://go.microsoft.com/fwlink/?linkid=2132482)

[<span data-ttu-id="7c5f1-110">Programos konfigūravimo naudojimas naršymo patirčiai valdyti</span><span class="sxs-lookup"><span data-stu-id="7c5f1-110">Use app configuration to manage the browsing experience</span></span>](https://go.microsoft.com/fwlink/?linkid=2132483)

[<span data-ttu-id="7c5f1-111">Leisti naudoti tik darbo ir mokymo įstaigos paskyras</span><span class="sxs-lookup"><span data-stu-id="7c5f1-111">Allow the use of only work and school accounts</span></span>](https://go.microsoft.com/fwlink/?linkid=2132652)

[<span data-ttu-id="7c5f1-112">Bendrųjų taikomųjų programų konfigūravimo strategijų diegimas</span><span class="sxs-lookup"><span data-stu-id="7c5f1-112">Deploy general app configuration policies</span></span>](https://go.microsoft.com/fwlink/?linkid=2132653)

[<span data-ttu-id="7c5f1-113">Taikomosios programos konfigūravimo strategijų diegimas duomenų apsaugai</span><span class="sxs-lookup"><span data-stu-id="7c5f1-113">Deploy app configuration policies for data protection</span></span>](https://go.microsoft.com/fwlink/?linkid=2132654)

[<span data-ttu-id="7c5f1-114">"Microsoft Endpoint Manager" naudojimas norint įdiegti programos konfigūravimo strategijas</span><span class="sxs-lookup"><span data-stu-id="7c5f1-114">Use Microsoft Endpoint Manager to deploy app configuration policies</span></span>](https://go.microsoft.com/fwlink/?linkid=2132707)

<span data-ttu-id="7c5f1-115">Norėdami sužinoti, kaip pasiekti valdomų taikomųjų programų žurnalus, žr. ["Microsoft Edge", skirta "iOS" ir "Android", naudojimas valdomų programų žurnalams pasiekti.](https://go.microsoft.com/fwlink/?linkid=2132578)</span><span class="sxs-lookup"><span data-stu-id="7c5f1-115">To learn how to access managed app logs, see [Use Microsoft Edge for iOS and Android to access managed app logs](https://go.microsoft.com/fwlink/?linkid=2132578).</span></span>
