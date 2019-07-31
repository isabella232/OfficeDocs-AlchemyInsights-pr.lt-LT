---
title: Problemos prisijungiant prie "Office" programos
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
ms.openlocfilehash: 5f500ecf1f779fb1be4d257fd050a3ad054087dc
ms.sourcegitcommit: 699ac3b0d66e0640f8e933eba3c2a4ba1cfcf3c7
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 07/30/2019
ms.locfileid: "35938280"
---
# <a name="fixing-the-office-apps-your-computers-trusted-platform-module-is-not-functioning-properly-message"></a><span data-ttu-id="6805c-102">Nustatant Office apps "jūsų kompiuterio patikimos platformos modulis veikia netinkamai" pranešimas</span><span class="sxs-lookup"><span data-stu-id="6805c-102">Fixing the Office apps "Your computer's Trusted Platform module is not functioning properly" message</span></span>

<span data-ttu-id="6805c-103">Norėdami išspręsti šią klaidą, atlikite šiuos veiksmus:</span><span class="sxs-lookup"><span data-stu-id="6805c-103">To fix this error, try the following:</span></span>

- <span data-ttu-id="6805c-104">Įdiekite naujausius [Windows](https://support.microsoft.com/help/4027667/windows-10-update) ir [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).</span><span class="sxs-lookup"><span data-stu-id="6805c-104">Install the latest updates for [Windows](https://support.microsoft.com/help/4027667/windows-10-update) and [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).</span></span>
- <span data-ttu-id="6805c-105">[Aišku Office kredencialus](https://docs.microsoft.com/eoffice/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) naudodami Windows kredencialų tvarkytuvas.</span><span class="sxs-lookup"><span data-stu-id="6805c-105">[Clear Office credentials](https://docs.microsoft.com/eoffice/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) using Windows Credential Manager.</span></span><br/>
    <span data-ttu-id="6805c-106">**Pastaba:** 16,0 pasikeitė registro maršrutai Office 2016.</span><span class="sxs-lookup"><span data-stu-id="6805c-106">**Note:** The registry paths for Office 2016 have changed to 16.0.</span></span> <span data-ttu-id="6805c-107">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span><span class="sxs-lookup"><span data-stu-id="6805c-107">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span></span>
- <span data-ttu-id="6805c-108">Pabandykite [vartotojo susigrąžinimo procesas](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) nustatyti patikimos platformos modulio (TPM) gedimai.</span><span class="sxs-lookup"><span data-stu-id="6805c-108">Try the [user recovery process](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) to fix Trusted Platform Module (TPM) failures.</span></span>
- <span data-ttu-id="6805c-109">Nustatyti, EnableADAL = 0, atlikite šiuos veiksmus:</span><span class="sxs-lookup"><span data-stu-id="6805c-109">Set the EnableADAL = 0 using the following steps:</span></span>  
    1. <span data-ttu-id="6805c-110">Dešiniuoju pelės mygtuku spustelėkite Windows mygtuką pradėti, pasirinkite **vykdyti**, įveskite **regedit**, ir tada pasirinkite **gerai**.</span><span class="sxs-lookup"><span data-stu-id="6805c-110">Right-click the Windows Start button, choose **Run**, type **regedit**, and then choose **OK**.</span></span>
    2. <span data-ttu-id="6805c-111">Pasirinkite **taip** , kad registro rengyklę, kad jūsų įrenginio.</span><span class="sxs-lookup"><span data-stu-id="6805c-111">Select **Yes** to allow Registry Editor to make changes to your device.</span></span>
    3. <span data-ttu-id="6805c-112">Registro rengyklėje pridėti reikšmę DWORD, **EnableADAL** su parametras **0** pagal HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\Identity.</span><span class="sxs-lookup"><span data-stu-id="6805c-112">In Registry Editor, add a DWORD value of **EnableADAL** with a setting of **0** under HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\Identity.</span></span>

<span data-ttu-id="6805c-113">Daugiau informacijos ieškokite [ryšio problemų prisijungdami po Office 2016 statyti 16.0.7967 "Windows 10" naujinimą](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).</span><span class="sxs-lookup"><span data-stu-id="6805c-113">For more information, see [Connection issues in sign-in after update to Office 2016 build 16.0.7967 on Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).</span></span>