---
title: Atpažinimo ženklų pretenzijų ir atributų problemos
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
ms.openlocfilehash: 0c9827ee312d6b236c86f5a2973fa61fdc78c49b8565dd4ceb41f9a3a48140bc
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54012892"
---
# <a name="issues-with-token-claims-and-attributes"></a>Atpažinimo ženklų pretenzijų ir atributų problemos

**Atpažinimo ženklų pretenzijų naujinimas, konfigūravimas arba pašalinimas**

1. Naudodami "Azure Active Directory" ("Azure AD"), [](https://docs.microsoft.com/azure/active-directory/develop/active-directory-enterprise-app-role-management) galite tinkinti vaidmens reikalavimo tipą atsakymo atpažinimo žetone, kurį gaunate įgaliodami programą.
2. Programų kūrėjai gali naudoti pasirinktinius teiginius savo "Azure AD" programose, kad nurodytų, kuriuos teiginius jie nori naudoti atpažinimo ženkluose, siunčiamuose jų taikomai programai. Daugiau informacijos žr. [Pasirinktinių teiginių pateiktis jūsų programoje](https://docs.microsoft.com/azure/active-directory/develop/active-directory-optional-claims).
3. [Konfigūruokite programų grupės pretenzijas naudodami "Azure Active Directory"](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-fed-group-claims).
4. Jei naudojate sklandžią bendrąją afiksinę programą, žr. Tinkinkite [pretenzijas, išduotas "SAML" atpažinimo ženklu, skirtame įmonės programoms.](https://docs.microsoft.com/azure/active-directory/develop/active-directory-saml-claims-customization)

**Pretenzijų atributų susiejimas**

1. Norėdami konfigūruoti pretenzijų susiejimo strategiją naudodami "PowerShell", žr. Konkrečios programos atpažinimo žetonuose tinkinimas [nuomotojo (peržiūra)](https://docs.microsoft.com/azure/active-directory/develop/active-directory-claims-mapping).
2. Katalogų schemos plėtinių atributai suteikia galimybę saugoti papildomus duomenis "Azure Active Directory" vartotojų objektų ir kitų katalogų objektų, pvz., grupių, nuomotojo išsamios informacijos, tarnybos vadovo, duomenų saugykloje. Tik vartotojo objektų plėtinių atributai gali būti naudojami išleidžiant pretenzijas į taikomąsias programas. [Katalogų schemos plėtinių atributų naudojimas](https://docs.microsoft.com/azure/active-directory/develop/active-directory-schema-extensions) pretenzijose aprašo, kaip naudoti katalogų schemos plėtinių atributus siunčiant vartotojo duomenis į taikomąsias programas atpažinimo ženklų teiginiuose.

Daugiau informacijos apie atpažinimo ženklų pretenzijas žr.:

- [Pretenzijos prieigos atpažinimo ženklus](https://docs.microsoft.com/azure/active-directory/develop/access-tokens#claims-in-access-tokens)
- [Pretenzijos id_token](https://docs.microsoft.com/azure/active-directory/develop/id-tokens#claims-in-an-id_token)
- [Pretenzijos,](https://docs.microsoft.com/azure/active-directory-b2c/tokens-overview#claims) kurių galite tikėtis ID atpažinimo ženklus ir prieigos atpažinimo ženklus, išduotus "Azure AD B2C"
- [SAML atpažinimo ženklo pretenzijų nuoroda](https://docs.microsoft.com/azure/active-directory/develop/reference-saml-tokens)
