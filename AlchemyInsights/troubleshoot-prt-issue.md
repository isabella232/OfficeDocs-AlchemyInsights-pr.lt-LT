---
title: "\"PRT\" problemos trikčių šalinimas"
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/01/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000076"
- "7317"
ms.openlocfilehash: 8e654a38d720aa51daf21bf5c3fb0da8b9c3d8e7
ms.sourcegitcommit: c069f1b53567ad14711c423740f120439a312a60
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 12/04/2020
ms.locfileid: "49573720"
---
# <a name="troubleshoot-prt-issue"></a><span data-ttu-id="b2067-102">"PRT" problemos trikčių šalinimas</span><span class="sxs-lookup"><span data-stu-id="b2067-102">Troubleshoot PRT issue</span></span>

<span data-ttu-id="b2067-103">Kad bet kuris įrenginys galėtų būti autentifikuotas, jis turi būti visiškai užregistruotas ir geras ir gali įsigyti pirminį atnaujinimo atpažinimo ženklą (PAG).</span><span class="sxs-lookup"><span data-stu-id="b2067-103">For any device to complete getting authenticated, it must be fully registered and in good state and able to acquire a Primary Refresh Token (PRT).</span></span>

<span data-ttu-id="b2067-104">Hibridinis "Azure AD" prisijungimo procesas reikalauja, kad įrenginiai būtų taikomi kolektyviniame tinkle.</span><span class="sxs-lookup"><span data-stu-id="b2067-104">The hybrid Azure AD join registration process requires devices to be on a corporate network.</span></span> <span data-ttu-id="b2067-105">Jis taip pat veikia per VPN, tačiau yra tam tikrų apribojimų.</span><span class="sxs-lookup"><span data-stu-id="b2067-105">It also works over VPN but there are some caveats to that.</span></span> <span data-ttu-id="b2067-106">Girdėjome klientų, kuriems reikia pagalbos šalinant hibridinio "Azure AD" prisijungimo procesą pagal nuotolinio darbo sąlygas.</span><span class="sxs-lookup"><span data-stu-id="b2067-106">We’ve heard customers needing assistance with troubleshooting the hybrid Azure AD join registration process under remote-work circumstances.</span></span> <span data-ttu-id="b2067-107">Toliau aprašyta, kas vyksta "po gaubtu" registracijos proceso metu.</span><span class="sxs-lookup"><span data-stu-id="b2067-107">Here’s a breakdown of what’s happening ‘under the hood’ during the registration process.</span></span>

<span data-ttu-id="b2067-108">**Debesies autentifikavimo aplinka (naudojant "Azure AD" slaptažodžių maišos sinchronizavimą arba Pass-per autentifikavimą)**</span><span class="sxs-lookup"><span data-stu-id="b2067-108">**Cloud authentication environment (using Azure AD password hash sync or pass-through authentication)**</span></span>

<span data-ttu-id="b2067-109">Šis registracijos srautas taip pat žinomas kaip "sinchronizavimo sujungimas".</span><span class="sxs-lookup"><span data-stu-id="b2067-109">This registration flow is also known as “Sync Join”.</span></span>

