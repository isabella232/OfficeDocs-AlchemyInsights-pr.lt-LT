---
title: Teams,skirtas "Mac"
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/10/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6173"
- "6166"
- "9003233"
- "9002573"
ms.openlocfilehash: c9c4eb811c93f6d11ebf606ba4bd20cddc2901d6616700ebfe6ef597dd8dc006
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 08/05/2021
ms.locfileid: "53940683"
---
# <a name="teams-add-in-for-mac"></a>Teams,skirtas "Mac"

Norėdami pašalinti trūkstamą "Teams", skirtą "Mac", operacinės sistemos vartotojams, atlikite šiuos veiksmus:

**1 veiksmas:** Jei turite hibridinę Exchange vietinį (2016 CU3 arba naujesnę), naudokite "Test-HMA.ps1" įrankį, kad patvirtintumėte, jog hibridinis modernusis autentifikavimas tinkamai sukonfigūruotas. Daugiau informacijos žr. [Hibridinio modernaus autentifikavimo sąrankos patvirtinimas "Outlook OS" ir "Android".](https://aka.ms/TestHMAEAS)  

**Pastaba** Naudokite UPN adreso formatą (pvz., [username@contoso.com](mailto:username@contoso.com)), o ne domeną\vartotojo vardą. Tai atlikite net vartotojams, naudojantiems Exchange Online pašto dėžutes.

**2 veiksmas:** Nueikite į Įrankių **paskyros**  >  ... "Outlook for Mac" ir raskite ir pasirinkite paskyrą. Patvirtinkite, kad nurodytas vartotojo vardas yra UPN formatu (pvz., [username@contoso.com](mailto:username@contoso.com)).

**3 veiksmas:** Patvirtinkite, kad vartotojas yra licencijuotas Microsoft Teams vartotojas. Vartotojas turi naudoti "Office 365 Mac" prenumeratą, 16.24 arba naujesnę produkto versiją.