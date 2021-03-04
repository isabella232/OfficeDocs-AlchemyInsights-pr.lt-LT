---
title: SSPR trikčių šalinimas
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/04/2021
ms.topic: article
ms.audience: Admin
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003259"
- "6128"
ms.openlocfilehash: 85bfc812dcffce008a6fa5394a6069bd64c514d6
ms.sourcegitcommit: f4ba304b92ed01e35273ecda67e9dc3ad9d475c1
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 03/04/2021
ms.locfileid: "50430221"
---
# <a name="troubleshoot-sspr"></a>SSPR trikčių šalinimas

**Kilo problemų konfigūruojant slaptažodžio nustatymą iš naujo**

- Jei esate administratorius ir ieškote, kaip įgalinti savitarnos slaptažodžio nustatymą iš naujo, žiūrėkite [Susipažinkite įgalinti SSPR](https://docs.microsoft.com/azure/active-directory/authentication/tutorial-enable-sspr), konfigūruoti savo organizacijos slaptažodį iš naujo. Taip pat galite peržiūrėti [licencijavimo reikalavimus](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-licensing?WT.mc_id=Portal-Microsoft_Azure_Support). Turite turėti bent vieną licenciją, priskirtą jūsų organizacijoje.
    - **Tik debesies vartotojai** – bet kuris "Office 365" (O365) sumokėtas SKU arba "Azure AD Basic"
    - **Debesies ir (arba) vietiniai vartotojai – "** Azure AD Premium" P1 arba P2, įmonės mobilumas + sauga (EPS) arba saugi gamybinė įmonė (SPE)
- Jei turite papildomų klausimų apie savitarnos slaptažodžio nustatymą iš naujo, peržiūrėkite [mūsų DUK](https://docs.microsoft.com/azure/active-directory/authentication/active-directory-passwords-faq?WT.mc_id=Portal-Microsoft_Azure_Support).

**Gaunu klaidos pranešimą**

Peržiūrėkite šį straipsnį, kad rastumėte įprastas klaidas ir jų sprendimus: [savitarnos slaptažodžio nustatymo iš naujo trikčių šalinimas](https://docs.microsoft.com/azure/active-directory/authentication/active-directory-passwords-troubleshoot?WT.mc_id=Portal-Microsoft_Azure_Support)

**Iškilo problema dėl slaptažodžio nustatymo iš naujo strategijos**

- Jei slaptažodžio nustatymo iš naujo strategija veikia ne taip, kaip tikėtasi, arba jei turite klausimų apie slaptažodžio nustatymo iš naujo strategijas, Peržiūrėkite šį straipsnį: [slaptažodžių strategijos ir "Azure Active Directory" apribojimai](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support).
- Slaptažodžio nustatymo iš naujo strategijos netaikomos administratoriams. "Microsoft" užtikrina, kad "Azure" administratoriaus vaidmuo būtų stipri numatytoji dviejų vartų slaptažodžio nustatymo iš naujo strategija. Įsitikinkite, kad testuojate vartotoją, kuris nėra administratorius. Daugiau informacijos apie administratoriaus nustatymo iš naujo strategiją ieškokite šiame straipsnyje: [administratoriaus iš naujo nustatyti strategijos skirtumus](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support#administrator-reset-policy-differences).

**Nenoriu, kad mano vartotojai užregistruotų papildomos saugos informacijos apie slaptažodžio nustatymą iš naujo**

Galite iš anksto įvesti duomenis (elektroninio pašto ir telefono atributus), kad vartotojai galėtų naudotis API, "PowerShell" arba "Azure AD Connect". Norėdami sužinoti, kaip skaityti:

- [Slaptažodžio nustatymo iš naujo diegimas nereikalaujant vartotojų registruotis](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support#set-and-read-authentication-data-using-powershell)
- [Kokius duomenis naudoja slaptažodžio nustatymas iš naujo](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support)

**Noriu, kad vartotojai registruotų savo papildomą saugos informaciją, skirtą slaptažodžiui nustatyti iš naujo**

1. Ar jūsų vartotojai užregistruoja savo saugos informaciją savitarnos slaptažodžio nustatymo iš naujo, nukreipdami juos į " [aka.ms/ssprsetup](https://mysignins.microsoft.com/security-info)".
1. Kai duomenys bus pateikti vartotojui (vartotojas arba administratorius), nukreipkite vartotoją į " [aka.ms/SSPR](https://passwordreset.microsoftonline.com/) ", kad jūsų vartotojai galėtų būti įgalioti iš naujo nustatyti savo slaptažodžius.
1. Jei vartotojai vis dar patiria problemų, jie greičiausiai yra **susietieji** arba **slaptažodžių maišos sinchronizuoti** vartotojai. Tai reiškia, kad iškilo problema dėl slaptažodžio įrašymo tarnybos.