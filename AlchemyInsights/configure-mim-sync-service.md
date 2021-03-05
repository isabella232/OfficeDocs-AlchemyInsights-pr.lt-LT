---
title: MIM sinchronizavimo paslaugos konfigūravimas
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8472"
- "9004688"
ms.openlocfilehash: 48e9a0e8c26088b690092bfaedfba641841739f6
ms.sourcegitcommit: 379e132c4d21ecf703d5506484ec96a767fdda39
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 03/04/2021
ms.locfileid: "50481870"
---
# <a name="configure-mim-sync-service"></a>MIM sinchronizavimo paslaugos konfigūravimas

"Microsoft Identity Manager" (MIM) Sinchronizavimo tarnyba yra MIM komponentas. Tai centralizuota vietinė tarnyba, kuri saugo ir sujungia informaciją apie organizacijas, kurios turi kelis vietinius katalogus ir duomenų bazes. Jums gali būti suteikta galimybė išspręsti problemą su MIM sinchronizavimu, jei problema buvo išspręsta naujausiame "MIM" naujinime arba yra viena iš kitų toliau nurodytų problemų.

**Rekomenduojami veiksmai**

1. Įsitikinkite, kad naudojate vėliausią MIM sinchronizavimo naujinimą ir patikrinkite [Mim sinchronizavimo leidimo pastabas](https://docs.microsoft.com/microsoft-identity-manager/reference/version-history) , kad nustatytumėte, ar problema buvo išspręsta naujinime.
2. Jei problema yra bendra LDAP, Bendrasis SQL, Lotus Domino arba žiniatinklio tarnybų jungtis, įsitikinkite, kad naudojate naujausią [bendrųjų jungčių](https://docs.microsoft.com/microsoft-identity-manager/reference/microsoft-identity-manager-2016-connector-version-history)naujinimą.
3. Jei MIM sinchronizavimo vykdymas sustabdomas su klaida, skaitykite " [Run" klaidų kodų](https://docs.microsoft.com/microsoft-identity-manager/reference/maerrorcodes) , kad nustatytumėte galimas priežastis, lentelę.
4. Jei paleisti sustoja naudodami **plėtinį – dll – išimtis**, tada spustelėkite šiuos žodžius, kad atidarytumėte langą **jungties vietos objekto ypatybės** , ir spustelėkite **rietuvės sekimas...** , kad pamatytumėte daugiau informacijos apie PRIEŽASTĮ, kaip aprašyta [plėtinio – DLL – išimtis](https://social.technet.microsoft.com/wiki/contents/articles/7515.fim-troubleshooting-extension-dll-exception.aspx).
5. Jei slaptažodžio keitimo pranešimų tarnybos (PCNS) komponento ataskaitos **klaida 6025** įvykių rodinyje sinchronizuojant slaptažodžius, patikrinkite " [PCNS" ataskaitų klaidos 6025](https://social.technet.microsoft.com/wiki/contents/articles/4159.pcns-troubleshooting-event-id-6025.aspx).
6. Jei visas sinchronizavimas su FIM tarnybos valdymo agentu yra lėtas, pažymėkite **automatinio padidinimo** parametrą, skirtą tempdb, kaip aprašyta skyriuje [trikčių šalinimas lėtas arba kabinamas visas sinchronizavimas](https://social.technet.microsoft.com/wiki/contents/articles/14713.troubleshooting-fim-performance-slow-or-hanging-full-synchronization.aspx).
7. Jei įvyksta klaida, kai sustojo serveris su nepavykusia kūrimo-Via-Web-Services, naudodami FIM tarnybos tvarkymo agentą, žiūrėkite [palaikymo-info: nepavyko – kūrimas – Via – Web – Services](https://docs.microsoft.com/archive/blogs/iamsupport/support-info-fimma-failed-creation-via-web-services) dėl priežasčių apžvalgos.

