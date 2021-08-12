---
title: Kaip įtraukti ir valdyti administratorius – rekomenduojami veiksmai
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/07/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004114"
- "7194"
ms.openlocfilehash: 5aa6f11d31ed62078fdd05090af5722289544c5ab2244a369182f4e0f9214183
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 08/05/2021
ms.locfileid: "53963795"
---
# <a name="how-to-add-and-manage-administrators---recommended-steps"></a>Kaip įtraukti ir valdyti administratorius – rekomenduojami veiksmai

Atsižvelgdami į problemos aprašą, radome jums sprendimą. Dauguma klientų galėjo išspręsti savo problemą patys po mūsų dokumentų.

**Prenumeratos administratoriaus arba bendro administratoriaus redagavimas**

- Paskyros administratorius gali redaguoti abu vaidmenis, o prenumeratos administratorius gali keisti tik "Azure" portalo [bendradarbiavimo administratorius.](https://ms.portal.azure.com/#home)
- ["Azure" prenumeratos administratorių įtraukimas arba keitimas](https://docs.microsoft.com/azure/cost-management-billing/manage/add-change-subscription-administrator)

**Atnaujinkite prenumeratos administratorių arba Co-Administrator (AIRS) prenumeratas**

Tarnybos administratorius arba bendras administratorius gali savarankiškai atlikti šį veiksmą, atlikite šiuos veiksmus:

1. Prisijunkite prie ["Azure" portalo](https://ms.portal.azure.com/#home) ir **kairėje pusėje spustelėkite** Išlaidų valdymas + Atsiskaitymas.
2. Spustelėkite eilutės elementą su prenumerata. Atidaroma jūsų prenumeratos apžvalga.
3. Prenumeratos **ašmenyse** spustelėkite **Ypatybės**. 
4. Spustelėkite tarnybos **administravimo** mygtuką.
5. Įveskite vartotojo, kurį norite nustatyti kaip tarnybos administratorių, el. paštą ir spustelėkite **Gerai**.

**Add/Change/Remove Co-administrator**

1. Prisijunkite prie ["Azure" portalo](https://ms.portal.azure.com/#home) kaip tarnybos administratorius.
2. Atidarykite [Prenumeratos](https://ms.portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade) ir pasirinkite prenumeratą. (Bendrai administratoriams gali būti priskirti tik prenumeratos aprėptis.)
3. Eikite į "Access" valdiklis **(IAM)** Klasikiniai administratoriai Įtraukti bendro administratoriaus, kad atidarytumėte sritį Įtraukti bendro administratoriaus (Jei parinktis Įtraukti bendro administratoriaus išjungta, ji  >    >    >   nurodo, kad neturite teisių). 
4. Pasirinkite vartotoją, kurį norite įtraukti, ir spustelėkite **Įtraukti**.

**Sužinokite daugiau:**
- [Bendro administratoriaus įtraukimas](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [Bendro administratoriaus pašalinimas](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [Tarnybos administratoriaus keitimas](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [Paskyros administratoriaus rodinys](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [Prieigos valdymas naudojant "RBAC" ir "Azure" portalą](https://docs.microsoft.com/azure/role-based-access-control/role-assignments-portal)

**Vartotojų įtraukimas / naikinimas naudojant "Azure Active Directory" (AD)**

Galite įtraukti naujų vartotojų arba panaikinti esamus vartotojus iš savo ""Azure Active Directory" ("Azure AD") organizacijos:

1. Norėdami įtraukti naują vartotoją, prisijunkite prie ["Azure" portalo](https://ms.portal.azure.com/#home) kaip organizacijos vartotojo administratorius.
2. Pasirinkite **"Azure Active Directory"**, pasirinkite **Vartotojai,** tada spustelėkite **Naujas vartotojas**.
3. Puslapyje **Vartotojas** užpildykite reikiamą informaciją. Spustelėkite **Kurti**. Vartotojas sukuriamas ir įtraukiamas į "Azure AD" nuomotoją.

**Sužinokite daugiau:**

- [Naujo vartotojo įtraukimas](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory)
- [Vartotojo naikinimas](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory)
- [Vartotojo profilio informacijos įtraukimas arba atnaujinimas naudojant "Azure Active Directory"](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-users-profile-azure-portal)

**Rekomenduojami dokumentai**

- [Kas yra vaidmenimis pagrįstas prieigos valdiklis (RBAC)?](https://docs.microsoft.com/azure/role-based-access-control/overview)
- [Skirtingų vaidmenų "Azure" supratimas](https://docs.microsoft.com/azure/role-based-access-control/rbac-and-directory-admin-roles)
- [Administratoriaus vaidmens teisės "Azure Active Directory"](https://docs.microsoft.com/azure/active-directory/roles/permissions-reference)
- [Vadovėlis: prieigos suteikimas vartotojui naudojant RBAC ir "Azure" portalą](https://docs.microsoft.com/azure/role-based-access-control/quickstart-assign-role-user-portal)
- ["Azure" RBAC trikčių šalinimas](https://docs.microsoft.com/azure/role-based-access-control/troubleshooting)
- [Išteklių tvarkymas naudojant "Azure" valdymo grupes](https://docs.microsoft.com/azure/governance/management-groups/overview)
- [Kaip prašyti "Azure" sąskaitos faktūros kopijos el. paštu](https://azure.microsoft.com/en-us/blog/azure-email-invoices/)
- [Kaip įtraukti, atnaujinti arba pašalinti kredito arba debeto kortelę iš "Azure"](https://docs.microsoft.com/azure/cost-management-billing/manage/change-credit-card)
- [Manage (Reactivate/Cancel/Switch) subscription](https://docs.microsoft.com/azure/cost-management-billing/manage/subscription-disabled)



