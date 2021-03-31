---
title: 126 OWA nepavyksta rasti klaidos gaunant pašto dėžutę?
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "126"
- "1600020"
ms.assetid: e85bffec-e5ad-418a-8561-dab6257e1864
ms.openlocfilehash: 6bab821aaa3b50c365ef5d25a61bca195c76d7ce
ms.sourcegitcommit: e552d65aac79433a911723412bf1252d20d3f0da
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 03/30/2021
ms.locfileid: "51426670"
---
# <a name="getting-a-mailbox-not-found-error-in-outlook-on-the-web"></a>Gaunate pašto dėžutę, kurios nepavyko rasti internetinėje "Outlook"?

Jei naudojate internetinę "Outlook" ir  nepavyksta rasti klaidos pašto dėžutės, paskyra, kurią naudojote prisijungdami prie internetinės "Outlook", neturi "Exchange Online" licencijos, todėl jokia pašto dėžutė nėra susieta su paskyra. Administratorius gali priskirti jūsų paskyrai licenciją, atlikite šiuos veiksmus:

1. Atidarykite ["Microsoft 365"](https://portal.office.com/adminportal/home#/homepage)  administravimo centrą  ir eikite į Aktyvūs vartotojai dalyje Vartotojai ir pasirinkite vartotoją, kuris mato klaidą.

2. Atidaromame vartotojo puslapyje eikite į sekciją **Licencijos** ir taikomosios programos, pasirinkite atitinkamą **vietos reikšmę** ir priskirkite licenciją, kurioje yra "Exchange Online" (išplėskite licenciją, kad pamatytumėte jos informaciją). Kai baigsite, spustelėkite Įrašyti **keitimus**.

Kai kuriais atvejais, jei licencija jau priskirta vartotojo paskyrai, pašalinus ir persignuojant licenciją galima išspręsti problemą ir tinkamai ją parengti sistemoje: 

- Patikrinkite, ar jūsų M365 "Exchange Online" (ir kitos, jei turite) prenumeratos yra dabartinės ir pastaruoju metu jų galiojimas nesibaigė.

Kai įsitikinsite, kad jūsų prenumeratos galiojimas nepasibaigė ir vartotojo paskyrai priskirta galiojanti licencija, gali užtrukti iki 24 valandų, kol licencija bus susaista, todėl gali tekti palaukti, kol problema bus išspręsta. Daugiau informacijos [žr. Licencijų priskyrimas ir valdymas](https://docs.microsoft.com/deployoffice/overview-licensing-activation-microsoft-365-apps#assign-and-manage-licenses).