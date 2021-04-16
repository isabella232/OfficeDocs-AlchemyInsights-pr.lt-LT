---
title: Pirštų atspaudų atrakinimo parinkties naudojimas "Windows 10"
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001689"
- "3765"
ms.openlocfilehash: ba1f2e7b0bb54e89178a320b8579b8d1bfdaff9a
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 04/15/2021
ms.locfileid: "51796685"
---
# <a name="use-fingerprint-unlock-option-in-windows-10"></a><span data-ttu-id="a2a25-102">Pirštų atspaudų atrakinimo parinkties naudojimas "Windows 10"</span><span class="sxs-lookup"><span data-stu-id="a2a25-102">Use fingerprint unlock option in Windows 10</span></span>

<span data-ttu-id="a2a25-103">**"Windows Hello" piršto atspaudo įgalinkite**</span><span class="sxs-lookup"><span data-stu-id="a2a25-103">**Enable Windows Hello Fingerprint**</span></span>

<span data-ttu-id="a2a25-104">Norėdami atrakinti "Windows 10" naudodami piršto atspaudą, turite nustatyti "Windows Hello Fingerprint" įtraukdami (leisdami "Windows" išmokti atpažinti) bent vienu pirštu.</span><span class="sxs-lookup"><span data-stu-id="a2a25-104">To unlock Windows 10 using your fingerprint, you need to set up Windows Hello Fingerprint by adding (letting Windows learn to recognize) at least one finger.</span></span> 

1. <span data-ttu-id="a2a25-105">Eikite **į Parametrai > Paskyros > prisijungimo parinktys** (arba spustelėkite [čia](ms-settings:signinoptions?activationSource=GetHelp)).</span><span class="sxs-lookup"><span data-stu-id="a2a25-105">Go to **Settings  > Accounts > Sign-in options** (or click [here](ms-settings:signinoptions?activationSource=GetHelp)).</span></span> <span data-ttu-id="a2a25-106">Bus išvardytos galimos prisijungimo parinktys.</span><span class="sxs-lookup"><span data-stu-id="a2a25-106">Available sign-in options will be listed.</span></span> <span data-ttu-id="a2a25-107">Toliau pateikiami pavyzdžiai.</span><span class="sxs-lookup"><span data-stu-id="a2a25-107">For example:</span></span>

    ![Prisijungimo parinktys.](media/sign-in-options.png)

2. <span data-ttu-id="a2a25-109">Spustelėkite arba bakstelėkite **"Windows Hello Fingerprint"**, tada **spustelėkite Nustatyti**.</span><span class="sxs-lookup"><span data-stu-id="a2a25-109">Click or tap **Windows Hello Fingerprint**, then click **Set up**.</span></span> <span data-ttu-id="a2a25-110">Lange "Windows Hello" sąranka spustelėkite **Darbo pradžia**.</span><span class="sxs-lookup"><span data-stu-id="a2a25-110">In the Windows Hello setup window, click **Get started**.</span></span> <span data-ttu-id="a2a25-111">Pirštų atspaudų jutiklis suaktyvins ir būsite paprašyti pirštu padėti ant jutiklio:</span><span class="sxs-lookup"><span data-stu-id="a2a25-111">The fingerprint sensor will activate, and you'll be asked to place your finger on the sensor:</span></span>

   ![Pirštų atspaudų jutiklis.](media/fingerprint-sensor.png)

3. <span data-ttu-id="a2a25-113">Vykdykite nurodymus, kuriuose bus nurodyta pakartotinai nuskaityti pirštą.</span><span class="sxs-lookup"><span data-stu-id="a2a25-113">Follow the instructions, which will ask you to repeatedly scan your finger.</span></span> <span data-ttu-id="a2a25-114">Kai tai bus baigta, galėsite įtraukti kitų pirštų, kuriuos galbūt norėsite naudoti prisijungdami.</span><span class="sxs-lookup"><span data-stu-id="a2a25-114">When this is finished, you'll have the option of adding other fingers you may want to use for sign-in.</span></span> <span data-ttu-id="a2a25-115">Kai kitą kartą prisijungsite prie "Windows 10", turėsite galimybę naudoti pirštų atspaudą.</span><span class="sxs-lookup"><span data-stu-id="a2a25-115">Next time you sign in to Windows 10, you will have the option of using your fingerprint to do so.</span></span>

