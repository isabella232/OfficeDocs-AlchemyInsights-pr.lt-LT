---
title: Prisijungimo prie "Microsoft 365" programų problemos
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
- "9000571"
- "2559"
ms.openlocfilehash: c64cf2c9dbf63caad22e54ae801adc3ed8ff0f62
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 04/15/2021
ms.locfileid: "51833012"
---
# <a name="fixing-the-microsoft-365-apps-your-computers-trusted-platform-module-is-not-functioning-properly-message"></a><span data-ttu-id="db8e4-102">Pranešimas "Microsoft 365" programų "Jūsų kompiuterio patikimos platformos modulis veikia netinkamai" taisymas</span><span class="sxs-lookup"><span data-stu-id="db8e4-102">Fixing the Microsoft 365 apps "Your computer's Trusted Platform module is not functioning properly" message</span></span>

<span data-ttu-id="db8e4-103">Norėdami pašalinti šią klaidą, atlikite šiuos veiksmus:</span><span class="sxs-lookup"><span data-stu-id="db8e4-103">To fix this error, try the following:</span></span>

- <span data-ttu-id="db8e4-104">Įdiekite naujausius ["Windows" ir "Office"](https://support.microsoft.com/help/4027667/windows-10-update) [naujinimus.](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5)</span><span class="sxs-lookup"><span data-stu-id="db8e4-104">Install the latest updates for [Windows](https://support.microsoft.com/help/4027667/windows-10-update) and [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).</span></span>
- <span data-ttu-id="db8e4-105">[Išvalykite "Office"](https://docs.microsoft.com/office/troubleshoot/office-suite-issues/another-account-already-signed-in#step-4-clear-cached-credentials-on-the-computer) kredencialus naudodami "Windows" kredencialų tvarkytuvą.</span><span class="sxs-lookup"><span data-stu-id="db8e4-105">[Clear Office credentials](https://docs.microsoft.com/office/troubleshoot/office-suite-issues/another-account-already-signed-in#step-4-clear-cached-credentials-on-the-computer) using Windows Credential Manager.</span></span><br/>
    <span data-ttu-id="db8e4-106">**Pastaba:** "Office 2016" registro keliai pakeisti į 16.0.</span><span class="sxs-lookup"><span data-stu-id="db8e4-106">**Note:** The registry paths for Office 2016 have changed to 16.0.</span></span> <span data-ttu-id="db8e4-107">(pvz.: \Software\Microsoft\Office\16.0\Common\Identity\)</span><span class="sxs-lookup"><span data-stu-id="db8e4-107">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span></span>
- <span data-ttu-id="db8e4-108">Išbandykite [vartotojo atkūrimo procesą,](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) kad išspręstų patikimos platformos modulio (TPM) triktis.</span><span class="sxs-lookup"><span data-stu-id="db8e4-108">Try the [user recovery process](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) to fix Trusted Platform Module (TPM) failures.</span></span>
- <span data-ttu-id="db8e4-109">Nustatykite EnableADAL = 0, atlikite šiuos veiksmus:</span><span class="sxs-lookup"><span data-stu-id="db8e4-109">Set the EnableADAL = 0 using the following steps:</span></span>  
    1. <span data-ttu-id="db8e4-110">Dešiniuoju pelės mygtuku spustelėkite "Windows" mygtuką Pradžia, **pasirinkite Vykdyti**, **įveskite regedit**, tada pasirinkite **Gerai**.</span><span class="sxs-lookup"><span data-stu-id="db8e4-110">Right-click the Windows Start button, choose **Run**, type **regedit**, and then choose **OK**.</span></span>
    2. <span data-ttu-id="db8e4-111">Pasirinkite **Taip,** kad registro rengyklė galėtų atlikti įrenginio keitimus.</span><span class="sxs-lookup"><span data-stu-id="db8e4-111">Select **Yes** to allow Registry Editor to make changes to your device.</span></span>
    3. <span data-ttu-id="db8e4-112">Registro rengyklėje įtraukite **"EnableADAL"** DWORD reikšmę su **parametru 0 dalyje** HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\Identity.</span><span class="sxs-lookup"><span data-stu-id="db8e4-112">In Registry Editor, add a DWORD value of **EnableADAL** with a setting of **0** under HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\Identity.</span></span>

<span data-ttu-id="db8e4-113">Daugiau informacijos žr. Prisijungimo problemos atnaujinus į ["Office 2016" komponavimo versiją 16.0.7967 sistemoje "Windows 10".](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016)</span><span class="sxs-lookup"><span data-stu-id="db8e4-113">For more information, see [Connection issues in sign-in after update to Office 2016 build 16.0.7967 on Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).</span></span>