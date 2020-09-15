---
title: Prisijungimo prie "Microsoft 365" programų problemos
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
- "9000571"
- "2559"
ms.openlocfilehash: 57a4df23dc66eaf4c283dde741be6f415939633d
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47695187"
---
# <a name="fixing-the-microsoft-365-apps-your-computers-trusted-platform-module-is-not-functioning-properly-message"></a><span data-ttu-id="41903-102">"Microsoft 365" taikomųjų programų taisymas pranešimas "jūsų kompiuterio patikimos platformos modulis neveikia tinkamai"</span><span class="sxs-lookup"><span data-stu-id="41903-102">Fixing the Microsoft 365 apps "Your computer's Trusted Platform module is not functioning properly" message</span></span>

<span data-ttu-id="41903-103">Norėdami pašalinti šią klaidą, atlikite šiuos veiksmus:</span><span class="sxs-lookup"><span data-stu-id="41903-103">To fix this error, try the following:</span></span>

- <span data-ttu-id="41903-104">Įdiekite naujausius ["Windows"](https://support.microsoft.com/help/4027667/windows-10-update) ir " [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5)" naujinimus.</span><span class="sxs-lookup"><span data-stu-id="41903-104">Install the latest updates for [Windows](https://support.microsoft.com/help/4027667/windows-10-update) and [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).</span></span>
- <span data-ttu-id="41903-105">[Išvalykite "Office" kredencialus](https://docs.microsoft.com/eoffice/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) naudodami "Windows" Kredencialų tvarkytuvą.</span><span class="sxs-lookup"><span data-stu-id="41903-105">[Clear Office credentials](https://docs.microsoft.com/eoffice/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) using Windows Credential Manager.</span></span><br/>
    <span data-ttu-id="41903-106">**Pastaba:** "Office 2016" registro keliai pakeisti į "16,0".</span><span class="sxs-lookup"><span data-stu-id="41903-106">**Note:** The registry paths for Office 2016 have changed to 16.0.</span></span> <span data-ttu-id="41903-107">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span><span class="sxs-lookup"><span data-stu-id="41903-107">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span></span>
- <span data-ttu-id="41903-108">Išbandykite [vartotojų atkūrimo procesą](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) , kad išspręstumėte patikimos platformos modulio (TPM) triktis.</span><span class="sxs-lookup"><span data-stu-id="41903-108">Try the [user recovery process](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) to fix Trusted Platform Module (TPM) failures.</span></span>
- <span data-ttu-id="41903-109">Nustatykite EnableADAL = 0 atlikdami šiuos veiksmus:</span><span class="sxs-lookup"><span data-stu-id="41903-109">Set the EnableADAL = 0 using the following steps:</span></span>  
    1. <span data-ttu-id="41903-110">Dešiniuoju pelės mygtuku spustelėkite "Windows" mygtuką pradėti, pasirinkite **vykdyti**, įveskite **regedit**, tada pasirinkite **gerai**.</span><span class="sxs-lookup"><span data-stu-id="41903-110">Right-click the Windows Start button, choose **Run**, type **regedit**, and then choose **OK**.</span></span>
    2. <span data-ttu-id="41903-111">Pasirinkite **taip** , kad leistumėte registro rengyklę atlikti savo įrenginio keitimą.</span><span class="sxs-lookup"><span data-stu-id="41903-111">Select **Yes** to allow Registry Editor to make changes to your device.</span></span>
    3. <span data-ttu-id="41903-112">Registro rengyklėje įtraukite **Enableadal** reikšmę DWORD su parametru **0** , HKEY_CURRENT_USER \Software\Microsoft\Office\16.0\Common\Identity.</span><span class="sxs-lookup"><span data-stu-id="41903-112">In Registry Editor, add a DWORD value of **EnableADAL** with a setting of **0** under HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\Identity.</span></span>

<span data-ttu-id="41903-113">Daugiau informacijos ieškokite [prisijungimo problemų prisijungiant, atnaujinus į "Office 2016" komponavimo versiją 16.0.7967 "Windows 10"](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).</span><span class="sxs-lookup"><span data-stu-id="41903-113">For more information, see [Connection issues in sign-in after update to Office 2016 build 16.0.7967 on Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).</span></span>