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
# <a name="blank-sign-in-screen-in-office-apps"></a>Tuščias prisijungimo ekranas, "Office" programos

Norėdami išspręsti šią problemą, pabandykite atlikti šiuos veiksmus:
- Įdiekite naujausius [Windows](https://support.microsoft.com/help/4027667/windows-10-update) ir [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).
- Iš naujo nustatyti "Internet Explorer" funkcijos: eikite į **Tools** > **Interneto parinktys** > **Išplėstinė** > (Atkreipkite dėmesį, kad jūs prarasite pritaikytus parametrus)**Iš naujo nustatyti Internet Explorer parametrus** , ir tada pabandykite prisijungti dar kartą į biurą.
- Išjungti "Windows" sargybos programa Guard (WDAG) ar panašią užkardos ir antivirusinę programą:
    1. Valdymo skyde eikite į **programos**ir tada pasirinkite **įjungti Windows funkcijas arba išjungti**.
    2. Jei "Windows" sargybos programa apsauga yra įjungta, bandykite jį išjungti.<br/>
    **Pastaba:** Gali tekti iš naujo paleisti kompiuterį.
- Užtikrinti, kad Microsoft.AAD.BrokerPlugin [AAD WAM plug-in](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-1) yra ne blokuojami iš bet kuri paraiška ar ugniasienės/anti-Anti-Virus programa.
- [Aišku Office kredencialus](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) naudodami Windows kredencialų tvarkytuvas.<br/>
    **Pastaba:** 16,0 pasikeitė registro maršrutai Office 2016. (Ex: \Software\Microsoft\Office\16.0\Common\Identity\)

Daugiau informacijos ieškokite [ryšio problemų prisijungdami po Office 2016 statyti 16.0.7967 "Windows 10" naujinimą](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).