---
title: Prisijungimo prie taikomųjų programų problemos
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/16/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7788"
- "9004355"
ms.openlocfilehash: 2d073367dc1c3e8e117c0b68e205297a65024872
ms.sourcegitcommit: 6d02eb533fd74199af6b20f714b3720991da2c4a
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 01/18/2021
ms.locfileid: "49901029"
---
# <a name="issues-signing-in-to-applications"></a>Prisijungimo prie taikomųjų programų problemos

Norėdami aptikti problemas, susijusias su vartotojų prisijungimų priežastimi arba diagnozuoti problemas, atlikite šiuos veiksmus:

1. Paleidžia [prisijungimo diagnostiką](https://ms.portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom).
2. Raskite įvykį, kurį norite analizuoti įvesdami išsamią informaciją apie vartotoją, taikomąją programą, prisijungimo laiką, užklausos ID arba koreliacijos ID.
3. Peržiūrėkite diagnostikos rezultatus, kuriuose pateikiama išsami informacija apie tai, kas nutiko ir kokių veiksmų galite imtis, jei reikia atlikti reikiamus pakitimus.

Toliau pateikiamos kelios Dažniausios problemos, su kuriomis galite susidurti prisijungiant prie taikomųjų programų:

1. Jūs arba vartotojas **yra užbaigę "AZURE AD" prisijungimo funkciją, tačiau yra netikėtas raginimas** – peržiūrėkite straipsnius [netikėtu sutikimu, kai prisijungimas prie taikomosios programos](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-prompt) ir [netikėta klaida atliekant sutikimą su taikomąja programa](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error).
2. Jūs arba vartotojas **prisijungęs prie taikomosios programos tiesiogiai, bet negaliu prisijungti prie jo iš "deeplink" pasirinktiniame portale arba "Access" skyde**: Peržiūrėkite [problemų, susijusių su prisijungiant prie taikomosios programos, šalinimas iš "Azure AD" mano programos](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-other-problem-access-panel).
3. Jūs arba vartotojas **atliko "AZURE AD" prisijungimo funkciją, bet taikomoji programa rodo klaidos pranešimą ir neleidžia vartotojui užbaigti prisijungimo srauto**: problema yra ta, kad programa nepriėmė atsakymo, kurį išleido "Azure AD". Atlikite [šiuos veiksmus](https://docs.microsoft.com/azure/active-directory/application-sign-in-problem-application-error) , kad išspręstumėte triktis.
4. Jūs arba vartotojas **negali prisijungti prie programos ne galerijos programos, sukonfigūruotos kaip vienkartinio prisijungimo slaptažodis**: vykdykite nurodymus atlikdami [šiuos veiksmus](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-password-based-sso) , kad išspręstumėte triktis.
5. Jūs arba vartotojas **negali prisijungti prie "AZURE ad Gallery" taikomosios programos, sukonfigūruotos kaip vienkartinio prisijungimo slaptažodis**: atlikite [šiuos veiksmus](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-password-based-sso) , kad išspręstumėte triktis.
6. Jūs arba vartotojas **negali prisijungti prie "Microsoft" taikomosios programos**: atlikite [šiuos veiksmus](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-first-party-microsoft) , kad išspręstumėte triktis.
7. Jūs arba vartotojas **negali prisijungti prie programos ne galerijos programos, sukonfigūruotos naudoti bendrą autentifikacijos**: atlikite [šiuos veiksmus](https://docs.microsoft.com/azure/active-directory/application-sign-in-problem-federated-sso-non-gallery) , kad išspręstumėte triktis.
8. Jūs arba vartotojas **negali prisijungti prie "AZURE ad Gallery" taikomosios programos, sukonfigūruotos naudoti bendrą autentifikacija**: atlikite [šiuos veiksmus](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-federated-sso-gallery) , kad išspręstumėte triktis.
9. Jūs arba vartotojas **negali prisijungti prie pagal vartotojo sukurtą taikomąją programą**: atlikite [šiuos veiksmus](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-federated-sso-gallery) , kad išspręstumėte triktis.
10. Jūs arba vartotojas **negalite prisijungti prie vietinių taikomųjų programų naudodami "AZURE AD" taikomosios programos tarpinį serverį**: atlikite [šiuos veiksmus](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-on-premises-application-proxy) , kad išspręstumėte triktis.

