---
title: Su atpažinimo ženklų reikalavimais ir atributais susijusios problemos
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
- "9004347"
- "7761"
ms.openlocfilehash: 4c12f768ab4bf4547f48abc19736743fa555c477
ms.sourcegitcommit: c1c6047ec467853dc823a17b02c461a6a476406d
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 01/27/2021
ms.locfileid: "50035966"
---
# <a name="issues-with-token-claims-and-attributes"></a>Su atpažinimo ženklų reikalavimais ir atributais susijusios problemos

**Atpažinimo ženklų reikalavimų naujinimas, konfigūravimas arba šalinimas**

1. Naudodami "Azure Active Directory" ("Azure AD"), atsakymų atpažinimo ženkle, kurį gaunate po to, kai įgaliojate taikomąją programą, galite [Tinkinti vaidmens reikalavimo tipą](https://docs.microsoft.com/azure/active-directory/develop/active-directory-enterprise-app-role-management) .
2. Taikomųjų programų kūrėjai savo "Azure AD" taikomosiose programose gali naudoti pasirinktines pretenzijas, kad nurodytų, kokius teiginius jie nori naudoti žetonams, siunčiamiems į jų taikomąją programą. Daugiau informacijos ieškokite [pasirinktinių reikalavimų pateikimas programėlei](https://docs.microsoft.com/azure/active-directory/develop/active-directory-optional-claims).
3. [Konfigūruokite "Azure Active Directory" taikomųjų programų grupės reikalavimus](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-fed-group-claims).
4. Jei naudojate sklandžią bendrąją autentifikacijos programą, žiūrėkite [Tinkinti reikalavimus, pateiktus "SAML" atpažinimo ženklo įmonėms taikomosiose programose](https://docs.microsoft.com/azure/active-directory/develop/active-directory-saml-claims-customization).

**Atributų atributo susiejimas**

1. Norėdami konfigūruoti pretenzijų atvaizdavimo strategiją naudodami "PowerShell", žiūrėkite [Tinkinti teiginius, pateiktus "Tokens" konkrečios programos nuomotojuje (peržiūra)](https://docs.microsoft.com/azure/active-directory/develop/active-directory-claims-mapping).
2. Katalogo schemos plėtinio atributai – tai būdas saugoti papildomus duomenis "Azure Active Directory" vartotojo objektams ir kitiems katalogo objektams, pvz., grupėms, nuomotojo duomenims, paslaugų direktams. Galima naudoti tik plėtinio atributus vartotojo objektuose. [Naudojant katalogų schemos plėtinio atributus teiginiams](https://docs.microsoft.com/azure/active-directory/develop/active-directory-schema-extensions) nurodoma, kaip naudoti katalogo schemos plėtinio atributus siunčiant vartotojo duomenis į taikomąsias programas atpažinimo ženklų ieškiniams.

Daugiau informacijos apie simbolinius teiginius rasite:

- ["Access" atpažinimo ženklų pretenzijos](https://docs.microsoft.com/azure/active-directory/develop/access-tokens#claims-in-access-tokens)
- [Ieškiniai id_token](https://docs.microsoft.com/azure/active-directory/develop/id-tokens#claims-in-an-id_token)
- [Teigia](https://docs.microsoft.com/azure/active-directory-b2c/tokens-overview#claims) , kad galite tikėtis ID atpažinimo ženklai ir prieigos žetonai, kuriuos išleido "Azure AD" B2C
- [SAML atpažinimo ženklo pretenzijų nuoroda](https://docs.microsoft.com/azure/active-directory/develop/reference-saml-tokens)
