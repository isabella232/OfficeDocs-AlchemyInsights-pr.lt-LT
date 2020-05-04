---
title: "\"Teams\" diegimas kaip atskiros arba su naujais arba esamais \"Office\" diegimais"
ms.author: danbrown
author: DHB-MSFT
manager: laurawi
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000660"
- "2509"
ms.openlocfilehash: ffa91eaf333792af149feda25f9a377ed591b597
ms.sourcegitcommit: 7e06d9ec1dd462cbd882f088c997d012a032f04d
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 05/04/2020
ms.locfileid: "44010226"
---
# <a name="deploying-teams-as-standalone-or-with-new-or-existing-office-installations"></a>"Teams" diegimas kaip atskiros arba su naujais arba esamais "Office" diegimais

"Microsoft Teams" dabar įtraukta kaip naujų "Microsoft 365 Apps" verslui, "Microsoft 365 Apps" verslui ir "Office for Mac" ***diegimų*** dalis. Daugiau informacijos ieškokite [Kada "Microsoft Teams" pradės būti įtraukta į naujus "Office" diegimus?](https://docs.microsoft.com/deployoffice/teams-install#when-will-microsoft-teams-start-being-included-with-new-installations-of-microsoft-365-apps)

Be to, pradedant 1906 versija mėnesio kanale, komandos bus ***įtrauktos į esamus*** "Microsoft 365 Apps" įmonėms (ir "Microsoft 365 Apps for business") diegimus įrenginiuose, kuriuose veikia "Windows", kai atnaujinsite esamą diegimą į naujausią versiją. Daugiau informacijos rasite [Ką apie esamus "Office" diegimus?](https://docs.microsoft.com/deployoffice/teams-install#what-about-existing-installations-of-microsoft-365-apps)

> [!NOTE]
> Jei nenorite laukti šio diegimo grafiko, galite diegti "Teams" kaip atskirą savo vartotojams [vadovaudamiesi šiomis instrukcijomis](https://docs.microsoft.com/MicrosoftTeams/msi-deployment) arba galite nustatyti, kad vartotojai patys įdiegtų "Teams" patys. [https://teams.microsoft.com/downloads](https://teams.microsoft.com/downloads)

Jei jūsų organizacija nėra pasirengusi diegti "Teams", turime atlikti veiksmus, kuriuos galite atlikti, kad ***"Teams" nebūtų*** įtrauktos į [naujus](https://docs.microsoft.com/deployoffice/teams-install#how-to-exclude-microsoft-teams-from-new-installations-of-microsoft-365-apps) arba [esamus](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-control-the-installation-of-microsoft-teams) "Office" diegimus. Jei norite, kad "Teams" būtų įdiegta, bet nenorite, kad įdiegus "Teams" automatiškai būtų paleista vartotojui, [žr.](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-prevent-microsoft-teams-from-starting-automatically-after-installation)

Norėdami ***pašalinti "Teams"*** iš įrenginio, kuriame veikia "Windows", [žr.](https://support.office.com/article/3b159754-3c26-4952-abe7-57d27f5f4c81) Norėdami išvalyti "Microsoft Teams" iš kelių paskirties mašinų arba vartotojų, [žr.](https://docs.microsoft.com/microsoftteams/scripts/powershell-script-teams-deployment-clean-up)

Jei naudojate bendrai naudojamus kompiuterius, nuotolinio darbalaukio tarnybas (RDS) arba virtualiojo darbalaukio infrastruktūrą (VDI), peržiūrėkite [bendrai naudojamų kompiuterių ir VDI aplinkoje su "Microsoft Teams".](https://docs.microsoft.com/deployoffice/teams-install#shared-computer-and-vdi-environments-with-microsoft-teams)

Jei naudojate "Office for Mac", peržiūrėkite ["Microsoft Teams" diegimus "Mac".](https://docs.microsoft.com/deployoffice/teams-install#microsoft-teams-installations-on-a-mac)

> [!NOTE]
> Įdiegus "Teams", ji [automatiškai atnaujinama](https://docs.microsoft.com/deployoffice/teams-install#feature-and-quality-updates-for-microsoft-teams) maždaug kas dvi savaites su naujomis funkcijomis ir kokybės naujinimais. 