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
- "2556"
ms.openlocfilehash: 4658b4df8a48072b4cc9d72bf503d7911bb5126b
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 06/05/2020
ms.locfileid: "44579909"
---
# <a name="blank-sign-in-screen-in-microsoft-365-apps"></a><span data-ttu-id="a140c-102">Tuščias prisijungimo ekranas "Microsoft 365" programėlėse</span><span class="sxs-lookup"><span data-stu-id="a140c-102">Blank sign-in screen in Microsoft 365 apps</span></span>

<span data-ttu-id="a140c-103">Norėdami išspręsti šią problemą, pabandykite atlikti šiuos veiksmus:</span><span class="sxs-lookup"><span data-stu-id="a140c-103">To fix this issue, try the following:</span></span>
- <span data-ttu-id="a140c-104">Įdiekite naujausius ["Windows"](https://support.microsoft.com/help/4027667/windows-10-update) ir ["Office"](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5)naujinimus .</span><span class="sxs-lookup"><span data-stu-id="a140c-104">Install the latest updates for [Windows](https://support.microsoft.com/help/4027667/windows-10-update) and [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).</span></span>
- <span data-ttu-id="a140c-105">Iš naujo nustatykite "Internet Explorer" parinktis: eikite į **Įrankiai**  >  **Interneto parinktys**  >  **Išplėstiniai**  >  **"Internet Explorer" parametrų nustatymas iš naujo** (atminkite, kad prarasite pasirinktinius parametrus), tada bandykite prisijungti prie "Office" dar kartą.</span><span class="sxs-lookup"><span data-stu-id="a140c-105">Reset Internet Explorer options: Go to **Tools** > **Internet Options** > **Advanced** > **Reset Internet Explorer Settings** (note that you will lose custom settings), and then try signing in to Office again.</span></span>
- <span data-ttu-id="a140c-106">Išjungti Windows Defender Application Guard (WDAG) arba bet kokios panašios ugniasienės ar antivirusinę programą:</span><span class="sxs-lookup"><span data-stu-id="a140c-106">Disable the Windows Defender Application Guard (WDAG) or any similar firewall or anti-virus program:</span></span>
    1. <span data-ttu-id="a140c-107">Valdymo skyde eikite į **Programos**, tada pasirinkite **Įjungti arba išjungti "Windows" funkcijas**.</span><span class="sxs-lookup"><span data-stu-id="a140c-107">In Control Panel, go to **Programs**, and then choose **Turn Windows features on or off**.</span></span>
    2. <span data-ttu-id="a140c-108">Jei įgalinta "Windows" sargybos programų apsauga, pabandykite ją išjungti.</span><span class="sxs-lookup"><span data-stu-id="a140c-108">If Windows Defender Application Guard is enabled, try disabling it.</span></span><br/>
    <span data-ttu-id="a140c-109">**Pastaba:** Gali tekti iš naujo paleisti kompiuterį.</span><span class="sxs-lookup"><span data-stu-id="a140c-109">**Note:** You may need to restart the computer.</span></span>
- <span data-ttu-id="a140c-110">Įsitikinkite, kad Microsoft.AAD.BrokerPlugin [AAD WAM papildinys](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-1) nėra užblokuotas jokios programos arba ugniasienės/antivirusinę programą.</span><span class="sxs-lookup"><span data-stu-id="a140c-110">Ensure that the Microsoft.AAD.BrokerPlugin [AAD WAM plug-in](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-1) is not being blocked by any application or firewall/anti-virus program.</span></span>
- <span data-ttu-id="a140c-111">[Išvalykite "Office" kredencialus](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) naudodami "Windows" kredencialų tvarkytuvą.</span><span class="sxs-lookup"><span data-stu-id="a140c-111">[Clear Office credentials](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) using Windows Credential Manager.</span></span><br/>
    <span data-ttu-id="a140c-112">**Pastaba:** Registro keliai Office 2016 pasikeitė į 16.0.</span><span class="sxs-lookup"><span data-stu-id="a140c-112">**Note:** The registry paths for Office 2016 have changed to 16.0.</span></span> <span data-ttu-id="a140c-113">(Pvz.: \Software\Microsoft\Office\16.0\Common\Identity\)</span><span class="sxs-lookup"><span data-stu-id="a140c-113">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span></span>

<span data-ttu-id="a140c-114">Jei norite gauti daugiau informacijos, peržiūrėkite [ryšio problemos prisijungimo atnaujinus į Office 2016 komponavimo versijos 16.0.7967 "Windows 10".](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016)</span><span class="sxs-lookup"><span data-stu-id="a140c-114">For more information, see [Connection issues in sign-in after update to Office 2016 build 16.0.7967 on Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).</span></span>