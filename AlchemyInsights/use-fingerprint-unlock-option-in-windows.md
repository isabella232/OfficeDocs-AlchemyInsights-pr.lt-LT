---
title: Pirštų atspaudų atrakinimo parinkties naudojimas sistemoje "Windows 10"
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001689"
- "3765"
ms.openlocfilehash: 99f037f62748c06d77b526e35f67b711885c4a1e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 09/15/2020
ms.locfileid: "47795252"
---
# <a name="use-fingerprint-unlock-option-in-windows-10"></a><span data-ttu-id="37d62-102">Pirštų atspaudų atrakinimo parinkties naudojimas sistemoje "Windows 10"</span><span class="sxs-lookup"><span data-stu-id="37d62-102">Use fingerprint unlock option in Windows 10</span></span>

<span data-ttu-id="37d62-103">**"Windows Hello" piršto atspaudo įgalinimas**</span><span class="sxs-lookup"><span data-stu-id="37d62-103">**Enable Windows Hello Fingerprint**</span></span>

<span data-ttu-id="37d62-104">Jei norite atrakinti "Windows 10" naudodami pirštų atspaudus, turite nustatyti "Windows Hello" pirštų atspaudus, įtraukdami ("Windows" išmokę atpažinti) bent vieną pirštą.</span><span class="sxs-lookup"><span data-stu-id="37d62-104">To unlock Windows 10 using your fingerprint, you need to set up Windows Hello Fingerprint by adding (letting Windows learn to recognize) at least one finger.</span></span> 

1. <span data-ttu-id="37d62-105">Eikite į **parametrai > paskyros > prisijungimo parinktys** (arba spustelėkite [čia](ms-settings:signinoptions?activationSource=GetHelp)).</span><span class="sxs-lookup"><span data-stu-id="37d62-105">Go to **Settings  > Accounts > Sign-in options** (or click [here](ms-settings:signinoptions?activationSource=GetHelp)).</span></span> <span data-ttu-id="37d62-106">Bus įtrauktos galimos prisijungimo parinktys.</span><span class="sxs-lookup"><span data-stu-id="37d62-106">Available sign-in options will be listed.</span></span> <span data-ttu-id="37d62-107">Pavyzdžiui:</span><span class="sxs-lookup"><span data-stu-id="37d62-107">For example:</span></span>

    ![Prisijungimo parinktys.](media/sign-in-options.png)

2. <span data-ttu-id="37d62-109">Spustelėkite arba bakstelėkite **"Windows Hello" piršto atspaudas**, tada spustelėkite **nustatyti**.</span><span class="sxs-lookup"><span data-stu-id="37d62-109">Click or tap **Windows Hello Fingerprint**, then click **Set up**.</span></span> <span data-ttu-id="37d62-110">"Windows Hello" sąrankos **lange spustelėkite pradėti**.</span><span class="sxs-lookup"><span data-stu-id="37d62-110">In the Windows Hello setup window, click **Get started**.</span></span> <span data-ttu-id="37d62-111">Pirštų atspaudų jutiklis suaktyvinamas ir būsite paraginti įdėti pirštą ant jutiklio:</span><span class="sxs-lookup"><span data-stu-id="37d62-111">The fingerprint sensor will activate, and you'll be asked to place your finger on the sensor:</span></span>

   ![Pirštų atspaudų jutiklis.](media/fingerprint-sensor.png)

3. <span data-ttu-id="37d62-113">Vykdykite nurodymus, kurie paprašys pakartotinai nuskaityti pirštą.</span><span class="sxs-lookup"><span data-stu-id="37d62-113">Follow the instructions, which will ask you to repeatedly scan your finger.</span></span> <span data-ttu-id="37d62-114">Kai tai bus baigta, turėsite galimybę įtraukti kitų pirštų, kuriuos galbūt norėsite naudoti prisijungdami.</span><span class="sxs-lookup"><span data-stu-id="37d62-114">When this is finished, you'll have the option of adding other fingers you may want to use for sign-in.</span></span> <span data-ttu-id="37d62-115">Kai prisijungsite prie "Windows 10", turėsite galimybę naudoti pirštų atspaudus.</span><span class="sxs-lookup"><span data-stu-id="37d62-115">Next time you sign in to Windows 10, you will have the option of using your fingerprint to do so.</span></span>

