---
title: GPO diegimas
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/24/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004400"
- "8602"
ms.openlocfilehash: d31f77e70e8456a4076a8146025f1f8ada977a06
ms.sourcegitcommit: 969219d6dff18d86d679d4d8741d1e39e4ce9539
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 03/03/2021
ms.locfileid: "50427566"
---
# <a name="gpo-deployment"></a>GPO diegimas

Vartotojo ir kompiuterio objektų "Azure Active Directory" domenų tarnybos ("Azure AD DS") parametrai dažnai valdomi naudojant grupės strategijos objektus (GPO). "Azure AD DS" yra įtaisytosios GPOs, skirtos "AADDC" vartotojams ir "AADDC" kompiuterių konteineriams. Galite tinkinti šiuos įtaisytuosius GPO, kad sukonfigūruotumėte grupės strategiją, kaip reikia jūsų aplinkai. "Azure AD DC" administratorių grupės nariai turi grupės strategijos administravimo teises "Azure AD DS" domene ir taip pat gali kurti pasirinktinio GPOs ir organizacijos vienetus (OUs). Daugiau informacijos apie grupės strategiją ir jos veikimą rasite [grupės strategijos apžvalga](https://docs.microsoft.com/previous-versions/windows/it-pro/windows-server-2012-R2-and-2012/hh831791(v=ws.11)).

Hibridinėje aplinkoje grupės strategijos sukonfigūruotos vietinėje AD DS aplinkoje nesinchronizuojamos su "Azure AD DS". Norėdami apibrėžti "Azure AD DS" vartotojų arba kompiuterių konfigūracijos parametrus, redaguokite vieną iš numatytųjų GPO arba sukurkite pasirinktinę GPO.

Šiame straipsnyje [valdoma grupės strategija](https://docs.microsoft.com/azure/active-directory-domain-services/manage-group-policy) rodoma, kaip įdiegti grupės strategijos valdymo įrankius, kaip ton redaguoti įtaisytuosius GPO ir kurti pasirinktinio GPOs.
