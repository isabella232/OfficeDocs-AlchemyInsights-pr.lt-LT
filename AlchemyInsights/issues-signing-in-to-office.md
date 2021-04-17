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
- "2556"
ms.openlocfilehash: e6cbab7401fd6168041e7fc31ac97e3be036536d
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 04/15/2021
ms.locfileid: "51833047"
---
# <a name="blank-sign-in-screen-in-microsoft-365-apps"></a><span data-ttu-id="162e5-102">Tuščias prisijungimo ekranas "Microsoft 365" programose</span><span class="sxs-lookup"><span data-stu-id="162e5-102">Blank sign-in screen in Microsoft 365 apps</span></span>

<span data-ttu-id="162e5-103">Norėdami išspręsti šią problemą, pabandykite atlikti šiuos veiksmus:</span><span class="sxs-lookup"><span data-stu-id="162e5-103">To fix this issue, try the following:</span></span>
- <span data-ttu-id="162e5-104">Įdiekite naujausius ["Windows" ir "Office"](https://support.microsoft.com/help/4027667/windows-10-update) [naujinimus.](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5)</span><span class="sxs-lookup"><span data-stu-id="162e5-104">Install the latest updates for [Windows](https://support.microsoft.com/help/4027667/windows-10-update) and [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).</span></span>
- <span data-ttu-id="162e5-105">Iš naujo nustatykite "Internet Explorer" parinktis: Eikite į Įrankiai Interneto parinktys Išplėstinis "Internet Explorer" parametrų nustatymas iš naujo (atminkite, kad prarasite pasirinktinius  >    >    >   parametrus), tada bandykite prisijungti prie "Office" dar kartą.</span><span class="sxs-lookup"><span data-stu-id="162e5-105">Reset Internet Explorer options: Go to **Tools** > **Internet Options** > **Advanced** > **Reset Internet Explorer Settings** (note that you will lose custom settings), and then try signing in to Office again.</span></span>
- <span data-ttu-id="162e5-106">Išjunkite "Windows" sargybos programos apsaugą (WDAG) arba panašią užkardą arba antivirusinę programą:</span><span class="sxs-lookup"><span data-stu-id="162e5-106">Disable the Windows Defender Application Guard (WDAG) or any similar firewall or anti-virus program:</span></span>
    1. <span data-ttu-id="162e5-107">Valdymo skyde eikite į **Programos**, tada pasirinkite **Įjungti arba išjungti "Windows" funkcijas.**</span><span class="sxs-lookup"><span data-stu-id="162e5-107">In Control Panel, go to **Programs**, and then choose **Turn Windows features on or off**.</span></span>
    2. <span data-ttu-id="162e5-108">Jei įgalinta "Windows" sargybos programos apsauga, pabandykite ją išjungti.</span><span class="sxs-lookup"><span data-stu-id="162e5-108">If Windows Defender Application Guard is enabled, try disabling it.</span></span><br/>
    <span data-ttu-id="162e5-109">**Pastaba:** Gali tekti iš naujo paleisti kompiuterį.</span><span class="sxs-lookup"><span data-stu-id="162e5-109">**Note:** You may need to restart the computer.</span></span>
- <span data-ttu-id="162e5-110">Įsitikinkite, kad "Microsoft.AAD.BrokerPlugin [AAD WAM"](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-1) priedo neblokuoja jokia programa arba užkarda / antivirusinė programa.</span><span class="sxs-lookup"><span data-stu-id="162e5-110">Ensure that the Microsoft.AAD.BrokerPlugin [AAD WAM plug-in](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-1) is not being blocked by any application or firewall/anti-virus program.</span></span>
- <span data-ttu-id="162e5-111">[Išvalykite "Office"](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) kredencialus naudodami "Windows" kredencialų tvarkytuvą.</span><span class="sxs-lookup"><span data-stu-id="162e5-111">[Clear Office credentials](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) using Windows Credential Manager.</span></span><br/>
    <span data-ttu-id="162e5-112">**Pastaba:** "Office 2016" registro keliai pakeisti į 16.0.</span><span class="sxs-lookup"><span data-stu-id="162e5-112">**Note:** The registry paths for Office 2016 have changed to 16.0.</span></span> <span data-ttu-id="162e5-113">(pvz.: \Software\Microsoft\Office\16.0\Common\Identity\)</span><span class="sxs-lookup"><span data-stu-id="162e5-113">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span></span>

<span data-ttu-id="162e5-114">Daugiau informacijos žr. Prisijungimo problemos atnaujinus į ["Office 2016" komponavimo versiją 16.0.7967 sistemoje "Windows 10".](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016)</span><span class="sxs-lookup"><span data-stu-id="162e5-114">For more information, see [Connection issues in sign-in after update to Office 2016 build 16.0.7967 on Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).</span></span>