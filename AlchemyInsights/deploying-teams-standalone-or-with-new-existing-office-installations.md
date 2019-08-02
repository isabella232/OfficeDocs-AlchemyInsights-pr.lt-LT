---
title: Diegti komandos kaip atskirą arba su naujų arba esamų biuro įrenginių
ms.author: danbrown
author: DHB-MSFT
manager: laurawi
ms.date: 08/01/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000660"
- "2509"
ms.openlocfilehash: 3318e1b17cc99e927e1011f7ca9eca8dec616d59
ms.sourcegitcommit: 4600dd4fb577bf5f5482a24616c2d9a6b81e8052
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 08/01/2019
ms.locfileid: "36054238"
---
# <a name="deploying-teams-as-standalone-or-with-new-or-existing-office-installations"></a>Diegti komandos kaip atskirą arba su naujų arba esamų biuro įrenginių

"Microsoft" Teams dabar yra įtraukiama ***naujų įrenginių*** Office 365 ProPlus "," Office 365 Business ir "Office" Mac ". Norėdami gauti daugiau informacijos, žr [Kada bus "Microsoft" Teams pradėti, buvo įtraukta naujų įrenginių Office?](https://docs.microsoft.com/deployoffice/teams-install#when-will-microsoft-teams-start-being-included-with-new-installations-of-office-365-proplus)

Be to, pradedant su versija 1906 m. kas mėnesį kanalas, komandos bus ***pridėta prie esamos*** "Office 365 ProPlus" (ir Office 365 Business) įrenginiuose, kuriuose naudojama "Windows", kai atnaujinate esamą įrenginį į naujausią versiją. Norėdami gauti daugiau informacijos, žr [ką apie esamos Office?](https://docs.microsoft.com/deployoffice/teams-install#what-about-existing-installations-of-office-365-proplus)

> [!NOTE]
> Jei nenorite laukti, kol šis rida tvarkaraštis, jūs galite panaudoti komandos kaip atskirą savo vartotojams vadovaudamiesi [šiomis instrukcijomis](https://docs.microsoft.com/MicrosoftTeams/msi-deployment) arba jūs galite turėti savo vartotojams įdiegti komandos už save nuo [https://teams.microsoft.com/downloads](https://teams.microsoft.com/downloads).

Jei jūsų organizacija nėra pasiruošę diegti komandos, mes turime priemonių galite imtis, siekiant ***pašalinti komandos*** iš [naujų](https://docs.microsoft.com/deployoffice/teams-install#how-to-exclude-microsoft-teams-from-new-installations-of-office-365-proplus) ar [esamų](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-control-the-installation-of-microsoft-teams) įrenginių Office. Jei norite, kad grupės galėtų montuoti, bet ne nori komandos paleisti automatiškai, kad vartotojas po to, kai ji yra įdiegta, pamatyti [Neleisti "Microsoft" komandos paleisti automatiškai po įdiegimo](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-prevent-microsoft-teams-from-starting-automatically-after-installation).

Norėdami ***pašalinti komandas*** įrenginyje, kuriame veikia "Windows", peržiūrėkite [Pašalinti "Microsoft" komandomis](https://support.office.com/article/3b159754-3c26-4952-abe7-57d27f5f4c81). Valymą "Microsoft" Teams kelių paskirties kompiuterius arba vartotojams, peržiūrėkite ["Microsoft" būrių dislokavimą išvalyti](https://docs.microsoft.com/microsoftteams/scripts/powershell-script-teams-deployment-clean-up).

Jei naudojate bendrai naudojamą kompiuterių, nuotolinio darbalaukio tarnybų (RDS) ar virtualų darbalaukį infrastruktūros (VDI), žr. [bendro naudojimo kompiuterių ir VDI aplinkoje, kurioje yra "Microsoft" komandomis](https://docs.microsoft.com/deployoffice/teams-install#shared-computer-and-vdi-environments-with-microsoft-teams).

Jei naudojate Office skirtą "Mac", peržiūrėkite ["Microsoft" komandos įrenginių "Mac"](https://docs.microsoft.com/deployoffice/teams-install#microsoft-teams-installations-on-a-mac).

> [!NOTE]
> Įdiegus komandos, tai [automatiškai atnaujinami](https://docs.microsoft.com/deployoffice/teams-install#feature-and-quality-updates-for-microsoft-teams) maždaug kas dvi savaites su naujomis funkcijomis ir kokybės atnaujinimai. 