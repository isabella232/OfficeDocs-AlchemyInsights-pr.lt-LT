---
title: Prisijungimo prie "Microsoft 365" programėlių problemos
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000571"
- "2559"
ms.openlocfilehash: 4e7612562d036f1c717817d3c883d6df80f86e2f
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 06/05/2020
ms.locfileid: "44579873"
---
# <a name="fixing-the-microsoft-365-apps-your-computers-trusted-platform-module-is-not-functioning-properly-message"></a><span data-ttu-id="b13b4-102">"Microsoft 365" programėlių "Kompiuterio patikimos platformos modulis veikia netinkamai" nustatymas</span><span class="sxs-lookup"><span data-stu-id="b13b4-102">Fixing the Microsoft 365 apps "Your computer's Trusted Platform module is not functioning properly" message</span></span>

<span data-ttu-id="b13b4-103">Norėdami pašalinti šią klaidą, atlikite šiuos veiksmus:</span><span class="sxs-lookup"><span data-stu-id="b13b4-103">To fix this error, try the following:</span></span>

- <span data-ttu-id="b13b4-104">Įdiekite naujausius ["Windows"](https://support.microsoft.com/help/4027667/windows-10-update) ir ["Office"](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5)naujinimus .</span><span class="sxs-lookup"><span data-stu-id="b13b4-104">Install the latest updates for [Windows](https://support.microsoft.com/help/4027667/windows-10-update) and [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).</span></span>
- <span data-ttu-id="b13b4-105">[Išvalykite "Office" kredencialus](https://docs.microsoft.com/eoffice/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) naudodami "Windows" kredencialų tvarkytuvą.</span><span class="sxs-lookup"><span data-stu-id="b13b4-105">[Clear Office credentials](https://docs.microsoft.com/eoffice/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) using Windows Credential Manager.</span></span><br/>
    <span data-ttu-id="b13b4-106">**Pastaba:** Registro keliai Office 2016 pasikeitė į 16.0.</span><span class="sxs-lookup"><span data-stu-id="b13b4-106">**Note:** The registry paths for Office 2016 have changed to 16.0.</span></span> <span data-ttu-id="b13b4-107">(Pvz.: \Software\Microsoft\Office\16.0\Common\Identity\)</span><span class="sxs-lookup"><span data-stu-id="b13b4-107">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span></span>
- <span data-ttu-id="b13b4-108">Pabandykite [vartotojo atkūrimo procesą,](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) norėdami išspręsti patikimos platformos modulio (TPM) triktys.</span><span class="sxs-lookup"><span data-stu-id="b13b4-108">Try the [user recovery process](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) to fix Trusted Platform Module (TPM) failures.</span></span>
- <span data-ttu-id="b13b4-109">Nustatykite EnableADAL = 0 atlikdami šiuos veiksmus:</span><span class="sxs-lookup"><span data-stu-id="b13b4-109">Set the EnableADAL = 0 using the following steps:</span></span>  
    1. <span data-ttu-id="b13b4-110">Dešiniuoju pelės mygtuku spustelėkite mygtuką Windows pradėti, pasirinkite **Vykdyti**, įveskite **regedit**, tada pasirinkite **Gerai**.</span><span class="sxs-lookup"><span data-stu-id="b13b4-110">Right-click the Windows Start button, choose **Run**, type **regedit**, and then choose **OK**.</span></span>
    2. <span data-ttu-id="b13b4-111">Pasirinkite **Taip,** kad leistumėte registro rengyklei keisti įrenginį.</span><span class="sxs-lookup"><span data-stu-id="b13b4-111">Select **Yes** to allow Registry Editor to make changes to your device.</span></span>
    3. <span data-ttu-id="b13b4-112">Registro rengyklėje įtraukite **EnableADAL** DWORD reikšmę su parametru **0** pagal HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\Identity.</span><span class="sxs-lookup"><span data-stu-id="b13b4-112">In Registry Editor, add a DWORD value of **EnableADAL** with a setting of **0** under HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\Identity.</span></span>

<span data-ttu-id="b13b4-113">Jei norite gauti daugiau informacijos, peržiūrėkite [ryšio problemos prisijungimo atnaujinus į Office 2016 komponavimo versijos 16.0.7967 "Windows 10".](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016)</span><span class="sxs-lookup"><span data-stu-id="b13b4-113">For more information, see [Connection issues in sign-in after update to Office 2016 build 16.0.7967 on Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).</span></span>