1. <span data-ttu-id="b2067-110">"Windows 10" aptinka "SCP" įrašą, kai vartotojas jungiasi prie įrenginio.</span><span class="sxs-lookup"><span data-stu-id="b2067-110">Windows 10 discovers an SCP record upon user logging on to the device.</span></span>
    1. <span data-ttu-id="b2067-111">Įrenginys pirmiausia bando gauti nuomotojo informaciją iš kliento "SCP" registre [HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD].</span><span class="sxs-lookup"><span data-stu-id="b2067-111">The device first tries to retrieve tenant information from client-side SCP in registry [HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD].</span></span> <span data-ttu-id="b2067-112">Daugiau informacijos ieškokite šiame [dokumente](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control).</span><span class="sxs-lookup"><span data-stu-id="b2067-112">For more information, see this [document](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control).</span></span>
    2. <span data-ttu-id="b2067-113">Jei nepavyksta, įrenginys palaiko ryšį su vietinio "Active Directory" (AD), kad gautų nuomotojo informaciją iš tarnybos jungties taško (SCP).</span><span class="sxs-lookup"><span data-stu-id="b2067-113">If it fails, the device communicates with on-premises Active Directory (AD) to get tenant information from Service Connection Point (SCP).</span></span> <span data-ttu-id="b2067-114">Norėdami patikrinti, ar yra "SCP", skaitykite šį [dokumentą](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-manual#configure-a-service-connection-point).</span><span class="sxs-lookup"><span data-stu-id="b2067-114">To verify SCP, please refer to this [document](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-manual#configure-a-service-connection-point).</span></span> 

> [!NOTE]
> <span data-ttu-id="b2067-115">Rekomenduojame įjungti "SCP" skelbimą ir naudoti tik kliento "SCP" pradiniam patvirtinimui.</span><span class="sxs-lookup"><span data-stu-id="b2067-115">We recommend enabling SCP in the AD and only using client-side SCP for initial validation.</span></span>

2. <span data-ttu-id="b2067-116">"Windows 10" bando palaikyti ryšį su "Azure AD" pagal sistemos kontekstą ir autentifikuoja save nuo "Azure AD".</span><span class="sxs-lookup"><span data-stu-id="b2067-116">Windows 10 tries to communicate with Azure AD under the system context to authenticate itself against Azure AD.</span></span> <span data-ttu-id="b2067-117">Galite patikrinti, ar įrenginys gali pasiekti "Microsoft" išteklius pagal sistemos paskyrą, naudodami bandomojo įrenginio registracijos ryšio scenarijų.</span><span class="sxs-lookup"><span data-stu-id="b2067-117">You can verify if the device can access Microsoft resources under the system account by using the Test Device Registration Connectivity script.</span></span>

3. <span data-ttu-id="b2067-118">"Windows 10" generuoja vartotojo pasirašomą sertifikatą ir saugo jį vietiniame skelbime esančiame kompiuterio objekte.</span><span class="sxs-lookup"><span data-stu-id="b2067-118">Windows 10 generates a self-signed certificate and stores it under the computer object in on-premises AD.</span></span> <span data-ttu-id="b2067-119">Tam reikia, kad būtų matomas domeno valdiklis.</span><span class="sxs-lookup"><span data-stu-id="b2067-119">This requires line-of-sight to Domain Controller.</span></span>

4. <span data-ttu-id="b2067-120">Įrenginio objektas, turintis sertifikatą, bus sinchronizuotas su "Azure AD" naudojant "Azure AD Connect".</span><span class="sxs-lookup"><span data-stu-id="b2067-120">A device object that has a certificate gets synchronized to Azure AD via Azure AD Connect.</span></span> <span data-ttu-id="b2067-121">Sinchronizavimo ciklas yra kas 30 minučių pagal numatytuosius parametrus, tačiau tai priklauso nuo "Azure AD Connect" konfigūracijos.</span><span class="sxs-lookup"><span data-stu-id="b2067-121">Sync cycle is every 30 minutes by default, but it depends on configuration of Azure AD Connect.</span></span> <span data-ttu-id="b2067-122">Daugiau informacijos rasite šiame [dokumente](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sync-configure-filtering#organizational-unitbased-filtering).</span><span class="sxs-lookup"><span data-stu-id="b2067-122">For more information, please refer to this [document](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sync-configure-filtering#organizational-unitbased-filtering).</span></span>

5. <span data-ttu-id="b2067-123">Šiame etape jums turėtų būti suteikta galimybė matyti temos įrenginį "laukianti" būsena dalyje "Azure" portalo įrenginio peilis.</span><span class="sxs-lookup"><span data-stu-id="b2067-123">At this stage, you should be able to see the subject device in “Pending” state under Device blade of Azure Portal.</span></span>

6. <span data-ttu-id="b2067-124">Kitas vartotojas prisijungęs prie "Windows 10", registracija bus atlikta.</span><span class="sxs-lookup"><span data-stu-id="b2067-124">At the next user login to Windows 10, the registration will be completed.</span></span> 

> [!NOTE]
> <span data-ttu-id="b2067-125">Jei esate VPN ir atsijungti prisijungimo procesas nutraukia domeno ryšį, galite suaktyvinti registraciją rankiniu būdu:</span><span class="sxs-lookup"><span data-stu-id="b2067-125">If you're on VPN and a logoff-login process terminates the domain connectivity, you can trigger registration manually:</span></span>
 1. <span data-ttu-id="b2067-126">"Dsregcmd" (prisijungti prie kompiuterio) arba nuotoliniu būdu per PSExec prie kompiuterio.</span><span class="sxs-lookup"><span data-stu-id="b2067-126">Issue a dsregcmd /join locally on admin prompt or remotely via PSExec to your PC.</span></span> <span data-ttu-id="b2067-127">Pvz., PsExec-s \\ win10client01 cmd, dsregcmd/Join</span><span class="sxs-lookup"><span data-stu-id="b2067-127">For example, PsExec -s \\win10client01 cmd, dsregcmd /join</span></span>

 2. <span data-ttu-id="b2067-128">Daugiau informacijos apie hibridinio sujungimo problemas ieškokite [įrenginių trikčių diagnostika](https://techcommunity.microsoft.com/t5/azure-active-directory-identity/azure-ad-mailbag-frequent-questions-about-using-device-based/ba-p/1257344).</span><span class="sxs-lookup"><span data-stu-id="b2067-128">For more details on Hybrid Join issues, see [Troubleshoot devices Issue](https://techcommunity.microsoft.com/t5/azure-active-directory-identity/azure-ad-mailbag-frequent-questions-about-using-device-based/ba-p/1257344).</span></span>
