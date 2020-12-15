---
title: Įrenginio laukiama būsena
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
- "9003244"
- "7319"
ms.openlocfilehash: f70b43a8b914b0d2dda9db61606b8ae24523f869
ms.sourcegitcommit: 097a8cabe0d2280af489159789988a0ab532dabb
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 12/11/2020
ms.locfileid: "49678485"
---
# <a name="device-in-pending-state"></a><span data-ttu-id="509df-102">Įrenginio laukiama būsena</span><span class="sxs-lookup"><span data-stu-id="509df-102">Device in pending state</span></span>

<span data-ttu-id="509df-103">**Būtinosios sąlygos**</span><span class="sxs-lookup"><span data-stu-id="509df-103">**Prerequisites:**</span></span>

1. <span data-ttu-id="509df-104">Jei pirmą kartą nustatote įrenginio registracijas, įsitikinkite, kad "Azure [Active Directory" ("Azure AD") peržiūrėjote Supažindinimas su įrenginių valdymu](https://docs.microsoft.com/azure/active-directory/devices/overview?WT.mc_id=Portal-Microsoft_Azure_Support) "Azure AD" ("Azure AD").</span><span class="sxs-lookup"><span data-stu-id="509df-104">If you are setting up device registrations for the first time, please ensure that you have reviewed [Introduction to device management in Azure Active Directory (Azure AD)](https://docs.microsoft.com/azure/active-directory/devices/overview?WT.mc_id=Portal-Microsoft_Azure_Support) that will guide you on how to get devices under the control of Azure AD.</span></span>
2. <span data-ttu-id="509df-105">Jei norite registruoti įrenginius į "Azure AD" tiesiogiai ir juos pateikti į "Intune", turite užtikrinti, kad [sukonfigūravote "Intune](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment?WT.mc_id=Portal-Microsoft_Azure_Support) " ir pirmiausia turite [licencijavimą](https://docs.microsoft.com/mem/intune/fundamentals/licenses-assign?WT.mc_id=Portal-Microsoft_Azure_Support) .</span><span class="sxs-lookup"><span data-stu-id="509df-105">If you are registering devices into Azure AD directly and enrolling them into Intune, you will need to ensure that you have [configured Intune](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment?WT.mc_id=Portal-Microsoft_Azure_Support) and have the [licensing](https://docs.microsoft.com/mem/intune/fundamentals/licenses-assign?WT.mc_id=Portal-Microsoft_Azure_Support) in place first.</span></span>
3. <span data-ttu-id="509df-106">Įsitikinkite, kad turite teisę atlikti operacijas "Azure AD" ir vietiniame skelbime.</span><span class="sxs-lookup"><span data-stu-id="509df-106">Ensure you are authorized to perform operations in Azure AD and on-premises AD.</span></span> <span data-ttu-id="509df-107">Tik visuotinis administratorius "Azure AD" gali valdyti įrenginio registravimų parametrus.</span><span class="sxs-lookup"><span data-stu-id="509df-107">Only a global administrator in Azure AD can manage settings for device registrations.</span></span> <span data-ttu-id="509df-108">Be to, jei nustatote automatines registracijas vietinėje "Active Directory", turite būti "Active Directory" ir AD FS (jei taikoma) administratorius.</span><span class="sxs-lookup"><span data-stu-id="509df-108">In addition, if you are setting up automatic registrations in your on-premises Active Directory, you will need to be an administrator of Active Directory and AD FS (if applicable).</span></span>

<span data-ttu-id="509df-109">Hibridinis "Azure AD" prisijungimo procesas reikalauja, kad įrenginiai būtų taikomi korporatyviniame tinkle.</span><span class="sxs-lookup"><span data-stu-id="509df-109">The hybrid Azure AD join registration process requires devices to be on corporate network.</span></span> <span data-ttu-id="509df-110">Jis taip pat veikia per VPN, tačiau yra tam tikrų apribojimų.</span><span class="sxs-lookup"><span data-stu-id="509df-110">It also works over VPN but there are some caveats to that.</span></span> <span data-ttu-id="509df-111">Mes girdėjome klientus, kuriems reikia pagalbos šalinant hibridinio "Azure AD" prisijungimo procesą pagal nuotolinio darbo aplinkybes.</span><span class="sxs-lookup"><span data-stu-id="509df-111">We have heard customers needing assistance with troubleshooting the hybrid Azure AD join registration process under remote work circumstances.</span></span>

<span data-ttu-id="509df-112">**Debesies autentifikavimo aplinka (naudojant "Azure AD" slaptažodžių maišos sinchronizavimą arba Pass-per autentifikavimą)**</span><span class="sxs-lookup"><span data-stu-id="509df-112">**Cloud authentication environment (using Azure AD password hash sync or pass-through authentication)**</span></span>

<span data-ttu-id="509df-113">Šis registracijos srautas taip pat žinomas kaip "sinchronizavimo sujungimas".</span><span class="sxs-lookup"><span data-stu-id="509df-113">This registration flow is also known as “Sync Join”.</span></span>

<span data-ttu-id="509df-114">Toliau aprašyta, kas nutinka registracijos proceso metu:</span><span class="sxs-lookup"><span data-stu-id="509df-114">Here is a breakdown of what happens during the registration process:</span></span>

1. <span data-ttu-id="509df-115">"Windows 10" aptinka tarnybos jungties taško (SCP) įrašą, kai vartotojas prisijungia prie įrenginio.</span><span class="sxs-lookup"><span data-stu-id="509df-115">Windows 10 discovers Service Connection Point (SCP) record when the user logs on to the device.</span></span>

    1. <span data-ttu-id="509df-116">Įrenginys pirmiausia bando gauti nuomotojo informaciją iš kliento "SCP" registre [HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD].</span><span class="sxs-lookup"><span data-stu-id="509df-116">The device first tries to retrieve tenant information from client-side SCP in registry [HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD].</span></span> <span data-ttu-id="509df-117">Daugiau informacijos ieškokite [dokumente](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control).</span><span class="sxs-lookup"><span data-stu-id="509df-117">For more information, see [document](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control).</span></span>
    1. <span data-ttu-id="509df-118">Jei nepavyksta, įrenginys palaiko ryšį su vietinio "Active Directory", kad gautų nuomotojo informaciją iš "SCP".</span><span class="sxs-lookup"><span data-stu-id="509df-118">If it fails, the device communicates with on-premises Active Directory to get tenant information from SCP.</span></span> <span data-ttu-id="509df-119">Norėdami patvirtinti, kad SCP būtų galima pateikti šį [dokumentą](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-manual#configure-a-service-connection-point).</span><span class="sxs-lookup"><span data-stu-id="509df-119">To verify SCP, refer this [document](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-manual#configure-a-service-connection-point).</span></span>

    > [!NOTE]
    > <span data-ttu-id="509df-120">Rekomenduojame įgalinti "Active Directory" SCP ir naudoti tik kliento "SCP" pradiniam patvirtinimui.</span><span class="sxs-lookup"><span data-stu-id="509df-120">We recommend enabling SCP in the Active Directory and only using client-side SCP for initial validation.</span></span>

2. <span data-ttu-id="509df-121">"Windows 10" bando palaikyti ryšį su "Azure AD" pagal sistemos kontekstą ir autentifikuoja save nuo "Azure AD".</span><span class="sxs-lookup"><span data-stu-id="509df-121">Windows 10 tries to communicate with Azure AD under the system context to authenticate itself against Azure AD.</span></span>

    <span data-ttu-id="509df-122">Galite patikrinti, ar įrenginys gali pasiekti "Microsoft" išteklius pagal sistemos paskyrą, naudodami [bandomojo įrenginio registracijos ryšio scenarijų](https://gallery.technet.microsoft.com/Test-Device-Registration-3dc944c0).</span><span class="sxs-lookup"><span data-stu-id="509df-122">You can verify if the device can access Microsoft resources under the system account by using the [Test Device Registration Connectivity script](https://gallery.technet.microsoft.com/Test-Device-Registration-3dc944c0).</span></span>

3. <span data-ttu-id="509df-123">"Windows 10" generuoja vartotojo pasirašomą sertifikatą ir saugo ją po kompiuterio objektu vietiniame "Active Directory".</span><span class="sxs-lookup"><span data-stu-id="509df-123">Windows 10 generates self-signed certificate and stores it under the computer object in on-premises Active Directory.</span></span> <span data-ttu-id="509df-124">Tam reikia, kad būtų matomas domeno valdiklis.</span><span class="sxs-lookup"><span data-stu-id="509df-124">This requires line-of-sight to Domain Controller.</span></span>

4. <span data-ttu-id="509df-125">Įrenginio objektas, turintis sertifikatą, bus sinchronizuotas su "Azure AD" naudojant "Azure AD Connect".</span><span class="sxs-lookup"><span data-stu-id="509df-125">Device object that has certificate gets synchronized to Azure AD via Azure AD Connect.</span></span> <span data-ttu-id="509df-126">Sinchronizavimo ciklas yra kas 30 minučių pagal numatytuosius parametrus, tačiau tai priklauso nuo "Azure AD Connect" konfigūracijos.</span><span class="sxs-lookup"><span data-stu-id="509df-126">Sync cycle is every 30 minutes by default, but it depends on the configuration of Azure AD Connect.</span></span> <span data-ttu-id="509df-127">Daugiau informacijos ieškokite šiame [dokumente](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sync-configure-filtering#organizational-unitbased-filtering).</span><span class="sxs-lookup"><span data-stu-id="509df-127">For more information, refer this [document](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sync-configure-filtering#organizational-unitbased-filtering).</span></span>

5. <span data-ttu-id="509df-128">Šiame etape jums turėtų būti suteikta galimybė matyti temos įrenginį "**laukianti**" būsena dalyje "Azure" portalo įrenginio peilis.</span><span class="sxs-lookup"><span data-stu-id="509df-128">At this stage, you should be able to see the subject device in “**Pending**” state under Device blade of Azure Portal.</span></span>

6. <span data-ttu-id="509df-129">Kitas vartotojas prisijungęs prie "Windows 10", registracija bus atlikta.</span><span class="sxs-lookup"><span data-stu-id="509df-129">At the next user login to Windows 10, the registration will be completed.</span></span>

    > [!NOTE]
    > <span data-ttu-id="509df-130">Jei esate VPN ir atsijungti/prisijungti nutraukia domeno ryšį, galite suaktyvinti registraciją neautomatiškai.</span><span class="sxs-lookup"><span data-stu-id="509df-130">If you are on VPN and logoff/login terminates the domain connectivity, you can trigger registration manually.</span></span> <span data-ttu-id="509df-131">Norėdami tai padaryti:</span><span class="sxs-lookup"><span data-stu-id="509df-131">To do that:</span></span>
    >
    > <span data-ttu-id="509df-132">`dsregcmd /join`Dėl administratoriaus raginimo arba nuotoliniu būdu per PSExec į kompiuterį problemą.</span><span class="sxs-lookup"><span data-stu-id="509df-132">Issue a `dsregcmd /join` locally on admin prompt or remotely via PSExec to your PC.</span></span>
    >
    > <span data-ttu-id="509df-133">Pavyzdžiui: `PsExec -s \\win10client01 cmd, dsregcmd /join`</span><span class="sxs-lookup"><span data-stu-id="509df-133">For example: `PsExec -s \\win10client01 cmd, dsregcmd /join`</span></span>

<span data-ttu-id="509df-134">Jei turite įprastas "Azure Active Directory" įrenginio registravimo problemas, peržiūrėkite [įrenginių DUK](https://docs.microsoft.com/azure/active-directory/devices/faq).</span><span class="sxs-lookup"><span data-stu-id="509df-134">For common issues with Azure Active Directory device registration, see [Devices FAQ](https://docs.microsoft.com/azure/active-directory/devices/faq).</span></span>
