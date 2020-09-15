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
- "2556"
ms.openlocfilehash: 3c016b198ad43f35c8149dde71c28a2f7fc3bd38
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47695295"
---
# <a name="blank-sign-in-screen-in-microsoft-365-apps"></a>Tuščias prisijungimo ekranas "Microsoft 365" programose

Norėdami išspręsti šią problemą, bandykite atlikti šiuos veiksmus:
- Įdiekite naujausius ["Windows"](https://support.microsoft.com/help/4027667/windows-10-update) ir " [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5)" naujinimus.
- "Internet Explorer" parinkčių nustatymas iš naujo: eikite į **Įrankiai**  >  **Interneto parinktys**  >  **Išplėstinė**  >  **"Internet Explorer" parametrų nustatymas iš naujo** (Nepamirškite, kad prarasite tinkintus parametrus), tada dar kartą bandykite prisijungti prie "Office".
- Išjunkite "Windows" sargybos taikomosios programos apsaugą (WDAG) arba bet kokią panašią užkardą ar antivirusinę programą:
    1. Valdymo skyde eikite į **programos**, tada pasirinkite **Įjungti arba išjungti "Windows" funkcijas**.
    2. Jei įgalinta "Windows" sargybos taikomosios programos apsauga, bandykite ją išjungti.<br/>
    **Pastaba:** Gali tekti iš naujo paleisti kompiuterį.
- Įsitikinkite, kad "Microsoft. AAD. BrokerPlugin [AAD WAM" papildinys](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-1) nėra blokuojamas naudojant bet kurią taikomąją programą arba užkardos/antivirusinės programos.
- [Išvalykite "Office" kredencialus](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) naudodami "Windows" Kredencialų tvarkytuvą.<br/>
    **Pastaba:** "Office 2016" registro keliai pakeisti į "16,0". (Ex: \Software\Microsoft\Office\16.0\Common\Identity\)

Daugiau informacijos ieškokite [prisijungimo problemų prisijungiant, atnaujinus į "Office 2016" komponavimo versiją 16.0.7967 "Windows 10"](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).