---
title: "\"Office\" diegimo komandų pašalinimas arba pašalinimas"
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2662"
- "9000660"
ms.openlocfilehash: 22d69db749671afdfe7a809d1bc598e2ad1891d8
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47658229"
---
# <a name="uninstall-or-exclude-teams-from-new-or-existing-office-installations"></a><span data-ttu-id="0891b-102">Pašalinkite arba išskirkite komandas iš naujų arba esamų "Office" įdiegčių</span><span class="sxs-lookup"><span data-stu-id="0891b-102">Uninstall or exclude Teams from new or existing Office installations</span></span>

<span data-ttu-id="0891b-103">"Microsoft teams" yra įtraukta kaip "Microsoft 365" taikomųjų programų, skirtų įmonėms, "Microsoft 365" verslui ir "Office for Mac", dalis.</span><span class="sxs-lookup"><span data-stu-id="0891b-103">Microsoft Teams is included as part of Microsoft 365 Apps for enterprise, Microsoft 365 Apps for business, and Office for Mac.</span></span>

- <span data-ttu-id="0891b-104">Naudokite " [Office" diegimo įrankį](https://docs.microsoft.com/deployoffice/teams-install#how-to-exclude-microsoft-teams-from-new-installations-of-microsoft-365-apps) , jei norite neįtraukti komandų į naujus "Office" diegimus.</span><span class="sxs-lookup"><span data-stu-id="0891b-104">Use the [Office Deployment Tool](https://docs.microsoft.com/deployoffice/teams-install#how-to-exclude-microsoft-teams-from-new-installations-of-microsoft-365-apps) to exclude Teams from new installations of Office.</span></span>
- <span data-ttu-id="0891b-105">Norėdami *pašalinti* komandas iš įrenginio, kuriame veikia "Windows", peržiūrėkite ["Microsoft teams" šalinimas](https://support.office.com/article/3b159754-3c26-4952-abe7-57d27f5f4c81).</span><span class="sxs-lookup"><span data-stu-id="0891b-105">To *uninstall* Teams from a device running Windows, see [Uninstall Microsoft Teams](https://support.office.com/article/3b159754-3c26-4952-abe7-57d27f5f4c81).</span></span> <span data-ttu-id="0891b-106">Norėdami išvalyti "Microsoft teams" iš kelių tikslinių įrenginių arba vartotojų, peržiūrėkite ["Microsoft teams" diegimo valymą](https://docs.microsoft.com/microsoftteams/scripts/powershell-script-teams-deployment-clean-up).</span><span class="sxs-lookup"><span data-stu-id="0891b-106">To clean up Microsoft Teams from multiple target machines or users, see [Microsoft Teams deployment clean up](https://docs.microsoft.com/microsoftteams/scripts/powershell-script-teams-deployment-clean-up).</span></span>
- <span data-ttu-id="0891b-107">Naudokite parinktį [profilaktinė Teamasinstall](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-control-the-installation-of-microsoft-teams
) , kad "Microsoft teams" nebūtų galima įdiegti automatiškai naudojant "Office".</span><span class="sxs-lookup"><span data-stu-id="0891b-107">Use the [PreventTeamsInstall](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-control-the-installation-of-microsoft-teams
) option to prevent Microsoft Teams from installing automatically with Office.</span></span>
- <span data-ttu-id="0891b-108">Naudokite parinktį " [Profilakfirstlaunchafterinstall](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-prevent-microsoft-teams-from-starting-automatically-after-installation) " prieš diegdami "teams", kad "Microsoft" komandos nebūtų *paleidžiamos*automatiškai po įdiegimo.</span><span class="sxs-lookup"><span data-stu-id="0891b-108">Use the [PreventFirstLaunchAfterInstall](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-prevent-microsoft-teams-from-starting-automatically-after-installation) option, *before Teams is installed*, to prevent Microsoft Teams from starting automatically after installation.</span></span>

<span data-ttu-id="0891b-109">Jei naudojate "Office for Mac", "Mac" kompiuteryje Peržiūrėkite ["Microsoft teams" diegimus](https://docs.microsoft.com/deployoffice/teams-install#microsoft-teams-installations-on-a-mac).</span><span class="sxs-lookup"><span data-stu-id="0891b-109">If you're using Office for Mac, see [Microsoft Teams installations on a Mac](https://docs.microsoft.com/deployoffice/teams-install#microsoft-teams-installations-on-a-mac).</span></span>