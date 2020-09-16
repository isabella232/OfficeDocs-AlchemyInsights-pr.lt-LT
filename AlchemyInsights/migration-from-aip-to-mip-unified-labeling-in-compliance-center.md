---
title: Perkėlimas iš Ail į MIK/suvienodintas žymėjimas atitikties centre
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002278"
- "5114"
ms.openlocfilehash: 7157eada10db2443f64fb7925f408359275d75eb
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47674334"
---
# <a name="migration-from-aip-to-mipunified-labeling-in-the-compliance-center"></a>Perkėlimas iš Ail į MIK/suvienodintas žymėjimas atitikties centre

Norėdami perkelti iš Ail etikečių į saugos ir atitikties centro suvienodintą ženklinimą, atlikite šiuos veiksmus:

**Apsaugos aktyvinimas iš "Azure" portalo**

1. Jei to dar nepadarėte, atidarykite naują naršyklės langą ir [Prisijunkite prie "Azure" portalo](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#signing-in-to-the-azure-portal). Pereikite prie " **Azure" informacijos apsaugos** ašmenų. Pvz., meniu koncentratorius spustelėkite **Visos tarnybos** ir pradėkite vesti **informaciją** lauke filtras. Pasirinkite **Azure informacijos apsauga**. Jei anksčiau neprisijungėte prie "Azure" informacijos apsaugos disko, peržiūrėkite [papildomus veiksmus](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#to-access-the-azure-information-protection-blade-for-the-first-time) , kad įtrauktumėte šį diską į portalą. Norėdami atidaryti "Azure" informacijos apsaugos diską, turite turėti " [Azure" informacijos apsaugos priemokų planą](https://www.microsoft.com/cloud-platform/azure-information-protection-pricing) arba "Office 365" planą, apimantį teisių valdymą. Jei turite vieną iš šių prenumeratų, bet matote pranešimą, kad nepavyksta rasti galiojančios prenumeratos, [kreipkitės į "Microsoft" palaikymo tarnybą](https://docs.microsoft.com/azure/information-protection/get-started/information-support#to-contact-microsoft-support) arba naudokite standartinius palaikymo kanalus.

2. Raskite meniu **tvarkyti** parinktis ir pasirinkite **apsaugos aktyvinimas**. Spustelėkite **Aktyvinti**, tada patvirtinkite savo veiksmą. Kai aktyvinimas baigtas, informacijos juostoje rodoma **sėkmingai baigta aktyvinti**.

**"Azure" informacijos apsaugos žymų perkėlimas į "Office 365" saugos & atitikties centras**

1. Įsitikinkite, kad esate prisijungęs kaip vartotojas su visuotinio administratoriaus teisėmis.

2. Pereikite prie " **Azure" informacijos apsaugos** ašmenų.

3. Meniu **valdyti** parinktį pasirinkite **Bendrasis žymėjimas**.

4. " **Azure" informacijos apsauga – bendrasis etiketės** peilis spustelėkite **Aktyvinti** ir vykdykite internetines instrukcijas.

**Pastaba**: patikrinkite, ar turite atitinkamas teises prieš suaktyvindami saugos & atitikties centro perkėlimą. Daugiau informacijos ieškokite šiuose straipsniuose:

1. [Ar reikia būti visuotiniu administratoriumi, kad sukonfigūruotumėte Azure informacijos apsaugą arba galėčiau perduoti kitiems administratoriams?](https://docs.microsoft.com/azure/information-protection/faqs#do-you-need-to-be-a-global-admin-to-configure-azure-information-protection-or-can-i-delegate-to-other-administrators)

2. [Svarbi informacija apie administracinius vaidmenis perkėlus į saugos & atitikties centrą.](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels#important-information-about-administrative-roles)

Daugiau informacijos apie PPK, kad būtų galima suvienodinti perkėlimo į saugos ir atitikties centrą, ieškokite [etikečių perkėlimas](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels).
