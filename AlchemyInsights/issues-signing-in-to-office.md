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
# <a name="blank-sign-in-screen-in-microsoft-365-apps"></a>Tuščias prisijungimo ekranas "Microsoft 365" programose

Norėdami išspręsti šią problemą, pabandykite atlikti šiuos veiksmus:
- Įdiekite naujausius ["Windows" ir "Office"](https://support.microsoft.com/help/4027667/windows-10-update) [naujinimus.](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5)
- Iš naujo nustatykite "Internet Explorer" parinktis: Eikite į Įrankiai Interneto parinktys Išplėstinis "Internet Explorer" parametrų nustatymas iš naujo (atminkite, kad prarasite pasirinktinius  >    >    >   parametrus), tada bandykite prisijungti prie "Office" dar kartą.
- Išjunkite "Windows" sargybos programos apsaugą (WDAG) arba panašią užkardą arba antivirusinę programą:
    1. Valdymo skyde eikite į **Programos**, tada pasirinkite **Įjungti arba išjungti "Windows" funkcijas.**
    2. Jei įgalinta "Windows" sargybos programos apsauga, pabandykite ją išjungti.<br/>
    **Pastaba:** Gali tekti iš naujo paleisti kompiuterį.
- Įsitikinkite, kad "Microsoft.AAD.BrokerPlugin [AAD WAM"](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-1) priedo neblokuoja jokia programa arba užkarda / antivirusinė programa.
- [Išvalykite "Office"](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) kredencialus naudodami "Windows" kredencialų tvarkytuvą.<br/>
    **Pastaba:** "Office 2016" registro keliai pakeisti į 16.0. (pvz.: \Software\Microsoft\Office\16.0\Common\Identity\)

Daugiau informacijos žr. Prisijungimo problemos atnaujinus į ["Office 2016" komponavimo versiją 16.0.7967 sistemoje "Windows 10".](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016)