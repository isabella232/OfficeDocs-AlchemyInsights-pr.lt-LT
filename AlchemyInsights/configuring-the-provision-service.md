---
title: Nuostatų paslaugos konfigūravimas
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
ms.openlocfilehash: fd272f8d554d73c87b832443815c25ebb2acc3eb
ms.sourcegitcommit: b71e5981b7f30ef2bce4e695118d03aa68a5be4a
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 03/05/2021
ms.locfileid: "50482872"
---
# <a name="configuring-the-provision-service"></a>Nuostatų paslaugos konfigūravimas

Jei reikia automatizuoto vartotojo parengimo darbui, "Azure AD" reikia galiojančių kredencialų, leidžiančių prisijungti prie darbo dienos žiniatinklio tarnybų API. Be to, "Test Connection" mygtukas darbo dieną, skirtas skelbimų vartotojo parengimo programėlei, taip pat patikrina, ar jis gali prisijungti prie "Azure AD Connect" parengimo agento, susieto su skelbimo domenu.

Jei "Azure" portale įrašant kredencialus grąžinama klaida, atlikite toliau nurodytus rekomenduojamus veiksmus:

1. Įsitikinkite, kad esate sukonfigūravę darbo dienos integravimo sistemos vartotojo abonementą, kaip nurodyta skyriuje mokomųjų [vartotojų integravimo sistemos vartotojo darbo dienos konfigūravimas](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial).
2. Įsitikinkite, kad "Azure AD Connect" parengimo agento tarnyba veikia ir veikia jūsų vietiniame "Windows Server", naudodami tarnybų valdymo konsolę. Taip pat galite patikrinti agento būseną "Azure" portale spustelėdami mygtuką Peržiūrėti vietinius agentus.
3. Įsitikinkite, kad įvedate lauko "WORKDAY username" reikšmę naudodami formatą username@workday – nuomotojo vardas. Jei darbo dienos – nuomotojo vardo nėra, nepavyksta autentifikuoti darbo dieną.
4. Jei konfigūruojate integraciją su "WORKDAY" diegimo nuomotoju, Įsiminkite jūsų darbo dienos nuomotojo suplanuotus prastovos valandas. Darbo diena suplanavo laiką savo įgyvendinimo nuomotojams per savaitgalius (paprastai nuo penktadienio vakaro iki šeštadienio ryto) ir ryšio triktys šio prastovų lange yra žinoma problema, kurią automatiškai išsprendžia, kai tik įgyvendinimo nuomotojai grįžta internete.
5. Retais atvejais taip pat galite matyti šią klaidą, jei integravimo sistemos vartotojo slaptažodis buvo pakeistas dėl nuomotojo atnaujinimo arba paskyra yra užrakintoje arba pasibaigutoje būsenoje. Patikrinkite integravimo sistemos vartotojo būseną su savo darbo dienos administratoriumi.

Išsamesnės informacijos apie darbo dienos konfigūravimą automatiniam parengimas ieškokite straipsnyje [Susipažinkite: darbo dienos konfigūravimas automatiniam vartotojų parengimas](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial).
