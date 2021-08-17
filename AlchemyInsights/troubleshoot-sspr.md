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
ms.openlocfilehash: 9d8184efdc60befd359059c62ea3eb1a14ad7d2a20dade921d4a71e424f52033
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54038966"
---
# <a name="troubleshoot-sspr"></a>SSPR trikčių šalinimas

**Kyla problemų konfigūruojant slaptažodžio nustatymo iš naujo**

- Jei esate administratorius ir ieškote, kaip įgalinti savitarnos slaptažodžio nustatymo iš naujo funkciją, [žr. Vadovėlis, įgalinęs SSPR](https://docs.microsoft.com/azure/active-directory/authentication/tutorial-enable-sspr), ir konfigūruokite savo organizacijos slaptažodžio nustatymo iš naujo parametrus. Taip pat galite peržiūrėti [licencijavimo reikalavimus.](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-licensing?WT.mc_id=Portal-Microsoft_Azure_Support) Turite turėti bent vieną licenciją, priskirtą jūsų organizacijoje.
    - **Tik debesies vartotojai** – bet Office 365 (O365) sumokėjo SKU arba "Azure AD Basic"
    - **Debesies ir (arba)** vietinės vartotojų – "Azure AD Premium P1 arba P2, Enterprise Mobility + Security (EMS) arba Secure Productive Enterprise (SPE)
- Jei reikia papildomų klausimų apie savitarnos slaptažodžio nustatymo iš naujo nustatymus, [peržiūrėkite duktus](https://docs.microsoft.com/azure/active-directory/authentication/active-directory-passwords-faq?WT.mc_id=Portal-Microsoft_Azure_Support).

**Gaunu klaidos pranešimą**

Peržiūrėkite šį straipsnį, kad rastumėte dažnai pasitaikančių klaidų ir jų sprendimų: [Savitarnos slaptažodžio nustatymo iš naujo trikčių šalinimas](https://docs.microsoft.com/azure/active-directory/authentication/active-directory-passwords-troubleshoot?WT.mc_id=Portal-Microsoft_Azure_Support)

**Kyla problemų dėl slaptažodžio nustatymo iš naujo strategijos**

- Jei jūsų slaptažodžio nustatymo iš naujo strategija neveikia taip, kaip tikėtasi, arba jei turite klausimų apie slaptažodžio nustatymo iš naujo strategijas, peržiūrėkite šį straipsnį: Slaptažodžių strategijos [ir apribojimai "Azure Active Directory"](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support).
- Slaptažodžių nustatymo iš naujo strategijos netaikomos administratoriams. "Microsoft" užtikrina griežtą numatytąją "Azure" administratoriaus vaidmens dviejų vartų slaptažodžio nustatymo iš naujo strategiją. Įsitikinkite, kad testavote su vartotojui, kuris nėra administratorius. Daugiau informacijos apie administratoriaus nustatymo iš naujo strategiją žr. šiame straipsnyje: [Administratorius iš naujo nustato strategijos skirtumus.](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support#administrator-reset-policy-differences)

**Nenoriu, kad mano vartotojai užregistruos papildomą saugos informaciją, kad galėtų nustatyti slaptažodį iš naujo**

Galite iš anksto įvesti duomenis (el. pašto ir telefono atributus) vartotojams naudodami API, "PowerShell" arba "Azure AD" Prisijungimas. Norėdami sužinoti, kaip skaityti:

- [Slaptažodžio nustatymo iš naujo diegimas nereikalaujant vartotojų registruotis](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support#set-and-read-authentication-data-using-powershell)
- [Kokie duomenys naudojami iš naujo nustačius slaptažodį](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support)

**Noriu, kad mano vartotojai užregistruotų papildomą saugos informaciją, kad galėtų nustatyti slaptažodį iš naujo**

1. Nustatykite, kad jūsų vartotojai užregistruotų savo savitarnos slaptažodžio nustatymo iš naujo saugos informaciją, nukreipiant [juos į aka.ms/ssprsetup](https://mysignins.microsoft.com/security-info).
1. Kai vartotojo (vartotojo arba administratoriaus) duomenys užpildomi, nustatykite vartotojui [aka.ms/sspr,](https://passwordreset.microsoftonline.com/) kad jūsų vartotojai galėtų būti įgalioti iš naujo nustatyti savo slaptažodžius.
1. Jei vartotojai vis dar susiduria su problemomis, jie greičiausiai **yra išoriniai** arba **slaptažodžių hash synched** vartotojai. Tai reiškia, kad gali kilti problemų dėl slaptažodžio įrašymo paslaugos.