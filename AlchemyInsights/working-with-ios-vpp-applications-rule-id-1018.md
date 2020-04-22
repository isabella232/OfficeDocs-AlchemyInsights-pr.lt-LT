---
title: Darbas su "iOS" VPP taikomųjų programų id 1018
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1018"
- "6700004"
ms.assetid: 2e51ae64-8ba2-42e1-9e3e-f4aad102c391
ms.openlocfilehash: 88a1ef66bf337b3a0094976c122330591aee77ff
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 04/22/2020
ms.locfileid: "43719965"
---
# <a name="working-with-ios-vpp-applications"></a>Darbas su "iOS" VPP programomis

Skaitykite [Kaip valdyti "iOS" programėles, įsigytas naudojant tomo pirkimo programą su "Microsoft Intune",](https://docs.microsoft.com/intune/vpp-apps-ios) kad sužinotumėte apie funkcijas, apribojimus ir veiksmus, kaip pasinaudoti "Apple Volume Purchase" programa ir jos palaikymu programoje "Microsoft Intune".
  
 **Dažniausiai pasitaikančios problemos:** "Priskiriau "iOS VPP" programą savo vartotojams, bet diegimas nepavyko."
  
- Taip gali nutikti, jei keliuose mobiliųjų įrenginių valdymo paslaugų teikėjuose naudojamas vienas VPP atpažinimo ženklas. VPP atpažinimo ženklus iš "Apple" galima naudoti tik su vienu teikėju. Jei naudojote VPP atpažinimo ženklą su keliais teikėjais, turite iš naujo nusiųsti atpažinimo ženklą į Intune.

- Diegimas taip pat gali nepavykti, jei bendras įrenginių skaičius viršija licencijų skaičių. Norėdami peržiūrėti licencijų naudojimo ataskaitą, eikite į puslapį **"Intune Mobile Apps"** \> **licencijos.** Norėdami sužinoti, kaip susigrąžinti naudojamas licencijas, skaitykite [šį straipsnį.](https://docs.microsoft.com/intune/vpp-apps-ios#revoking-app-licenses-and-deleting-tokens)
