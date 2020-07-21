---
title: Naikinti pavienį vartotoją iš vietinio serverio
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/20/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1725"
- "9000179"
ms.openlocfilehash: 7927c0684d2f5289f92506d7d05d5b1a3b43b658
ms.sourcegitcommit: b0b050a83db28566b68e3ec09810c6b94280008e
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 07/20/2020
ms.locfileid: "45198180"
---
# <a name="delete-orphaned-user-from-on-premises-server"></a>Naikinti pavienį vartotoją iš vietinio serverio

Norėdami pašalinti pavienį vartotoją, atlikite šiuos veiksmus:

1. Priversti katalogų sinchronizavimas vadovaudamiesi instrukcijomis [Kas yra hibridinė tapatybė su Azure Active Directory?](https://technet.microsoft.com/library/jj151771.aspx#bkmk_synchronizedirectories).

2. Norėdami patikrinti katalogų sinchronizavimą, peržiūrėkite [Kas yra hibridinė tapatybė su Azure Active Directory?](https://technet.microsoft.com/library/jj151797.aspx).

3. Jei sinchronizavimas veikia tinkamai, bet Active Directory objekto naikinimas nėra platinti Azure AD, rankiniu būdu pašalinti pavienių objektą naudodami vieną iš šių Azure Active Directory modulis, skirtas "Windows PowerShell" cmdlet:

    Pašalinti-MsolKontaktas  
    Šalinti MsolGroup  
    Pašalinti MsolUser

    Pvz., norėdami pašalinti našlaičiai vartotojo ID john.smith@contoso.com, iš pradžių sukurtas naudojant katalogų sinchronizavimą, vykdykite cmdlet:

    Pašalinti MsolUser –UserPrincipalName John.Smith@Contoso.com