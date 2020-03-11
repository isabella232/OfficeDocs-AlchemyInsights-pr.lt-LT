---
title: Pirštų atspaudų atrakinimo parinkties naudojimas sistemoje "Windows 10"
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001689"
- "3765"
ms.openlocfilehash: 8a5059c722c306ad79811140062cec7f52f31766
ms.sourcegitcommit: 00e4266575438f55bdc18db05ed54aafcb75a3c9
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 03/11/2020
ms.locfileid: "42588323"
---
# <a name="use-fingerprint-unlock-option-in-windows-10"></a><span data-ttu-id="8491e-102">Pirštų atspaudų atrakinimo parinkties naudojimas sistemoje "Windows 10"</span><span class="sxs-lookup"><span data-stu-id="8491e-102">Use fingerprint unlock option in Windows 10</span></span>

<span data-ttu-id="8491e-103">**Įgalinti "Windows Hello" piršto atspaudą**</span><span class="sxs-lookup"><span data-stu-id="8491e-103">**Enable Windows Hello Fingerprint**</span></span>

<span data-ttu-id="8491e-104">Norėdami atrakinti "Windows 10" naudodami piršto atspaudą, turite nustatyti "Windows Hello" pirštų atspaudą pridėdami (leisdami "Windows išmokti atpažinti") bent vienu pirštu.</span><span class="sxs-lookup"><span data-stu-id="8491e-104">To unlock Windows 10 using your fingerprint, you need to set up Windows Hello Fingerprint by adding (letting Windows learn to recognize) at least one finger.</span></span> 

1. <span data-ttu-id="8491e-105">Eikite į **Parametrai > Paskyros > prisijungimo parinktys** (arba spustelėkite [čia](ms-settings:signinoptions?activationSource=GetHelp)).</span><span class="sxs-lookup"><span data-stu-id="8491e-105">Go to **Settings  > Accounts > Sign-in options** (or click [here](ms-settings:signinoptions?activationSource=GetHelp)).</span></span> <span data-ttu-id="8491e-106">Bus išvardytos galimos prisijungimo parinktys.</span><span class="sxs-lookup"><span data-stu-id="8491e-106">Available sign-in options will be listed.</span></span> <span data-ttu-id="8491e-107">Pavyzdžiui:</span><span class="sxs-lookup"><span data-stu-id="8491e-107">For example:</span></span>

    ![Prisijungimo parinktys.](media/sign-in-options.png)

2. <span data-ttu-id="8491e-109">Spustelėkite arba bakstelėkite **"Windows Hello" pirštų atspaudas**, tada spustelėkite **Nustatyti**.</span><span class="sxs-lookup"><span data-stu-id="8491e-109">Click or tap **Windows Hello Fingerprint**, then click **Set up**.</span></span> <span data-ttu-id="8491e-110">"Windows Hello" sąrankos lange spustelėkite **Pradėti**.</span><span class="sxs-lookup"><span data-stu-id="8491e-110">In the Windows Hello setup window, click **Get started**.</span></span> <span data-ttu-id="8491e-111">Pirštų atspaudų jutiklis įsijungs, o jūsų bus paprašyta pirštu padėti ant jutiklio:</span><span class="sxs-lookup"><span data-stu-id="8491e-111">The fingerprint sensor will activate, and you'll be asked to place your finger on the sensor:</span></span>

   ![Pirštų atspaudų jutiklis.](media/fingerprint-sensor.png)

3. <span data-ttu-id="8491e-113">Vykdykite nurodymus, kurie paprašys pakartotinai nuskaityti pirštą.</span><span class="sxs-lookup"><span data-stu-id="8491e-113">Follow the instructions, which will ask you to repeatedly scan your finger.</span></span> <span data-ttu-id="8491e-114">Kai tai bus baigta, turėsite galimybę pridėti kitus pirštus, kuriuos galbūt norėsite naudoti prisijungdami.</span><span class="sxs-lookup"><span data-stu-id="8491e-114">When this is finished, you'll have the option of adding other fingers you may want to use for sign-in.</span></span> <span data-ttu-id="8491e-115">Kai kitą kartą prisijungsite prie "Windows 10", turėsite galimybę naudoti piršto atspaudą.</span><span class="sxs-lookup"><span data-stu-id="8491e-115">Next time you sign in to Windows 10, you will have the option of using your fingerprint to do so.</span></span>

