---
title: Perdavimas el. paštu per „Microsoft 365“
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "154"
- "3000003"
ms.assetid: 84191e23-496c-495a-a2ec-28c5ae0d4c0b
ms.openlocfilehash: ef06cfe41eee5d67bf82d4f64875ddafac82ee2062aade761f81b906cd428dd5
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54024214"
---
# <a name="set-up-a-multifunction-device-or-application-to-send-email"></a>Daugiafunkcio įrenginio arba programos, skirtos siųsti el. laiškus, nustatymas

Jei norite sužinoti apie galimas parinktis ir veiksmus, žr. [Kaip nustatyti daugiafunkcį įrenginį arba programą siųsti el. laiškus naudojant „Microsoft 365“](/Exchange/mail-flow-best-practices/how-to-set-up-a-multifunction-device-or-application-to-send-email-using-microsoft-365-or-office-365).
  
Jei turite įrenginį arba taikomąją programą, kuri neseniai nustojo veikti, dažniausiai pasitaiko problemų:

- **Autentifikavimo susijusios klaidos naudojant SMTP autentifikavimo kliento pateikimą** Neseniai atlikome keletą pakeitimų, susijusių su SMTP autentifikavimo darbu. Daugiau informacijos apie tai, kaip išspręsti problemas, žr. nesėkmingo autentifikavimo skyrių Spausdintuvų, skaitytuvų ir LOB programų, kurios siunčia [el. laiškus naudodami "Microsoft 365" arba "Office 365".](/Exchange/mail-flow-best-practices/fix-issues-with-printers-scanners-and-lob-applications-that-send-email-using-off#error-authentication-unsuccessful)
- **Mes priimame tik TLS 1.2 versiją, kai užtikriname saugų ryšį su Office 365** Jei naudojate saugų ryšį (TLS), įsitikinkite, kad jūsų taikomosios programos įrenginys palaiko TLS 1.2. Daugiau informacijos žr. [Pasirengimas TLS 1.2 Office 365 ir Office 365 GCC](/microsoft-365/compliance/prepare-tls-1.2-in-office-365).
 
Kitų problemų ir sprendimų ieškokite Spausdintuvų, skaitytuvų ir LOB programų, kurios siunčia el. laiškus naudodami ["Microsoft 365" arba "Office 365", problemų sprendimas.](/Exchange/mail-flow-best-practices/fix-issues-with-printers-scanners-and-lob-applications-that-send-email-using-off)

Norėdami peržiūrėti susijusius įrenginius, eikite į [SMTP autentifikavimo klientų ataskaitą](https://protection.office.com/mailflow/dashboard).

**Pastaba:** Exchange Online nėra masinio pašto scenarijų. Norėdami siųsti masinius komercinius el. laiškus (pvz., klientų informacinius biuletenius), turėtumėte naudoti trečiųjų šalių teikėjus, kurie specializuojasi šiose paslaugose.
