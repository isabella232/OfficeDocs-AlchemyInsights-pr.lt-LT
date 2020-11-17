---
title: Privilegijuotas tapatybės valdymo vaidmuo
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003230"
- "6825"
ms.openlocfilehash: 726511d016462f56c48a4272b57abc3e9f0cbc3d
ms.sourcegitcommit: 35e2c122d8a838d98d1f0851c29b16282261580f
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 11/17/2020
ms.locfileid: "49088879"
---
# <a name="privileged-identity-managementpim-role"></a>Privilegijuotos tapatybės valdymo (PIM) vaidmuo

**Teisės nesuteikiamos suaktyvinus vaidmenį**

Kai suaktyvinate "Azure AD" privilegijuoto tapatybės valdymo (PIM) vaidmenį, aktyvinimas gali būti iš karto išplatintas visiems portaluose, kuriems būtinas privilegijuotas vaidmuo. Kartais, net jei pakeitimai dauginami, žiniatinklio kaupimas svetainėje gali sukelti pakeitimus iš karto.

Jei aktyvinimas vėluoja, atlikite šiuos veiksmus:

1. Atsijunkite nuo "Azure" portalo ir vėl prisijunkite. Kai suaktyvinsite "Azure AD" vaidmenį arba "Azure" išteklių vaidmenį, matysite aktyvinimo etapus. Kai visi etapai bus baigti, matysite saitą Atsijungti. Galite naudoti šį saitą, kad atsijungtumėte. Tai padės išspręsti daugumą aktyvinimo vėlavimo atvejų.
2. "PIM" Patikrinkite, ar esate sąraše kaip vaidmens narys.
3. Jei aktyvinate "Exchange" administratoriaus vaidmenį, įsitikinkite, kad atsijungiate ir vėl prisijungsite. Jei problema kartojasi, atidarykite palaikymo bilietą ir iškelkite ją kaip problemą. Jei naudojate "Exchange" administratoriaus vaidmenį, kad pasiektumėte saugos ir atitikties centrą, peržiūrėkite paskesnį veiksmą.
4. Jei aktyvinate vaidmenį, kad pasiektumėte saugos ir atitikties centrą, arba jei aktyvinate "SharePoint" administratoriaus vaidmenį, nuo kelių minučių iki kelių valandų bus rodomas aktyvinimo vėlavimas. Tai žinoma problema ir mes aktyviai bendradarbiaujame su šiomis komandomis, kad kuo greičiau išspręstumėte šią problemą.

Daugiau informacijos rasite:

- ["Azure AD" vaidmenų aktyvinimas "PIM"](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-how-to-activate-role?WT.mc_id=Portal-Microsoft_Azure_Support "https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-how-to-activate-role?wt.mc_id=portal-microsoft_azure_support")
- ["Azure" išteklių vaidmenų aktyvinimas "PIM"](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-resource-roles-activate-your-roles?WT.mc_id=Portal-Microsoft_Azure_Support "https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-resource-roles-activate-your-roles?wt.mc_id=portal-microsoft_azure_support")

**Teisės nepašalinamos po to, kai deaktyvintas vaidmuo arba vaidmens aktyvinimas baigiasi**

Kai išjungsite vaidmenį "Azure AD" privilegijuotoje tapatybės tvarkyme arba pasibaigus vaidmenų aktyvinimo laikotarpiui, gali būti, kad galite atidėti "Access".

Jei jūsų aktyvinimas vėluoja, atlikite šiuos veiksmus:

1. Jei išjungsite "Exchange" administratoriaus vaidmenį arba suaktyvinate vaidmens aktyvinimo laikotarpį, o jūs pastebėjote reikšmingą vėlavimą prieš panaikinant teises, atidarykite palaikymo bilietą ir praneškite savo palaikymo inžinieriui, kad padėtumėte jums gauti bilietą su privilegijuoto "Access Management" (PAM) komanda, esanti "Office" "Office" apie šią problemą.
2. Jei baigėsi aktyvinimo laikotarpis, bet vis tiek atidaromas naršyklės seansas, uždarykite naršyklę. Galite toliau naudoti vaidmenį, kol uždarysite šį seansą. Tai žinoma problema ir mes ieškome galimų pataisų, kad aktyviai atšauktumėte kiekvieną seansą, kai aktyvinimas baigėsi.

Jei vėlavimas skiriasi nuo šių dviejų scenarijų, atidarykite palaikymo bilietą.
