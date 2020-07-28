---
title: Automatinių "Office Apps" naujinimų valdymas
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/24/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1743"
- "9000140"
ms.openlocfilehash: 5c56c3adcc9a06db43d4df6f367657cb8ff0c8c8
ms.sourcegitcommit: b10cea11b4975354b91193327b58aa4740d34833
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 07/28/2020
ms.locfileid: "45439336"
---
# <a name="control-automatic-updates-for-office-apps"></a>Automatinių "Office Apps" naujinimų valdymas

Pagal numatytuosius nustatymus "Office Apps" naujinimai atsisiunčiami automatiškai ir taikomi fone be jokio vartotojo įsikišimo. Tačiau administratoriai gali valdyti, kaip naujinimai taikomi naudojant "Office Update" parametrus. Naujinimo parametrai leidžia administratoriams įgalinti arba išjungti automatinius naujinimus, rodyti arba slėpti mygtuką **Naujinti dabar** "Office", nustatyti naujinimo terminus ir kt. Išsamesnės informacijos ieškokite:

- ["Office" naujinimo parametrų konfigūravimas](https://docs.microsoft.com/deployoffice/configure-update-settings-for-office-365-proplus)  
- [Automatinis "Office" naujinimas neįgalintas](https://support.microsoft.com/help/2753538/automatic-updating-for-office-2013-and-office-2016-click-to-run-is-not)  
- [Nustatyti, kaip "Office" atnaujinamas jį įdiegus](https://docs.microsoft.com/deployoffice/configuration-options-for-the-office-2016-deployment-tool#updates-element)

Norėdami peržiūrėti esamus naujinimus parametrus, taikomus kliento kompiuteryje, atlikite šiuos veiksmus:

1. Atidarykite registro rengyklę, eikite į **Pradėti**  >  **vykdyti**  >  **regedit**.
2. Pereikite į šią vietą ir peržiūrėkite "Office Update" parametrus:  
    A. HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Office\  
    B. Spustelėkite ĮVykdyti\Konfigūracija

**Pastaba**  Jei OfficeMgmtCOM raktas nustatytas, **"Office Account**Office" naujinimuose gali būti rodomas pranešimas "Naujinimai valdo sistemos  >  **Account**  >  **administratorius".** Jei norite gauti daugiau informacijos, [peržiūrėkite tvarkyti naujinimus į Microsoft 365 apps su Microsoft Endpoint Configuration Manager](https://docs.microsoft.com/deployoffice/manage-updates-to-office-365-proplus-with-system-center-configuration-manager#method-1-use-office-deployment-tool-to-enable-office-365-clients-to-receive-updates-from-configuration-manager).  