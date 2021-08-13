---
title: Tarpinio serverio adreso klaida kuriant bendrinamą pašto dėžutę
ms.author: pebaum
author: CrystalThomasMS
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ece4bcce-1053-4ed3-a194-9d0af8f73c6f
ms.custom:
- "19"
- "6"
ms.openlocfilehash: 7c15d5db5445fbe4c3ec22878f180f48d2da4f90369f2e6f223916646eb19c12
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54062916"
---
# <a name="proxy-address-error-while-creating-a-mailbox-or-other-email-enabled-object"></a>Tarpinio serverio adreso klaida kuriant pašto dėžutę arba kitą objektą su įgalinta el. pašto funkcija

Jei bandėte sukurti objektą, palaikantį el. paštą (pašto dėžutę, bendrinamą pašto dėžutę ir t. t.) ir gavote klaidą "Tarpinio serverio adresas "SMTP:alias@domain.com" jau naudojamas...", jūsų pasirinktą el. pašto adresą jau naudoja kitas organizacijos objektas, palaikantis el. paštą.
  
Turite rasti vartotoją, grupę, bendrinamą pašto dėžutę arba viešąjį aplanką, kuriame yra šis el. pašto adresas, ir jį panaikinti arba pakeisti savo el. pašto adresą. Tada galėsite sukurti naują objektą, palaikantį el. paštą su laisvu el. pašto adresu. Naudokite iešką pagrindiniame puslapyje, kad ją rastumėte. Taip pat galite naudoti šią Exchange Online "PowerShell" komandą, kad jos ieškote:

`
    Get-EXORecipient -Filter "EmailAddresses -eq 'email@contoso.onmicrosoft.com'"
`
  
Jei nenorite panaikinti esamo el. pašto adreso, pasirinkite naują kuriamo objekto el. pašto adresą.
  