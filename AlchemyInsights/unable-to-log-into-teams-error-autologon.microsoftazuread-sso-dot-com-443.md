---
title: Nepavyksta prisijungti prie „Teams“ dėl klaidos autologon.microsoftazuread-sso.com:443
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 686e8f18-b871-4dd2-864f-8562947ab583
ms.collection: Adm_O365
ms.custom:
- "9001686"
- "3750"
ms.openlocfilehash: 6671a63d97f24fadc9b34907d75600a3c0ad1c9990a4a8f8d32034c11e8a952e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: lt-LT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54038408"
---
# <a name="unable-to-log-into-teams-due-to-error-autologonmicrosoftazuread-sso-dot-com443"></a>Nepavyksta prisijungti prie „Teams“ dėl klaidos autologon.microsoftazuread-sso taškas com:443

Jei kaip O365 autentifikavimas įjungta sklandi SSO, URL „autologon.microsoftazuread-sso.com“ gali prireikti įtraukti į intraneto svetaines.  Jei ji anksčiau buvo įtraukta į patikimas svetaines ir yra naudojama sklandi SSO, ji turi būti pašalinta iš patikimų svetainių.

Peržiūrėkite [Sklandžios SSO trikčių diagnostikos kontrolinį sąrašą](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-sso#troubleshooting-checklist).

Atlikite šiuos veiksmus, kad įtrauktumėte URL į intraneto svetainių sąrašą:

1. Atidarykite „Internet Explorer“ spustelėdami mygtuką **Pradžia**. Ieškos lauke įveskite „Internet Explorer“, tada rezultatų sąraše spustelėkite **Internet Explorer**.
2. Spustelėkite **Įrankiai**, tada spustelėkite **Interneto parinktys**.
3. Spustelėkite skirtuką **Sauga**.
4. Spustelėkite **Vietinio intraneto svetainės**, tada spustelėkite mygtuką **svetainės** ir mygtuką **Išsamiai**.
5. Įveskite svetainės URL ir spustelėkite **Įtraukti**.
6. Baigę spustelėkite **Uždaryti**.

Daugiau informacijos žr. [Sklandžios SSO, skirtos O365, diegimo dokumentacija](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-quick-start) (apima strategija pagrįstą procesą, kad būtų galima įtraukti URL į intraneto svetaines atliekant 3 veiksmą).
