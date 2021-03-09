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
ms.openlocfilehash: ab491e883ab294f08d0b5d2e686dc059b468d29f
ms.sourcegitcommit: bd6a9cb5d357baee5134c0dea430afc2a035c810
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 03/09/2021
ms.locfileid: "50568298"
---
# <a name="proxy-address-error-while-creating-a-mailbox-or-other-email-enabled-object"></a>Tarpinio serverio adreso klaida kuriant pašto dėžutę arba kitą objektą, kuriam įgalintas el. paštas

Jei bandėte kurti el. pašto funkciją palaikantį objektą (pašto dėžutę, bendrinamą pašto dėžutę ir kt.) ir gavote klaidos pranešimą "tarpinio serverio adresas" SMTP:alias@domain.com "jau naudojamas...", jūsų pasirinktas elektroninio pašto adresas jau yra įtrauktas į kitą jūsų organizacijoje esantį objektą, kuriame įgalintas el. laiškas.
  
Jums reikia surasti vartotoją, grupę, bendrinamą pašto dėžutę arba viešąjį aplanką, kuriame yra šis elektroninio pašto adresas ir jį panaikinti arba pakeisti jo elektroninio pašto adresą. Tada galite sukurti naują el. pašto objektą su atlaisvintomis el. pašto adresu. Naudokite iešką pagrindiniame puslapyje, kad ją rastumėte. Taip pat galite naudoti šią "Exchange Online PowerShell" komandą, kad galėtumėte ją rasti:

`
    Get-EXORecipient -Filter "EmailAddresses -eq 'email@contoso.onmicrosoft.com'"
`
  
Jei nenorite panaikinti esamo elektroninio pašto adreso, pasirinkite naują naujo objekto, kurį kuriate, elektroninio pašto adresą.
  