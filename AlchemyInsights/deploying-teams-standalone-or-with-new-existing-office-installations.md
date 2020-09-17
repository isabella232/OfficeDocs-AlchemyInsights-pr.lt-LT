---
title: "\"Teams\" diegimas kaip atskira arba naudojant naujas arba esamas \"Office\" įdiegtis"
ms.author: danbrown
author: DHB-MSFT
manager: laurawi
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000660"
- "2509"
ms.openlocfilehash: c3ca4365abc41509ccf602c5b9046655706840fc
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 09/15/2020
ms.locfileid: "47806767"
---
# <a name="deploying-teams-as-standalone-or-with-new-or-existing-office-installations"></a>"Teams" diegimas kaip atskira arba naudojant naujas arba esamas "Office" įdiegtis

"Microsoft teams" dabar įtraukta kaip "Microsoft 365" programų, skirtų įmonėms, "Microsoft 365" verslui ir "Office for Mac", ***naujų įrenginių*** dalis. Daugiau informacijos ieškokite [Kada "Microsoft teams" pradės būti įtrauktas į naujus "Office" diegimus?](https://docs.microsoft.com/deployoffice/teams-install#when-will-microsoft-teams-start-being-included-with-new-installations-of-microsoft-365-apps)

Be to, pradedant "1906" versija dabartiniame kanale, "teams" bus ***įtrauktos į esamus*** "Microsoft 365" taikomųjų programų "Enterprise" (ir "Microsoft 365" verslui) diegimus įrenginiuose, kuriuose veikia "Windows", kai naujinate esamą įdiegtį į naujausią versiją. Daugiau informacijos rasite peržiūrėję skyrių [apie esamus "Office" diegimus?](https://docs.microsoft.com/deployoffice/teams-install#what-about-existing-installations-of-microsoft-365-apps)

> [!NOTE]
> Jei nenorite laukti šio rida grafiko, galite diegti komandas kaip atskirą savo vartotojams [vykdydami šias instrukcijas](https://docs.microsoft.com/MicrosoftTeams/msi-deployment)   arba galite nustatyti, kad vartotojai patys įdiegtų komandas  [https://teams.microsoft.com/downloads](https://teams.microsoft.com/downloads) .

Jei jūsų organizacija nėra pasirengusi įdiegti "teams", mes turime veiksmus, kurių galite imtis norėdami ***neįtraukti komandų*** į [naują](https://docs.microsoft.com/deployoffice/teams-install#how-to-exclude-microsoft-teams-from-new-installations-of-microsoft-365-apps) arba [esamą](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-control-the-installation-of-microsoft-teams) "Office" diegimą. Jei norite, kad "Office" būtų diegiamos, tačiau nenorite, kad "teams" automatiškai pradėtų naudoti vartotojui įdiegus, peržiūrėkite ["Microsoft teams" nepaleisti automatiškai po įdiegimo](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-prevent-microsoft-teams-from-starting-automatically-after-installation).

Norėdami ***pašalinti komandas*** iš įrenginio, kuriame veikia "Windows", peržiūrėkite ["Microsoft teams" šalinimas](https://support.office.com/article/3b159754-3c26-4952-abe7-57d27f5f4c81). Norėdami išvalyti "Microsoft teams" iš kelių tikslinių įrenginių arba vartotojų, peržiūrėkite ["Microsoft teams" diegimo išvalymas](https://docs.microsoft.com/microsoftteams/scripts/powershell-script-teams-deployment-clean-up).

Jei naudojate bendrinamus kompiuterius, nuotolinio darbalaukio tarnybas (RDS) arba virtualiąją kompiuterio infrastruktūrą (VDI), peržiūrėkite [bendrai naudojamą kompiuterį ir VDI aplinką su "Microsoft teams"](https://docs.microsoft.com/deployoffice/teams-install#shared-computer-and-vdi-environments-with-microsoft-teams).

Jei naudojate "Office for Mac", "Mac" kompiuteryje Peržiūrėkite ["Microsoft teams" diegimus](https://docs.microsoft.com/deployoffice/teams-install#microsoft-teams-installations-on-a-mac).

> [!NOTE]
> Įdiegus komandas, ji [automatiškai atnaujinama](https://docs.microsoft.com/deployoffice/teams-install#feature-and-quality-updates-for-microsoft-teams) kas dvi savaites su naujomis funkcijomis ir kokybės naujinimais. 