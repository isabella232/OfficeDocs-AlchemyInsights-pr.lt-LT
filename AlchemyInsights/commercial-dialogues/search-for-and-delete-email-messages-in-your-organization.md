---
title: Savo organizacijos el. laiškų ieška ir naikinimas
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000260"
- "7257"
ms.openlocfilehash: e935b10083459b81fc58e12bb59c9511defefa6d
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 03/11/2021
ms.locfileid: "50750010"
---
# <a name="search-for-and-delete-email-messages-in-your-organization"></a>Savo organizacijos el. laiškų ieška ir naikinimas

Atlikite šiuos veiksmus:

1. Jei nesate visuotinis administratorius, norėdami ieškoti pranešimo, jūsų abonementas turi būti įtrauktas į " **e" aptikimo tvarkytuvo vaidmenų grupę** arba **atitikties ieškos valdymo vaidmenį**. Norėdami panaikinti laišką, turite prisijungti prie **organizacijos valdymo vaidmenų grupės** arba **ieškos ir valymo valdymo vaidmens**. Šių vaidmenų teisės priskirtos [saugos & atitikties centre.](https://protection.office.com)
2. [Sukurkite turinio iešką](https://docs.microsoft.com/office365/securitycompliance/content-search) , kad rastumėte pranešimą, kurį norite panaikinti.
3. [Prisijunkite prie saugos & atitikties centro "PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell)". Jei naudojate MFA, peržiūrėkite šias instrukcijas: [prisijungimas prie saugos & atitikties centro "PowerShell" naudojant kelių dalių autentifikavimą](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell)
4. Panaikinkite laišką: paleiskite " `New-ComplianceSearchAction` cmdlet", kad panaikintumėte pranešimą. Pašalinti laiškai perkeliami į vartotojo atkuriamų elementų aplanką. Jei turite komandą pavyzdys, žiūrėkite [3 veiksmas: panaikinkite laišką.](https://docs.microsoft.com/office365/securitycompliance/search-for-and-delete-messages-in-your-organization)
