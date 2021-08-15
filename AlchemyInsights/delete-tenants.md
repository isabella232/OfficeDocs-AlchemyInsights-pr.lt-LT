---
title: Naikinti nuomotoją
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 11/23/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003256"
- "7297"
ms.openlocfilehash: 7377f77b7295e8134673c9a46fa7606842d4df949f535878d13986c6d39d0b5e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 08/05/2021
ms.locfileid: "53993901"
---
# <a name="delete-tenant"></a>Naikinti nuomotoją

Norėdami panaikinti "Azure AD", įsitikinkite, kad:
- Esate visuotinis administratorius kataloge.
- Esate PRISIJUNGĘ NAUDODAMI paskyrą, kurios numatytasis katalogas, pvz., contoso.onmicrosoft.com, yra prisijungusioje paskyroje, pvz., admin@contoso.onmicrosoft.com.
- Pašalinkite visas aktyvias taikomąsias programas kataloge prieš naikinimą. Norėdami pašalinti aktyvias taikomąsias programas, eikite į Taikomųjų programų registracijos ir pašalinkite esamas taikomąsias programas.
- Nėra aktyvių "Microsoft Online Services" prenumeratų, pvz., "Microsoft Azure", "Office 365" arba "Azure AD Premium, susietų kataloge. Perduokite prenumeratas arba paspartinkite aktyvių prenumeratų atšaukimą per "Azure" palaikymą ir atsiskaitymą. Sužinokite daugiau apie kaip atšaukti "Office 365 "Azure" prenumeratas. Patarimų, kaip susieti arba įtraukti esamą prenumeratą į nuomotoją, žr. "Azure" prenumeratos susiejimas arba įtraukimas [į "Azure AD" nuomotoją](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-how-subscriptions-associated-directory).
- Nėra aktyvios licencijos. Norėdami pašalinti licencijas, [žr. Kaip pašalinti prenumeratą, kad pašalintumėte licenciją](https://docs.microsoft.com/azure/active-directory/enterprise-users/directory-delete-howto#delete-a-subscription).
- Bandant panaikinti "Azure AD", kataloge nėra kitų aktyvių vartotojų kaip visuotinis administratorius. Taip pat reikia pašalinti visus kitus aktyvius vartotojus ir priklausomybes nuo pasirinktinio domeno vardo nuomotojo, pvz., vartotojus, sukurtus naudojant admin@contoso.com.

Daugiau informacijos apie tai, kaip atlikti šiuos veiksmus:
- Panaikinkite ""Azure Active Directory"" arba "prenumeratą", [žr. Naikinti "Azure Active Directory"](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-delete-howto).
- Šalinant taikomąsias programas kataloge, [žr. Programų šalinimas](https://docs.microsoft.com/azure/active-directory/develop/quickstart-remove-app). 
