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
# <a name="blank-sign-in-screen-in-microsoft-365-apps"></a>Tuščias prisijungimo ekranas "Microsoft 365" programėlėse

Norėdami išspręsti šią problemą, pabandykite atlikti šiuos veiksmus:
- Įdiekite naujausius ["Windows"](https://support.microsoft.com/help/4027667/windows-10-update) ir ["Office"](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5)naujinimus .
- Iš naujo nustatykite "Internet Explorer" parinktis: eikite į **Įrankiai**  >  **Interneto parinktys**  >  **Išplėstiniai**  >  **"Internet Explorer" parametrų nustatymas iš naujo** (atminkite, kad prarasite pasirinktinius parametrus), tada bandykite prisijungti prie "Office" dar kartą.
- Išjungti Windows Defender Application Guard (WDAG) arba bet kokios panašios ugniasienės ar antivirusinę programą:
    1. Valdymo skyde eikite į **Programos**, tada pasirinkite **Įjungti arba išjungti "Windows" funkcijas**.
    2. Jei įgalinta "Windows" sargybos programų apsauga, pabandykite ją išjungti.<br/>
    **Pastaba:** Gali tekti iš naujo paleisti kompiuterį.
- Įsitikinkite, kad Microsoft.AAD.BrokerPlugin [AAD WAM papildinys](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-1) nėra užblokuotas jokios programos arba ugniasienės/antivirusinę programą.
- [Išvalykite "Office" kredencialus](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) naudodami "Windows" kredencialų tvarkytuvą.<br/>
    **Pastaba:** Registro keliai Office 2016 pasikeitė į 16.0. (Pvz.: \Software\Microsoft\Office\16.0\Common\Identity\)

Jei norite gauti daugiau informacijos, peržiūrėkite [ryšio problemos prisijungimo atnaujinus į Office 2016 komponavimo versijos 16.0.7967 "Windows 10".](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016)