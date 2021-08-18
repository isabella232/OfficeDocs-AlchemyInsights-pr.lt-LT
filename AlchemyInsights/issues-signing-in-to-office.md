---
title: Prisijungimo prie "Microsoft 365" problemos
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
ms.openlocfilehash: 7a8a0b68fc211e99b22e857d51d1de54e53a69357f75a0c60b1e83078cd5b27f
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54088044"
---
# <a name="blank-sign-in-screen-in-microsoft-365-apps"></a>Tuščias prisijungimo ekranas Microsoft 365 programėlėse

Norėdami išspręsti šią problemą, pabandykite atlikti šiuos veiksmus:
- Įdiekite naujausius ["Windows"](https://support.microsoft.com/help/4027667/windows-10-update) [ir "Office" naujinimus.](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5)
- Iš naujo nustatykite "Internet Explorer" parinktis: Eikite į Įrankiai Interneto parinktys Išplėstinis nustatymas iš  >    >    >  **naujo "Internet Explorer Parametrai** (atkreipkite dėmesį, kad prarasite pasirinktinius parametrus), tada bandykite prisijungti Office dar kartą.
- Išjunkite "Windows" sargybos "Application Guard" (WDAG) arba panašią užkardą arba antivirusinę programą:
    1. Valdymo skyde eikite **į Programos**, tada pasirinkite **Įjungti Windows arba išjungti.**
    2. Jei "Windows" sargybos "Application Guard" įjungta, pabandykite ją išjungti.<br/>
    **Pastaba:** Gali tekti iš naujo paleisti kompiuterį.
- Įsitikinkite, kad "Microsoft.AAD.BrokerPlugin [AAD WAM"](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-1) priedo neblokuoja jokia programa arba užkarda / antivirusinė programa.
- [Išvalykite Office kredencialus](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) naudodami Windows kredencialų tvarkytuvą.<br/>
    **Pastaba:** 2016 m. Office keliai pakeisti į 16.0. (ex: \Software\Microsoft\Office\16.0\Common\Identity\)

Daugiau informacijos žr. Prisijungimo problemos atnaujinus į ["Office 2016" komponavimo versiją 16.0.7967" Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).