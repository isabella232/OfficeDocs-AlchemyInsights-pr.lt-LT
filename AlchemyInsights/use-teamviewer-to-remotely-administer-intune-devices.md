---
title: "\"TeamViewer\" naudojimas nuotoliniu būdu administruoti \"Intune\" įrenginius"
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1284"
- "6700008"
ms.openlocfilehash: 63e7f068f3c53240ad13d1679df460c97a1a94f4
ms.sourcegitcommit: 0e50dfcdb3f6aa72368279e23b83efecb9dc9c3f
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 07/28/2020
ms.locfileid: "46555242"
---
# <a name="use-teamviewer-to-remotely-administer-intune-devices"></a><span data-ttu-id="7c5b1-102">"TeamViewer" naudojimas nuotoliniu būdu administruoti "Intune" įrenginius</span><span class="sxs-lookup"><span data-stu-id="7c5b1-102">Use TeamViewer to remotely administer Intune devices</span></span>

<span data-ttu-id="7c5b1-103">"Intune" valdomi įrenginiai gali būti administruojami nuotoliniu būdu naudojant ["TeamViewer".](https://www.teamviewer.com/)</span><span class="sxs-lookup"><span data-stu-id="7c5b1-103">Devices managed by Intune can be administered remotely by using [TeamViewer](https://www.teamviewer.com/).</span></span>

<span data-ttu-id="7c5b1-104">Norėdami administruoti "Intune" naudodami "TeamViewer", atlikite šiuos veiksmus:</span><span class="sxs-lookup"><span data-stu-id="7c5b1-104">To administer Intune by using TeamViewer, use these steps:</span></span> 

<span data-ttu-id="7c5b1-105">Pradėkite gaudami kredencialus iš "TeamViewer", kad nustatytumėte "TeamViewer Connector" intune.</span><span class="sxs-lookup"><span data-stu-id="7c5b1-105">Begin by obtaining credentials from TeamViewer to set up the TeamViewer Connector on Intune.</span></span> <span data-ttu-id="7c5b1-106">Tai leidžia administratoriui įvesti kredencialus "TeamViewer Connector" vartotojo sąsajoje įrenginiai, vienkartinė operacija, siekiant nustatyti ryšį tarp "Intune" ir "TeamViewer" paslaugos.</span><span class="sxs-lookup"><span data-stu-id="7c5b1-106">This allows the admin to enter credentials in the TeamViewer Connector UI under Devices, a one-time operation to establish the link between Intune and the TeamViewer service.</span></span>

<span data-ttu-id="7c5b1-107">**1 dalis: pradėkite seansą naudodami nuotolinį įrenginį**</span><span class="sxs-lookup"><span data-stu-id="7c5b1-107">**Part 1: Start a session with a remote device**</span></span>

1. <span data-ttu-id="7c5b1-108">Dalyje **Visi įrenginiai**pasirinkite įrenginį, su kuriuo norite pradėti nuotolinį seansą.</span><span class="sxs-lookup"><span data-stu-id="7c5b1-108">Under **All devices**, select the device you want to start a remote session with.</span></span>
2. <span data-ttu-id="7c5b1-109">Nuo **... Daugiau**, pasirinkite **Naujas nuotolinės pagalbos seansas**.</span><span class="sxs-lookup"><span data-stu-id="7c5b1-109">From  **…More**, select **New remote assistance session**.</span></span>
3. <span data-ttu-id="7c5b1-110">Pasirinkite **Taip,** kad patvirtintumėte, jog norite nustatyti nuotolinį seansą.</span><span class="sxs-lookup"><span data-stu-id="7c5b1-110">Select **Yes** to acknowledge you want to establish a remote session.</span></span>
    <span data-ttu-id="7c5b1-111">"TeamViewer" tarnybai patvirtinus užklausą "Pradėti naują nuotolinį seansą", įrenginio apžvalgos (arba "Essentials") srityje matysite parinktį **Pradėti nuotolinę pagalbą.**</span><span class="sxs-lookup"><span data-stu-id="7c5b1-111">After the "Initiating a new remote session" request is acknowledged by the TeamViewer service, you'll see an option to **Start remote assistance** under the details of the Overview (or, Essentials) pane for the device.</span></span> <span data-ttu-id="7c5b1-112">Pasirinkite **Žiūrėti daugiau,** kad išplėstumėte sritį ir parodytumėte nuotolinės pagalbos būseną.</span><span class="sxs-lookup"><span data-stu-id="7c5b1-112">Select **See More** to expand the pane and show the Remote Assistance status.</span></span>
4. <span data-ttu-id="7c5b1-113">Pasirinkite **Pradėti nuotolinį seansą,** kad inicijuotumėte seansą administratoriaus pusėje.</span><span class="sxs-lookup"><span data-stu-id="7c5b1-113">Select **Start remote session** to initiate the session on the admin side.</span></span>
5. <span data-ttu-id="7c5b1-114">Pasirinkite atsisiųsti "TeamViewer" dvejetainį ("Windows") ir pasirinkite **Vykdyti**.</span><span class="sxs-lookup"><span data-stu-id="7c5b1-114">Choose to download the TeamViewer binary (Windows), and select **Run**.</span></span><br/>
    <span data-ttu-id="7c5b1-115">**Pastaba** Galite nepaisyti bet kurio žiniatinklio naršyklės puslapio, atidaryto "TeamViewer" svetainėje.</span><span class="sxs-lookup"><span data-stu-id="7c5b1-115">**Note** You can ignore any web browser page opened to the TeamViewer web site.</span></span>

6. <span data-ttu-id="7c5b1-116">Patvirtinkite "TeamViewer" programėlės prašymą atlikti pakeitimus įrenginyje (tik "Windows").</span><span class="sxs-lookup"><span data-stu-id="7c5b1-116">Acknowledge the request for the TeamViewer app to make changes on the device (Windows only).</span></span>
7. <span data-ttu-id="7c5b1-117">Paleidžiama "TeamViewer" programa, į kurią įtraukiamas seanso kodas, skirtas ryšio su nuotoliniu įrenginiu autentifikuoti.</span><span class="sxs-lookup"><span data-stu-id="7c5b1-117">The TeamViewer app starts and includes the session code to authenticate the connection with the remote device.</span></span>

<span data-ttu-id="7c5b1-118">**2 dalis: Įrenginyje, skirtame nuotoliniam seansui**</span><span class="sxs-lookup"><span data-stu-id="7c5b1-118">**Part 2: On the device being targeted for a remote session**</span></span>

1. <span data-ttu-id="7c5b1-119">Atidarykite įmonės portalą Intune.</span><span class="sxs-lookup"><span data-stu-id="7c5b1-119">Open the Intune company portal.</span></span>
2. <span data-ttu-id="7c5b1-120">Ieškokite pranešimo vėliavėlės: "Jūsų IT administratorius prašo valdyti šį įrenginį nuotolinės pagalbos seansui", ir pasirinkite pranešimą.</span><span class="sxs-lookup"><span data-stu-id="7c5b1-120">Look for a notification flag: "Your IT administrator is requesting control of this device for a remote assistance session," and select the notification.</span></span>
3. <span data-ttu-id="7c5b1-121">Pasirinkite atsisiųsti "TeamViewer" programą arba patvirtinti "TeamViewer" programos atsisiuntimą iš programų parduotuvės ir pasirinkite **Vykdyti**.</span><span class="sxs-lookup"><span data-stu-id="7c5b1-121">Choose to download the TeamViewer application, or acknowledge download of the TeamViewer app from the app store, and select **Run**.</span></span>
    <span data-ttu-id="7c5b1-122">**Pastaba** Galite nepaisyti bet kurio žiniatinklio naršyklės puslapio, atidaryto "TeamViewer" svetainėje.</span><span class="sxs-lookup"><span data-stu-id="7c5b1-122">**Note** You can ignore any web browser page opened to the TeamViewer web site.</span></span>

4. <span data-ttu-id="7c5b1-123">Patvirtinkite "TeamViewer" programėlės prašymą atlikti pakeitimus įrenginyje (tik "Windows").</span><span class="sxs-lookup"><span data-stu-id="7c5b1-123">Acknowledge the request for the TeamViewer app to make changes on the device (Windows only).</span></span>
5. <span data-ttu-id="7c5b1-124">Paleidžiama "TeamViewer" programa, į kurią įtraukiamas seanso kodas, skirtas ryšio su nuotoliniu įrenginiu autentifikuoti.</span><span class="sxs-lookup"><span data-stu-id="7c5b1-124">The TeamViewer app starts and includes the session code to authenticate the connection with the remote device.</span></span>
6. <span data-ttu-id="7c5b1-125">Iššokantis langas klausia, ar norite leisti pradėti seansą.</span><span class="sxs-lookup"><span data-stu-id="7c5b1-125">A popup asks if you want to allow the session to start.</span></span>

<span data-ttu-id="7c5b1-126">**Pastaba** "TeamViewer" tarnybos sugeneruoti seanso kodai naudojami tik vieną kartą.</span><span class="sxs-lookup"><span data-stu-id="7c5b1-126">**Note** The session codes generated by the TeamViewer service are one-time use only.</span></span> <span data-ttu-id="7c5b1-127">Jei prarasite ryšį, turite:</span><span class="sxs-lookup"><span data-stu-id="7c5b1-127">If you lose the connection, you must:</span></span>

1. <span data-ttu-id="7c5b1-128">Uždarykite "TeamViewer" programos egzempliorių nuotoliniame įrenginyje ir administratoriaus darbo vietoje.</span><span class="sxs-lookup"><span data-stu-id="7c5b1-128">Close the instance of the TeamViewer app on the remote device and on the admin workstation.</span></span>
2. <span data-ttu-id="7c5b1-129">Uždarykite nuotolinio įrenginio įmonės portalą.</span><span class="sxs-lookup"><span data-stu-id="7c5b1-129">Close the company portal on the remote device.</span></span>
3. <span data-ttu-id="7c5b1-130">Inicijuoti naują "Naują nuotolinės pagalbos seansą" iš administravimo portalo.</span><span class="sxs-lookup"><span data-stu-id="7c5b1-130">Initiate a new "New remote Assistance session" from the admin portal.</span></span>
4. <span data-ttu-id="7c5b1-131">Iš naujo atidarykite nuotolinio įrenginio įmonės portalą, kad gautumėte naują pranešimą.</span><span class="sxs-lookup"><span data-stu-id="7c5b1-131">Re-open the company portal on the remote device to receive the new notification.</span></span>
5. <span data-ttu-id="7c5b1-132">Atsisiųskite ir atidarykite "TeamViewer" programą nuotoliniame įrenginyje ir administratoriaus darbo vietoje, kaip ir anksčiau.</span><span class="sxs-lookup"><span data-stu-id="7c5b1-132">Download and open the TeamViewer app on both the remote device and the admin workstation, as before.</span></span>