---
title: "\"Privileged Identity Management\" vaidmuo"
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
ms.openlocfilehash: 358e446192e6b58ace81afa06e0d65ae3a207282351ffc3ec9975a24779951fb
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 08/05/2021
ms.locfileid: "53973237"
---
# <a name="privileged-identity-managementpim-role"></a>"Privileged Identity Management"(PIM) vaidmuo

**Suaktyvinus vaidmenį, teisės nėra suteikiamos**

Kai aktyvinate vaidmenį "Azure AD "Privileged Identity Management" (PIM), aktyvinimas gali būti ne iš karto išplatintas visuose portaluose, kuriems reikia privilegijuoto vaidmens. Kartais, net jei keitimas platinamas, žiniatinklio kaupimas portale gali atsirasti, kad pakeitimas iš karto įsigalios.

Jei aktyvinimas atidėtas, atlikite šiuos veiksmus:

1. Atsijungimas nuo "Azure" portalo ir vėl prisijunkite. Kai suaktyvinsite "Azure AD" vaidmenį arba "Azure" išteklių vaidmenį, matysite aktyvinimo etapus. Kai visi etapai bus užbaigti, matysite saitą Atsijungti. Šį saitą galite naudoti norėdami atsijungti. Tai išspręs daugumą aktyvinimo delsos atvejų.
2. PIM patikrinkite, ar esate nurodytas kaip vaidmens narys.
3. Jei aktyvinsite administratoriaus Exchange vaidmenį, įsitikinkite, kad atsijungi ir vėl prisijungsite. Jei problema išlieka, atidarykite palaikymo kvitą ir pakelkite tai kaip problemą. Jei naudojate savo Exchange administratoriaus vaidmenį, kad pasiektumėte saugos ir atitikties centrą, žr. kitą veiksmą.
4. Jei aktyvinsite vaidmenį, kad pasieksite saugos ir atitikties centrą arba suaktyvinsite "SharePoint" administratoriaus vaidmenį, suaktyvinsite uždelsimą nuo kelių minučių iki kelių valandų. Tai žinoma problema ir aktyviai dirbame su šiomis komandomis, kad kuo greičiau išspręssime šią problemą.

Daugiau informacijos rasite:

- ["Azure AD" vaidmenų aktyvinimas PIM](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-how-to-activate-role?WT.mc_id=Portal-Microsoft_Azure_Support "https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-how-to-activate-role?wt.mc_id=portal-microsoft_azure_support")
- ["Azure" išteklių vaidmenų aktyvinimas PIM](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-resource-roles-activate-your-roles?WT.mc_id=Portal-Microsoft_Azure_Support "https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-resource-roles-activate-your-roles?wt.mc_id=portal-microsoft_azure_support")

**Išjungus vaidmenį arba pasibaigus vaidmenų aktyvinimo galiojimui, teisės nepašalinmos**

Kai išjungiate vaidmenį "Azure AD "Privileged Identity Management" arba kai baigiasi vaidmenų aktyvinimo laikotarpis, gali būti delsa, kai ir toliau turite prieigą.

Jei jūsų išjungimas vėluoja, atlikite šiuos veiksmus:

1. Jei išjunginote "Exchange" administratoriaus vaidmenį arba baigiasi vaidmenų aktyvinimo laikotarpis ir pastebėsite, kad gerokai vėluojate prieš šalinant teises, atidarykite palaikymo kvitą ir praneškite palaikymo inžinieriui, kad jis padėtų jums pateikti bilietą su privilegijuotos prieigos valdymo (PAM) komanda "Office" apie šią problemą.
2. Jei aktyvinimo laikotarpis baigėsi, bet vis tiek atidarytas naršyklės seansas, uždarykite naršyklę. Galite toliau naudoti vaidmenį, kol uždarysite šį seansą. Tai žinoma problema ir mes ieškome galimo taisymo, kad būtų galima aktyviai atšaukti kiekvieną seansą pasibaigus aktyvinimo galiojimui.

Jei jūsų delsa skiriasi nuo šių dviejų scenarijų, atidarykite palaikymo kvitą.
