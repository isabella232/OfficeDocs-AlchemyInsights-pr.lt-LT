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
ms.openlocfilehash: aa1525c6d221dbcfe91da7abd3d094ae1c228ece
ms.sourcegitcommit: 0f42d1600b6845083f0273d14c1d9e59344e4371
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 11/30/2020
ms.locfileid: "49564616"
---
# <a name="delete-tenant"></a>Naikinti nuomotoją

Norėdami panaikinti "Azure AD", įsitikinkite, kad:
- Esate visuotinis administratorius kataloge.
- Nesate prisijungę naudodami paskyrą, kurioje yra numatytasis katalogas, pvz., "contoso.onmicrosoft.com", prisijungęs prie paskyros, pvz., "admin@contoso.onmicrosoft.com".
- Pašalinkite visas aktyvias taikomąsias programas kataloge prieš ištrindami. Norėdami pašalinti aktyvias taikomąsias programas, pereikite prie taikomųjų programų registracijų ir pašalinkite esamas taikomąsias programas.
- Nėra jokių aktyvių "Microsoft Online Services" prenumeratų, pvz., "Microsoft Azure", "Office 365" arba "Azure AD Premium". Perkelkite savo prenumeratas arba Paspartinkite aktyvių prenumeratų panaikinimą naudodami "Azure" palaikymą ir atsiskaitymą. Sužinokite daugiau, kaip atšaukti "Office 365" ir "Azure" prenumeratas. Nurodymų, kaip susieti arba įtraukti esamą prenumeratą į nuomotoją, ieškokite "Azure [AD" nuomotojui susiekite arba įtraukite "Azure" prenumeratą](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-how-subscriptions-associated-directory).
- Nėra aktyvios licencijos. Norėdami pašalinti licencijas, Sužinokite, [kaip pašalinti prenumeratą, kad pašalintumėte licenciją](https://docs.microsoft.com/azure/active-directory/enterprise-users/directory-delete-howto#delete-a-subscription).
- Kataloge nėra kitų aktyvių vartotojų, išskyrus save kaip visuotinį administratorių, bandant panaikinti "Azure AD". Pašalinti visus kitus aktyvius vartotojus ir bet kurią priklausomybes, esančias pasirinktinio domeno varde nuomotojuje, taip pat reikės pašalinti, pvz., "admin@contoso.com" sukurtus vartotojus.

Daugiau informacijos apie tai, kaip:
- Naikinti "Azure Active Directory" arba "prenumerata", rasite " [Azure Active Directory" naikinimas](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-delete-howto).
- Pašalinti taikomąsias programas kataloge rasite [taikomųjų programų šalinimas](https://docs.microsoft.com/azure/active-directory/develop/quickstart-remove-app). 
