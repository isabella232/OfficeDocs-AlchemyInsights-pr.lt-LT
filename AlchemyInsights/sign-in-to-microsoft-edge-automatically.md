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
- "8333"
- "9004625"
ms.openlocfilehash: 6021991c125f5cb2a33ce8db8fe7717b528bf49b
ms.sourcegitcommit: 6bfe9cd9d0b18481e0cac6f1f5bc86ed7df31037
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 03/27/2021
ms.locfileid: "51398737"
---
# <a name="sign-in-to-microsoft-edge-automatically"></a>Automatinis prisijungimas prie "Microsoft Edge"

"Microsoft Edge" naudoja numatytąją OS paskyrą, kad automatiškai prisijungtų prie vartotojo pagal vartotojo įrenginio konfigūravimą. 

Toliau aprašyti kiekvieno įrenginio konfigūracijos tipo ir priklausomo vartotojo prisijungimo proceso scenarijai:

- **Įrenginys yra hibridinis / AAD-J**: Ši parinktis galima "Windows 10", "Windows" žemyn lygyje ir atitinkamose serverio versijose. Vartotojai automatiškai prisijungę naudodami savo "Azure Active Directory" (AD) paskyras.
- **Įrenginys yra prijungtas prie domeno:** ši parinktis pasiekiama "Windows 10", "Windows" žemyn lygyje ir atitinkamose serverio versijose. Pagal numatytuosius nustatymus vartotojai, kurie turi domeno paskyras, nėra automatiškai prisijungę; norėdami įgalinti automatinį jų prisijungimą, naudokite **strategiją ConfigureOnPremisesAccountAutoSignIn.** Norėdami įgalinti automatinį prisijungimą vartotojams, naudojantiems "Azure AD" paskyras, apsvarstykite galimybę hibridinį prisijungimą prie savo įrenginių.
- **Numatytoji OS** paskyra yra "Microsoft" paskyra: ši parinktis galima "Windows 10 RS3" (1709 versija, 10.0.16299 komponavimo versija) ir naujesnėse versijose. Tikėtina, kad scenarijus įvyks įmonės įrenginiuose. Tačiau jei OS numatytoji paskyra yra "Microsoft" paskyra, "Microsoft Edge" automatiškai prisijungs prie vartotojo naudodami "Microsoft" paskyrą.
 
 