<span data-ttu-id="37d62-116">**"Windows Hello" piršto atspaudas negalimas kaip prisijungimo parinktis**</span><span class="sxs-lookup"><span data-stu-id="37d62-116">**Windows Hello Fingerprint not available as a sign-in option**</span></span>

<span data-ttu-id="37d62-117">Jei "Windows Hello" kontrolinis kodas nerodomas kaip parinktis **prisijungimo parinktyse**, vadinasi, "Windows" nežino apie bet kokį pirštų atspaudų skaitytuvą/skaitytuvą, prijungtą prie jūsų kompiuterio, arba kad sistemos strategija neleidžia jos naudoti (pvz., jūsų kompiuterį tvarko jūsų darbo vieta).</span><span class="sxs-lookup"><span data-stu-id="37d62-117">If Windows Hello Fingerprint is not shown as an option in **Sign-in options**, it means Windows is not aware of any fingerprint reader/scanner attached to your PC, or that a system policy prevents its use (if for example your PC is managed by your workplace).</span></span> <span data-ttu-id="37d62-118">Norėdami pašalinti triktis:</span><span class="sxs-lookup"><span data-stu-id="37d62-118">To troubleshoot:</span></span> 

1. <span data-ttu-id="37d62-119">Pasirinkite mygtuką **Pradžia** užduočių juostoje ir ieškokite **įrenginių tvarkytuvė**.</span><span class="sxs-lookup"><span data-stu-id="37d62-119">Select the **Start** button in the Taskbar and search for **Device Manager**.</span></span>

2. <span data-ttu-id="37d62-120">Spustelėkite arba bakstelėkite, kad atidarytumėte **įrenginių tvarkytuvę**.</span><span class="sxs-lookup"><span data-stu-id="37d62-120">Click or tap to open **Device Manager**.</span></span>

3. <span data-ttu-id="37d62-121">Įrenginių tvarkytuvėje išplėskite biometrinius įrenginius spustelėdami jo ševroną.</span><span class="sxs-lookup"><span data-stu-id="37d62-121">In Device Manager, expand Biometric devices by clicking its chevron.</span></span>

   ![Biometriniai įrenginiai.](media/biometric-devices.png)

4. <span data-ttu-id="37d62-123">Jūsų pirštų atspaudų skaitytuvas turi būti pateiktas kaip biometrinis įrenginys, pvz., "Synaptics WBDI" skaitytuvas:</span><span class="sxs-lookup"><span data-stu-id="37d62-123">Your fingerprint scanner should be listed as a biometric device, such as the Synaptics WBDI scanner:</span></span>

   ![Biometriniai įrenginiai.](media/biometric-devices-expanded.png)

5. <span data-ttu-id="37d62-125">Jei jūsų pirštų atspaudų skaitytuvas nerodomas ir skaitytuvas integruotas į jūsų kompiuterį, eikite į kompiuterio gamintojo svetainę.</span><span class="sxs-lookup"><span data-stu-id="37d62-125">If your fingerprint scanner is not shown, and the scanner is integrated into your PC, go to the PC manufacturer's website.</span></span> <span data-ttu-id="37d62-126">KOMPIUTERIO modelio techninio palaikymo sekcijoje ieškokite "Windows 10" tvarkyklės, skirtos skaitytuvui, kurį galite įdiegti.</span><span class="sxs-lookup"><span data-stu-id="37d62-126">In the technical support section for your PC model, search for a Windows 10 driver for a scanner that you can install.</span></span>

6. <span data-ttu-id="37d62-127">Jei skaitytuvas yra atskirtas nuo asmeninio kompiuterio (pridėto per USB), eikite į skaitytuvo gamintojo svetainę ir raskite bei įdiekite "Windows 10" įrenginio tvarkyklės programinę įrangą, skirtą skaitytuvo modeliui.</span><span class="sxs-lookup"><span data-stu-id="37d62-127">If the scanner is separate from the PC (attached via USB), go to the scanner manufacturer's website to find and install Windows 10 device driver software for the scanner model you have.</span></span>
