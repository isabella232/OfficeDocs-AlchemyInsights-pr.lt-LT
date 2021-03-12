---
title: Problemos diegiant "Microsoft Defender" "Mac" arba "Linux"
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/16/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6028"
- "9001222"
ms.openlocfilehash: a8d5ad2246b9b83e1e0a4d5be4dd8bb41c16e734
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 09/14/2020
ms.locfileid: "50713839"
---
# <a name="issues-installing-microsoft-defender-on-mac-or-linux"></a>Problemos diegiant "Microsoft Defender" "Mac" arba "Linux"

**Mac**

- Įsitikinkite, kad prieš diegiant "Microsoft Defender ATP for Mac" laikomasi sistemos reikalavimų. Daugiau informacijos rasite [kaip įdiegti "Microsoft Defender ATP for Mac](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-atp-mac#how-to-install-microsoft-defender-atp-for-mac)".  
- Peržiūrėkite failo informaciją: "/Library/Logs/Microsoft/mdatp/install.log".

**Linux**

- Įsitikinkite, kad prieš diegiant "Microsoft Defender ATP for Linux" laikomasi sistemos reikalavimų. Daugiau informacijos rasite [kaip įdiegti "Microsoft Defender ATP for Linux"](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-atp-linux#system-requirements). 
- Norėdami patikrinti, ar veikia MDATP tarnyba, žiūrėkite [diegimas nepavyko](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-support-install#installation-failed).  
    Jei norite pašalinti triktis ir išspręsti problemas, jei tarnyba nepaleista, peržiūrėkite [veiksmus, skirtus triktims šalinti, jei nevykdoma mdatp tarnyba](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-support-install#steps-to-troubleshoot-if-mdatp-service-isnt-running).
- Norėdami patikrinti kliento konfigūraciją, kuri patikrina produkto sveikatą ir atlikti "EICAR" teksto failo aptikimo testą, žr.: [kliento konfigūracija](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-install-manually#client-configuration).  

    **Pastaba** "Access" veiklos palaikomų failų sistemų sąrašą rasite ["Microsoft Defender ATP for Linux](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-atp-linux#system-requirements)".