<span data-ttu-id="8491e-116">**"Windows Hello" pirštų atspaudų negalima kaip prisijungimo parinktis**</span><span class="sxs-lookup"><span data-stu-id="8491e-116">**Windows Hello Fingerprint not available as a sign-in option**</span></span>

<span data-ttu-id="8491e-117">Jei **prisijungimo parinktyse**"Windows Hello" pirštų atspaudų nėra rodoma kaip parinktis, tai reiškia, kad "Windows" nežino jokio prie kompiuterio prijungto pirštų atspaudų skaitytuvo / skaitytuvo arba kad sistemos strategija neleidžia jo naudoti (pvz., jūsų kompiuterį valdo jūsų darbo vieta).</span><span class="sxs-lookup"><span data-stu-id="8491e-117">If Windows Hello Fingerprint is not shown as an option in **Sign-in options**, it means Windows is not aware of any fingerprint reader/scanner attached to your PC, or that a system policy prevents its use (if for example your PC is managed by your workplace).</span></span> <span data-ttu-id="8491e-118">Norėdami pašalinti:</span><span class="sxs-lookup"><span data-stu-id="8491e-118">To troubleshoot:</span></span> 

1. <span data-ttu-id="8491e-119">Užduočių \*\*\*\* juostoje pasirinkite pradžios mygtuką ir ieškokite **Įrenginių tvarkytuvės**.</span><span class="sxs-lookup"><span data-stu-id="8491e-119">Select the **Start** button in the Taskbar and search for **Device Manager**.</span></span>

2. <span data-ttu-id="8491e-120">Spustelėkite arba bakstelėkite , kad atidarytumėte **įrenginių tvarkytuvę**.</span><span class="sxs-lookup"><span data-stu-id="8491e-120">Click or tap to open **Device Manager**.</span></span>

3. <span data-ttu-id="8491e-121">Įrenginių tvarkytuvėje išplėskite Biometriniai įrenginiai spustelėdami jo ševroną.</span><span class="sxs-lookup"><span data-stu-id="8491e-121">In Device Manager, expand Biometric devices by clicking its chevron.</span></span>

   ![Biometriniai prietaisai.](media/biometric-devices.png)

4. <span data-ttu-id="8491e-123">Pirštų atspaudų skaitytuvas turi būti nurodytas kaip biometrinis įrenginys, pvz., Synaptics WBDI skaitytuvas:</span><span class="sxs-lookup"><span data-stu-id="8491e-123">Your fingerprint scanner should be listed as a biometric device, such as the Synaptics WBDI scanner:</span></span>

   ![Biometriniai prietaisai.](media/biometric-devices-expanded.png)

5. <span data-ttu-id="8491e-125">Jei pirštų atspaudų skaitytuvas nerodomas ir skaitytuvas integruotas į kompiuterį, eikite į kompiuterio gamintojo svetainę.</span><span class="sxs-lookup"><span data-stu-id="8491e-125">If your fingerprint scanner is not shown, and the scanner is integrated into your PC, go to the PC manufacturer's website.</span></span> <span data-ttu-id="8491e-126">Kompiuterio modelio techninio palaikymo skyriuje ieškokite skaitytuvo, kurį galite įdiegti, "Windows 10" tvarkyklės.</span><span class="sxs-lookup"><span data-stu-id="8491e-126">In the technical support section for your PC model, search for a Windows 10 driver for a scanner that you can install.</span></span>

6. <span data-ttu-id="8491e-127">Jei skaitytuvas yra atskirtas nuo kompiuterio (prijungtas per USB), eikite į skaitytuvo gamintojo svetainę ir raskite ir įdiekite "Windows 10" įrenginio tvarkyklės programinę įrangą, skirtą jūsų skaitytuvo modeliui.</span><span class="sxs-lookup"><span data-stu-id="8491e-127">If the scanner is separate from the PC (attached via USB), go to the scanner manufacturer's website to find and install Windows 10 device driver software for the scanner model you have.</span></span>
