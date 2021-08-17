---
title: Prisijungimas prie Microsoft Edge automatiškai
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
ms.openlocfilehash: 4e069a1c75caabf3bef7387140edd5650cf966856b888b5c6b5618a603986d6d
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54050702"
---
# <a name="sign-in-to-microsoft-edge-automatically"></a>Prisijungimas prie Microsoft Edge automatiškai

Microsoft Edge naudoja numatytąją OS paskyrą, kad automatiškai prisijungtų prie vartotojo pagal vartotojo įrenginio konfigūravimą. 

Toliau aprašyti kiekvieno įrenginio konfigūracijos tipo ir priklausomo vartotojo prisijungimo proceso scenarijai:

- **Įrenginys yra hibridinis / AAD-J**: Ši parinktis galima Windows 10, žemyn lygio Windows ir atitinkamose serverio versijose. Vartotojai automatiškai prisijungę naudodami savo "Azure Active Directory" (AD) paskyras.
- **Įrenginys yra prijungtas prie** domeno: ši parinktis galima Windows 10, žemyn lygio Windows ir atitinkamose serverio versijose. Pagal numatytuosius nustatymus vartotojai, kurie turi domeno paskyras, nėra automatiškai prisijungę; norėdami įgalinti automatinį jų prisijungimą, naudokite **strategiją ConfigureOnPremisesAccountAutoSignIn.** Norėdami įgalinti automatinį prisijungimą vartotojams, naudojantiems "Azure AD" paskyras, apsvarstykite galimybę hibridinį prisijungimą prie savo įrenginių.
- **Numatytoji OS** paskyra yra "Microsoft" paskyra: ši parinktis galima "Windows 10 RS3" (1709 versija, komponavimo versija 10.0.16299) ir naujesnėse versijose. Tikėtina, kad scenarijus įvyks įmonės įrenginiuose. Tačiau jei OS numatytoji paskyra yra "Microsoft" paskyra, Microsoft Edge automatiškai prisijungsite prie vartotojo naudodami "Microsoft" paskyrą.
 
 
