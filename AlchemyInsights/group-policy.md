---
title: Grupės strategija
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8303"
- "9003234"
ms.openlocfilehash: a829a78bbe947300b6dabb9fdb36088c17809742
ms.sourcegitcommit: 6900c2b7208ca51a9873dfc2e00be6f66cb25e3c
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 02/15/2021
ms.locfileid: "50256781"
---
# <a name="group-policy"></a>Grupės strategija

Vartotojo ir kompiuterio objektų "Azure Active Directory" domenų tarnybos ("Azure AD DS") parametrai dažnai valdomi naudojant grupės strategijos objektus (GPO). "Azure AD DS" yra įtaisytosios GPOs, skirtos "AADDC" vartotojams ir "AADDC" kompiuterių konteineriams. Galite tinkinti šiuos įtaisytuosius GPO, kad sukonfigūruotumėte grupės strategiją, kaip reikia jūsų aplinkai. "Azure AD DC" administratorių grupės nariai turi grupės strategijos administravimo teises "Azure AD DS" domene ir taip pat gali kurti pasirinktinio GPOs ir organizacijos vienetus (OUs). Daugiau informacijos apie grupės strategiją ir jos veikimą rasite [grupės strategijos apžvalga](https://docs.microsoft.com/previous-versions/windows/it-pro/windows-server-2012-R2-and-2012/hh831791(v=ws.11)).

Hibridinėje aplinkoje grupės strategijos sukonfigūruotos vietinėje AD DS aplinkoje nesinchronizuojamos su "Azure AD DS". Norėdami apibrėžti "Azure AD DS" vartotojų arba kompiuterių konfigūracijos parametrus, redaguokite vieną iš numatytųjų GPO arba sukurkite pasirinktinę GPO.

Šiame straipsnyje [valdoma grupės strategija](https://docs.microsoft.com/azure/active-directory-domain-services/manage-group-policy) rodoma, kaip įdiegti grupės strategijos valdymo įrankius, kaip ton redaguoti įtaisytuosius GPO ir kurti pasirinktinio GPOs.