<span data-ttu-id="a2a25-116">**"Windows Hello Fingerprint" nėra kaip prisijungimo parinktis**</span><span class="sxs-lookup"><span data-stu-id="a2a25-116">**Windows Hello Fingerprint not available as a sign-in option**</span></span>

<span data-ttu-id="a2a25-117">Jei "Windows Hello Fingerprint" nėra rodoma kaip parinktis prisijungimo parinktyse, tai reiškia, kad "Windows" nežino apie pirštų atspaudų skaitytuvą / skaitytuvą, pridėtą prie jūsų kompiuterio, arba kad sistemos strategija neleidžia jo naudoti (pvz., jei jūsų kompiuterį valdo jūsų darbovietė).</span><span class="sxs-lookup"><span data-stu-id="a2a25-117">If Windows Hello Fingerprint is not shown as an option in **Sign-in options**, it means Windows is not aware of any fingerprint reader/scanner attached to your PC, or that a system policy prevents its use (if for example your PC is managed by your workplace).</span></span> <span data-ttu-id="a2a25-118">Norėdami šalinti triktis:</span><span class="sxs-lookup"><span data-stu-id="a2a25-118">To troubleshoot:</span></span> 

1. <span data-ttu-id="a2a25-119">Užduočių **juostoje pasirinkite** mygtuką Pradžia ir ieškokite Įrenginių **tvarkytuvė.**</span><span class="sxs-lookup"><span data-stu-id="a2a25-119">Select the **Start** button in the Taskbar and search for **Device Manager**.</span></span>

2. <span data-ttu-id="a2a25-120">Spustelėkite arba bakstelėkite, kad atidarytumėte **įrenginių tvarkytuvę.**</span><span class="sxs-lookup"><span data-stu-id="a2a25-120">Click or tap to open **Device Manager**.</span></span>

3. <span data-ttu-id="a2a25-121">Įrenginių tvarkytuvėje išplėskite Biometriniai įrenginiai spustelėdami savo "v" pavidalo.</span><span class="sxs-lookup"><span data-stu-id="a2a25-121">In Device Manager, expand Biometric devices by clicking its chevron.</span></span>

   ![Biometriniai įrenginiai.](media/biometric-devices.png)

4. <span data-ttu-id="a2a25-123">Jūsų pirštų atspaudų skaitytuvas turi būti nurodytas kaip biometrinis įrenginys, pvz., "Synaptics WBDI" skaitytuvas:</span><span class="sxs-lookup"><span data-stu-id="a2a25-123">Your fingerprint scanner should be listed as a biometric device, such as the Synaptics WBDI scanner:</span></span>

   ![Biometriniai įrenginiai.](media/biometric-devices-expanded.png)

5. <span data-ttu-id="a2a25-125">Jei pirštų atspaudų skaitytuvas nerodomas ir skaitytuvas integruotas į jūsų kompiuterį, eikite į kompiuterio gamintojo svetainę.</span><span class="sxs-lookup"><span data-stu-id="a2a25-125">If your fingerprint scanner is not shown, and the scanner is integrated into your PC, go to the PC manufacturer's website.</span></span> <span data-ttu-id="a2a25-126">Kompiuterio modelio techninio palaikymo skyriuje ieškokite skaitytuvo, kurį galite įdiegti, "Windows 10" tvarkyklės.</span><span class="sxs-lookup"><span data-stu-id="a2a25-126">In the technical support section for your PC model, search for a Windows 10 driver for a scanner that you can install.</span></span>

6. <span data-ttu-id="a2a25-127">Jei skaitytuvas yra atskirtas nuo kompiuterio (pridėto per USB), eikite į skaitytuvo gamintojo svetainę, kad rastumėte ir įdiegtumėte "Windows 10" įrenginio tvarkyklės programinę įrangą, skirtą jūsų turimo skaitytuvo modeliui.</span><span class="sxs-lookup"><span data-stu-id="a2a25-127">If the scanner is separate from the PC (attached via USB), go to the scanner manufacturer's website to find and install Windows 10 device driver software for the scanner model you have.</span></span>
