---
title: Parengimo tarnybos konfigūravimas
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004687"
- "8468"
ms.openlocfilehash: 271ab7ad34c0f85f6f5a9d8d3dc2d901fe6fe8f978a2cc98eed986f594036f17
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54033286"
---
# <a name="configuring-the-provision-service"></a>Parengimo tarnybos konfigūravimas

Kad veiktų automatinis vartotojų parengimas, "Azure AD" reikalauja galiojančių kredencialų, kurie leidžia prisijungti prie darbo dienos žiniatinklio tarnybų API. Be to, mygtukas Tikrinti ryšį darbo dieną su AD vartotojo parengimo programa taip pat patikrina, ar jis gali prisijungti prie "Azure AD Prisijungimas parengimo agento, susieto su AD domenu.

Jei įrašant kredencialus "Azure" portalas grąžina klaidą, atlikite toliau nurodytus rekomenduojamus veiksmus:

1. Įsitikinkite, kad sukonfigūravote darbo dienos integravimo sistemos vartotojo paskyrą, kaip nurodyta mokymo priemonės skyriuje Integravimo [sistemos vartotojo konfigūravimas darbo dieną](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial).
2. Patvirtinkite, kad "Azure AD Prisijungimas" parengimo agento tarnyba veikia jūsų vietiniame "Windows serveryje naudojant tarnybų valdymo konsolę. Taip pat galite patikrinti agento būseną "Azure" portale spustelėdami mygtuką Peržiūrėti vietinį agentą.
3. Įsitikinkite, kad įvedate lauko "Darbo dienos vartotojo vardas" reikšmę naudodami username@workday-nuomotojo vardo formatą. Jei trūksta darbo dienos nuomotojo vardo, darbo dienos autentifikavimas nepavyksta.
4. Jei konfigūruojate integravimą su darbo dienos diegimo nuomotoju, atkreipkite dėmesį į suplanuotas darbo dienos nuomotojo prastovas. Darbo diena suplanavo savo įgyvendinimo nuomotojų laiką savaitgaliais (paprastai nuo penktadienio vakaro iki šeštadienio ryto), o ryšio gedimai šiame prastovos lange yra žinoma problema, kuri automatiškai išsprendžiama, kai tik diegimo nuomotojai vėl bus prisijungę.
5. Retais atvejais taip pat galite matyti šią klaidą, jei integravimo sistemos vartotojo slaptažodis pasikeitė dėl nuomotojo atnaujinimo arba jei paskyros būsena užrakinta arba jos galiojimo laikas baigėsi. Patikrinkite integravimo sistemos vartotojo būseną su savo darbo dienos administratoriumi.

Daugiau informacijos apie automatinio parengimo darbo dienos konfigūravimą žr. [Vadovėlis: Darbo dienos konfigūravimas automatiniam vartotojų parengimui](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial).
