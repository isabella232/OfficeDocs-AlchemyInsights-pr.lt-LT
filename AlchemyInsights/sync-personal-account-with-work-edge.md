---
title: Įgalinkite vartotoją sinchronizuoti asmeninę paskyrą su darbo paskyra Microsoft Edge
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/26/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9127"
- "9004429"
ms.openlocfilehash: da435b37b689e97ca51ce5cf94eb7e7d71eb972060526989239310fac1460628
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: lt-LT
ms.lasthandoff: 08/05/2021
ms.locfileid: "57813400"
---
# <a name="enable-a-user-to-sync-a-personal-account-with-the-work-account-in-microsoft-edge"></a>Įgalinkite vartotoją sinchronizuoti asmeninę paskyrą su darbo paskyra Microsoft Edge

Įsitikinkite, kad atitinkate šiuos kriterijus:

- Enterprise State Roaming is enabled in the "Azure Active Directory" admin center, which requires a subscription to "Azure Active Directory" Premium or Enterprise Mobility + Security (EMS). Daugiau informacijos žr. ["Enterprise State Roaming" įgalinimas "Azure Active Directory"](/azure/active-directory/devices/enterprise-state-roaming-enable).
- Tenkinami vienas arba abu iš šių kriterijų:
    - Jūsų nuomotojui įgalinta "Azure" informacijos apsaugos tarnyba. Daugiau informacijos žr. ["Azure Rights Management" apsaugos aktyvinimas "Microsoft 365" administravimo centras.](/azure/information-protection/activate-office365)
    - ""Azure Active Directory"" tarptinklinio ryšio (ESR) funkcija įgalinta bet kuriam vartotojui arba nuomotojui. Daugiau informacijos žr. [Kas yra įmonės būsenos tarptinklinis ryšys?](/azure/active-directory/devices/enterprise-state-roaming-overview).

Jei abu AIP ir ESR išjungti, klaidos pranešimas informuoja vartotojus, kurie negali sinchronizuoti savo paskyrų.
