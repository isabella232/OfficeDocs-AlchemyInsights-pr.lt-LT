---
title: Problemos naudojant Intune administratoriaus konsolę
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/29/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1790"
- "9000214"
ms.openlocfilehash: 7a36d502a92d360b06336ccfa6183f666f0260ab
ms.sourcegitcommit: ffbed67c0a16ec423fa1d79b71e48ea4e2d320e1
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 07/29/2020
ms.locfileid: "46555386"
---
# <a name="problems-using-the-intune-admin-console"></a>Problemos naudojant Intune administratoriaus konsolę

**"Prieiga uždrausta" naršant Intune administravimo portale.**

- Jei esate "Intune" pasirinktinio vaidmens narys, įsitikinkite, kad jūsų abonementui priskirta "Intune" arba "Enterprise Mobility Suite" (EMS) licencija.
- Jei naudojate konfigūracijos tvarkyklė valdyti įrenginius, patikrinkite, ar nesate dalis Intune vartotojų rinkinio konfigūracijos tvarkytuvo MDM.
- Patikrinkite, ar jums buvo priskirtos atitinkamos vaidmenimis pagrįstos administravimo kontrolės (RBAC) teisės intune vaidmenų ašmenys.
- Patikrinkite, ar naudojama grupė nėra siuntimo sąrašas. Intune Azure portalas palaiko tik vartotojų abonementus, kurie priklauso Azure Active Directory saugos grupes. Peržiūrėkite savo grupes "Azure" portale > **"Intune**  >  **Groups"** arba "Azure" portale > **"Azure Active Directory".**

**Vartotojas turi per daug priskirtų intune vaidmens teisių**

Patarkite vartotojui eiti į **Intune**  >  **Intune vaidmenis**  >  **Mano teisės**  >  **Eksportuoti,** kad peržiūrėtumėte suteiktas teises.

**Į vaidmenį įtraukiau aprėpties grupę, bet to vaidmens vartotojai vis dar mato kitus vartotojus arba įrenginius.**

Aprėpties grupės neišfiltruoja vartotojų arba įrenginių. Aprėpties grupės:

- Apribokite, kam vartotojai gali priskirti strategijas arba programas.
- Leisti tik konkretiems vartotojams vykdyti nuotolines užduotis įrenginiuose.

Daugiau informacijos apie aprėpties grupes ieškokite [Vaidmenimis pagrįstas prieigos valdymas (RBAC) su "Microsoft Intune".](https://docs.microsoft.com/intune/role-based-access-control)

**Aš pridėjo vartotoją Intune vaidmenį, bet jie vis dar turi visišką prieigą prie Intune admin konsolės.**

Eikite į Intune > **vartotojai** Azure portalas ir patikrinkite, ar vartotojas nėra priskirtas bet kurį iš šių vaidmenų Azure portalas:

- Visuotinis administratorius
- Intune tarnybos administratorius
- "SharePoint" administratorius

Daugiau informacijos ieškokite [Vaidmenimis pagrįstas prieigos valdymas (RBAC) su "Microsoft Intune".](https://docs.microsoft.com/intune/role-based-access-control)

**Prieigos problemos**

Daugiau informacijos rasite [Negalite prisijungti prie "Office 365", "Azure" arba "Intune".](https://support.microsoft.com/help/2412085/you-can-t-sign-in-to-office-365-azure-or-intune)