---
title: Automatinis prisijungimas prie "Microsoft Edge"
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003848"
- "6898"
ms.openlocfilehash: 68a1119abd0a3f687b6448bb6e58c6485c239c0f
ms.sourcegitcommit: 94036315916fbc79dca2a692c2e9bc1139dd28f6
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 12/08/2020
ms.locfileid: "49677768"
---
# <a name="sign-in-to-microsoft-edge-automatically"></a>Automatinis prisijungimas prie "Microsoft Edge"

"Microsoft Edge" naudoja numatytąjį OS abonementą, kad automatiškai prisijungtų vartotojui pagal vartotojo įrenginio konfigūraciją. 

Kiekvieno įrenginio konfigūracijos tipo ir jo priklausomo vartotojo prisijungimo proceso scenarijai aprašyti toliau:

1. **Įrenginys yra hibridinis/AAD-J**: Ši parinktis pasiekiama "Windows 10", "Windows 10", "Windows" ir atitinkamose serverio versijose. Vartotojai automatiškai pasirašomi naudojant "Azure Active Directory" (AD) paskyras.
2. **Įrenginys yra domeno prisijungęs**: Ši parinktis pasiekiama "Windows 10", "Windows 10", "Windows" ir atitinkamose serverio versijose. Pagal numatytuosius parametrą vartotojai, turintys domeno paskyras, automatiškai nepasirašomi; Norėdami įgalinti automatinį jų papildymą, naudokite " **Configureonpremisesaccountautosignin** " strategiją. Norėdami įgalinti automatinį prisijungimą vartotojams su "Azure AD" paskyromis, apsvarstykite galimybę naudoti hibridinius įrenginius.
3. **OS Numatytoji paskyra yra "Microsoft" abonementas**: Ši parinktis pasiekiama "Windows 10" RS3 (1709 versija, Komponavimo versija 10.0.16299) ir vėlesnės versijos. Vargu, ar scenarijus gali įvykti įmonės įrenginiuose. Tačiau jei OS numatytoji "Microsoft" paskyra yra "Microsoft" paskyra, tada "Microsoft Edge" automatiškai prisimins vartotoją su "Microsoft" abonementu.
 
 
