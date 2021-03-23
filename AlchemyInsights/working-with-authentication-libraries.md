---
title: Darbas su autentifikavimo bibliotekomis
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/17/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9775"
- "9004342"
ms.openlocfilehash: f9f54ed2bfc5841df66d3e714112b9307455c182
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 03/19/2021
ms.locfileid: "51035827"
---
# <a name="working-with-authentication-libraries"></a>Darbas su autentifikavimo bibliotekomis

Norėdami išspręsti "Microsoft" autentifikavimo bibliotekos (MSAL) problemą, atlikite šiuos rekomenduojamus veiksmus:

1. **Darbas su MSAL**: ["Microsoft" tapatybės platformos autentifikavimo bibliotekos](https://docs.microsoft.com/azure/active-directory/develop/reference-v2-libraries) – šiame straipsnyje rodomas kelių taikomųjų programų tipų "Microsoft" autentifikavimo bibliotekos palaikymas. Jis turi saitų su bibliotekos šaltinio kodu; kur gauti paketo programos projektui; ir ar biblioteka palaiko vartotojo prisijungimą (autentifikavimas), prieigą prie apsaugotų žiniatinklio API (autorizavimą) arba abu.

2. **Autentifikavimo trikčių šalinimas**: msal palaiko kelis autentifikavimo srautus, skirtus naudoti skirtinguose taikomosios programos scenarijuose. Atsižvelgiant į tai, kaip jūsų kliento programa yra sukurta, MSAL gali naudoti vieną ar daugiau autentifikavimo srautų, kuriuos palaiko "Microsoft" tapatybės platforma. Šie srautai gali pateikti kelių tipų atpažinimo ženklus ir autorizavimo kodus ir reikalauti skirtingų žetonų, kad jie galėtų dirbti.

3. " **Access" žetonai**: ["Microsoft" tapatybės platformos prieigos žetonai](https://docs.microsoft.com/azure/active-directory/develop/access-tokens) – Sužinokite, kaip jūsų API gali patvirtinti ir naudoti "Access" atpažinimo ženklo teiginius. Visi šiame straipsnyje nurodyti dokumentai, išskyrus tuos atvejus, kai pažymėta, taikomi tik žetonams, kurie buvo išduoti jūsų įregistruotam API. Jis netaikomas žetonams, išduodamais "Microsoft" valdomoms API, taip pat šie žetonai negali būti naudojami norint patikrinti, kaip "Microsoft" tapatybės platforma pateiks Jūsų kuriamos API atpažinimo ženklus.

**"Azure Active Directory" autentifikavimo bibliotekos (ADAL) palaikymo pabaiga**

- **Nuo birželio 30 d., 2020,** mes nebeįtrauksime jokių naujų "adal" ir "Azure AD Graph" funkcijų. Mes toliau teiksime techninį palaikymą ir saugos naujinimus, bet nebeteiksime funkcijų naujinimų.
- **Nuo birželio 30 d., 2022,** mes užbaigsime "adal" ir "Azure AD Graph" palaikymą ir nebepateiks techninio palaikymo ar saugos naujinimų.
- Taikomosios programos, naudojančios ADAL esamą operacinės sistemos versiją, toliau veiks po šio laiko, bet negalės *gauti jokio techninio palaikymo ar saugos naujinimų*.
- Programos, naudojančios "Azure AD Graph", po šio laiko gali nebegauti atsakymų iš "Azure AD Graph" galinio punkto.

**ADAL perkėlimas**

- Rekomenduojame naujinti į MSAL, kuriame yra naujausios funkcijos ir saugos naujinimai.
- Jei naudojate "Microsoft" taikomąsias programas, žinokite, kad "Microsoft", siekdama perkelti savo taikomąsias programas į MSAL iki palaikymo termino pabaigos, užtikrins, kad jos bus naudingos naudojant MSAL esamą saugos ir funkcijų patobulinimus.

1. [Perskaitykite ADAL DUK](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq).
2. [Sužinokite, kaip perkelti taikomąsias programas pagal platformą](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#migration-guidance).
3. Jei perskaitę programos platformos vadovą turite papildomų klausimų, galite skelbti " [Microsoft" Q&A](https://docs.microsoft.com/answers/topics/azure-ad-adal-deprecation.html) su žymomis [Azure – AD-adal – nuteistųjų] arba atidaryti problemą bibliotekoje "GitHub" saugykloje. Peržiūrėkite " **Msal" apžvalgos** straipsnio skyrių [kalbos ir sistemos](https://docs.microsoft.com/azure/active-directory/develop/msal-overview#languages-and-frameworks) , kad būtų galima susieti su kiekviena biblioteka atpirkimo.
4. **Jei reikia pagalbos norint suprasti, kurios programos naudoja ADAL**, rekomenduojame Peržiūrėti visus savo programų šaltinio kodus. Jei reikia, susisiekite su visais nepriklausomais programinės įrangos tiekėjais (ISVs) arba taikomųjų programų teikėjais. „Microsoft“ palaikymo tarnyba taip pat gali pateikti visų jūsų nuomotojo ne „Microsoft“ ADAL programų sąrašą.







