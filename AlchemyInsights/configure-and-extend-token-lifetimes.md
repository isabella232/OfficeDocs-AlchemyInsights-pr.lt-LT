---
title: Simbolinis gyvenimo trukmės konfigūravimas ir išplėtimas
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/20/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7778"
- "9004351"
ms.openlocfilehash: 505e79ae9a163b89a6df2a7085480728bb0f1051
ms.sourcegitcommit: e378232f4c9ef4e962208100db752221e7bd2dd6
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 01/20/2021
ms.locfileid: "49917005"
---
# <a name="configure-and-extend-token-lifetimes"></a>Simbolinis gyvenimo trukmės konfigūravimas ir išplėtimas

Galite apibrėžti "Microsoft" tapatybės platformos išduoto prieigos, SAML arba ID atpažinimo ženklo galiojimo laiką. Galite nustatyti atpažinimo ženklų naudojimo visas savo organizacijos taikomąsias programas, kelių nuomotojų (kelių organizacijų) taikomąją programą arba konkrečią organizacijos pagrindinę tarnybą. Daugiau informacijos rasite [konfigūruotinas atpažinimo ženklų naudojimo laikas](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes).

Pavyzdžiuose rasite [pavyzdžių, kaip sukonfigūruoti atpažinimo ženklų naudojimo laiką](https://docs.microsoft.com/azure/active-directory/develop/configure-token-lifetimes).

Norėdami sužinoti, kaip sukonfigūruoti atpažinimo ženklo gyvavimo laiką ir suderinamumą "Azure Active Directory" B2C ("Azure AD B2C"), žiūrėkite " [Azure Active Directory" "B2C" esančių atpažinimo ženklų konfigūravimas](https://docs.microsoft.com/azure/active-directory-b2c/configure-tokens?pivots=b2c-user-flow).

Straipsnyje [Konfigūruokite seanso veikimą "Azure Active Directory](https://docs.microsoft.com/azure/active-directory-b2c/session-behavior?pivots=b2c-user-flow) " "B2C" aprašomi bendrosios AUTENTIFIKACIJOS (SSO) metodai, naudojami "AZURE ad B2C", ir padeda pasirinkti tinkamiausią SSO metodą konfigūruojant savo strategiją.

**Kiek laiko žetonai trunka? Kiek laiko galioja?**

Atpažinimo ženklų naudojimo laikas yra 1 valanda, o seanso trukmė – 24 valandos. Tai reiškia, kad jei per 24 valandas nebuvo pateikta jokių prašymų, prieš prašydami naujo atpažinimo ženklo turėsite vėl prisiregistruoti.

> [!NOTE]
> 2020 gegužės 30 d., "", joks naujas nuomotojas negalės naudoti Konfigūruotinos atpažinimo ženklo naudojimo strategijos, kad sukonfigūruotumėte seansą ir atnaujintų žetonų. Nuteistųjų bus įvykti per kelis mėnesius po to, o tai reiškia, kad mes sustabdysime esamą seansą ir atnaujinsime žetonų politikos kryptis. Vis dar galite sukonfigūruoti prieigos atpažinimo ženklo naudojimo laiką po nuteistųjų.






