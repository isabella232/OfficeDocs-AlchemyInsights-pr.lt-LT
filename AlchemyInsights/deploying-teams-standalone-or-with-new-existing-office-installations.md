---
title: Diegimo Teams kaip atskiras arba naudojant naujas arba esamas Office įdiegtis
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
ms.openlocfilehash: e8baefafc1c2f9583345779c5ae7a9d3d0e05c4b3b7e1b3a74a9a22f7ceed02a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54102210"
---
# <a name="deploying-teams-as-standalone-or-with-new-or-existing-office-installations"></a>Diegimo Teams kaip atskiras arba naudojant naujas arba esamas Office įdiegtis

Microsoft Teams dabar yra įtraukta kaip  naujų ""Microsoft 365" programos įmonėms", ""Microsoft 365" programos verslui" ir "Office for Mac" įrenginių dalis. Daugiau informacijos [žr. Kada Microsoft Teams bus įtraukta į naujas "Office"?](https://docs.microsoft.com/deployoffice/teams-install#when-will-microsoft-teams-start-being-included-with-new-installations-of-microsoft-365-apps)

Be to, pradedant nuo 1906 versijos dabartiniame kanale , "Teams" bus įtraukta į esamas ""Microsoft 365" programos įmonėms" (ir ""Microsoft 365" programos verslui") įdiegtis įrenginiuose, kuriuose veikia "Windows", kai ***atnaujinsite*** esamą įdiegtį į naujausią versiją. Daugiau informacijos [žr. Ką apie esamas "Office"?](https://docs.microsoft.com/deployoffice/teams-install#what-about-existing-installations-of-microsoft-365-apps)

> [!NOTE]
> Jei nenorite laukti šio diegimo tvarkaraščio, galite įdiegti "Teams" kaip atskirą vartotojams, [](https://docs.microsoft.com/MicrosoftTeams/msi-deployment) vykdykite šias instrukcijas arba galite nustatyti, kad jūsų vartotojai įdiegtų "Teams" patys [https://teams.microsoft.com/downloads](https://teams.microsoft.com/downloads) iš .

Jei jūsų organizacija nėra pasirengusi diegti "Teams", turime veiksmus, kurių ***galite imtis, kad "Teams"*** nebūtų įtraukti į naujas arba esamas "Office" įdiegtis. [](https://docs.microsoft.com/deployoffice/teams-install#how-to-exclude-microsoft-teams-from-new-installations-of-microsoft-365-apps) [](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-control-the-installation-of-microsoft-teams) Jei norite Teams, bet nenorite, kad įdiegus Teams vartotojas būtų paleidžiamas automatiškai, žr. Apsauga [nuo Microsoft Teams](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-prevent-microsoft-teams-from-starting-automatically-after-installation)nuo paleidimo automatiškai įdiegus .

Norėdami ***pašalinti Teams*** iš įrenginio, kuriame veikia Windows, [žr. Microsoft Teams .](https://support.office.com/article/3b159754-3c26-4952-abe7-57d27f5f4c81) Norėdami išvalyti Microsoft Teams iš kelių tikslinių įrenginių arba vartotojų, [žr. Microsoft Teams diegimo valymo .](https://docs.microsoft.com/microsoftteams/scripts/powershell-script-teams-deployment-clean-up)

Jei naudojate bendrinamus kompiuterius, nuotolinio darbalaukio tarnybas (RDS) arba virtualiojo darbalaukio infrastruktūrą (VDI), žr. Bendrai naudojamos kompiuterio ir VDI aplinkos [su "Microsoft Teams".](https://docs.microsoft.com/deployoffice/teams-install#shared-computer-and-vdi-environments-with-microsoft-teams)

Jei naudojate "Office Mac", [žr. Microsoft Teams "Mac" įdiegtys.](https://docs.microsoft.com/deployoffice/teams-install#microsoft-teams-installations-on-a-mac)

> [!NOTE]
> Įdiegus Teams, ji automatiškai atnaujinama maždaug [kas](https://docs.microsoft.com/deployoffice/teams-install#feature-and-quality-updates-for-microsoft-teams) dvi savaites naujomis funkcijomis ir kokybės naujinimais. 