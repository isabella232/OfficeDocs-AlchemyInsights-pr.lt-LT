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
- "2556"
ms.openlocfilehash: 08bb0a94066f071f2ba0e9c54378f0d479191496
ms.sourcegitcommit: 699ac3b0d66e0640f8e933eba3c2a4ba1cfcf3c7
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 07/30/2019
ms.locfileid: "35938279"
---
# <a name="blank-sign-in-screen-in-office-apps"></a><span data-ttu-id="9e25a-102">Tuščias prisijungimo ekranas, "Office" programos</span><span class="sxs-lookup"><span data-stu-id="9e25a-102">Blank sign-in screen in Office apps</span></span>

<span data-ttu-id="9e25a-103">Norėdami išspręsti šią problemą, pabandykite atlikti šiuos veiksmus:</span><span class="sxs-lookup"><span data-stu-id="9e25a-103">To fix this issue, try the following:</span></span>
- <span data-ttu-id="9e25a-104">Įdiekite naujausius [Windows](https://support.microsoft.com/help/4027667/windows-10-update) ir [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).</span><span class="sxs-lookup"><span data-stu-id="9e25a-104">Install the latest updates for [Windows](https://support.microsoft.com/help/4027667/windows-10-update) and [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).</span></span>
- <span data-ttu-id="9e25a-105">Iš naujo nustatyti "Internet Explorer" funkcijos: eikite į **Tools** > **Interneto parinktys** > **Išplėstinė** > (Atkreipkite dėmesį, kad jūs prarasite pritaikytus parametrus)**Iš naujo nustatyti Internet Explorer parametrus** , ir tada pabandykite prisijungti dar kartą į biurą.</span><span class="sxs-lookup"><span data-stu-id="9e25a-105">Reset Internet Explorer options: Go to **Tools** > **Internet Options** > **Advanced** > **Reset Internet Explorer Settings** (note that you will lose custom settings), and then try signing in to Office again.</span></span>
- <span data-ttu-id="9e25a-106">Išjungti "Windows" sargybos programa Guard (WDAG) ar panašią užkardos ir antivirusinę programą:</span><span class="sxs-lookup"><span data-stu-id="9e25a-106">Disable the Windows Defender Application Guard (WDAG) or any similar firewall or anti-virus program:</span></span>
    1. <span data-ttu-id="9e25a-107">Valdymo skyde eikite į **programos**ir tada pasirinkite **įjungti Windows funkcijas arba išjungti**.</span><span class="sxs-lookup"><span data-stu-id="9e25a-107">In Control Panel, go to **Programs**, and then choose **Turn Windows features on or off**.</span></span>
    2. <span data-ttu-id="9e25a-108">Jei "Windows" sargybos programa apsauga yra įjungta, bandykite jį išjungti.</span><span class="sxs-lookup"><span data-stu-id="9e25a-108">If Windows Defender Application Guard is enabled, try disabling it.</span></span><br/>
    <span data-ttu-id="9e25a-109">**Pastaba:** Gali tekti iš naujo paleisti kompiuterį.</span><span class="sxs-lookup"><span data-stu-id="9e25a-109">**Note:** You may need to restart the computer.</span></span>
- <span data-ttu-id="9e25a-110">Užtikrinti, kad Microsoft.AAD.BrokerPlugin [AAD WAM plug-in](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-1) yra ne blokuojami iš bet kuri paraiška ar ugniasienės/anti-Anti-Virus programa.</span><span class="sxs-lookup"><span data-stu-id="9e25a-110">Ensure that the Microsoft.AAD.BrokerPlugin [AAD WAM plug-in](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-1) is not being blocked by any application or firewall/anti-virus program.</span></span>
- <span data-ttu-id="9e25a-111">[Aišku Office kredencialus](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) naudodami Windows kredencialų tvarkytuvas.</span><span class="sxs-lookup"><span data-stu-id="9e25a-111">[Clear Office credentials](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) using Windows Credential Manager.</span></span><br/>
    <span data-ttu-id="9e25a-112">**Pastaba:** 16,0 pasikeitė registro maršrutai Office 2016.</span><span class="sxs-lookup"><span data-stu-id="9e25a-112">**Note:** The registry paths for Office 2016 have changed to 16.0.</span></span> <span data-ttu-id="9e25a-113">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span><span class="sxs-lookup"><span data-stu-id="9e25a-113">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span></span>

<span data-ttu-id="9e25a-114">Daugiau informacijos ieškokite [ryšio problemų prisijungdami po Office 2016 statyti 16.0.7967 "Windows 10" naujinimą](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).</span><span class="sxs-lookup"><span data-stu-id="9e25a-114">For more information, see [Connection issues in sign-in after update to Office 2016 build 16.0.7967 on Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).</span></span>