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
ms.openlocfilehash: 6f9e164713ce36023de954d45031fd4414780e174bf5c7741c4aec274a65b32e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54067848"
---
# <a name="gpo-deployment"></a>GPO diegimas

Parametrai vartotojų ir kompiuterių objektų "Azure Active Directory" domenų tarnybos ("Azure AD DS") dažnai valdomos naudojant grupės strategijos objektus (GPO). "Azure AD DS" yra įtaisytųjų GPO AADDC vartotojams ir AADDC kompiuterių konteineriams. Galite tinkinti šias įtaisytas GPO, kad sukonfigūruotų grupės strategiją, kiek reikia jūsų aplinkai. "Azure AD DC" administratorių grupės nariai turi grupės strategijos administravimo teises "Azure AD DS" domene ir taip pat gali kurti pasirinktinius GPO ir organizacijos vienetus (OUs). Daugiau informacijos apie tai, kas yra grupės strategija ir kaip ji veikia, žr. [Grupės strategijos apžvalga](https://docs.microsoft.com/previous-versions/windows/it-pro/windows-server-2012-R2-and-2012/hh831791(v=ws.11)).

Hibridinės aplinkos grupės strategijos, sukonfigūruotos vietinėje AD DS aplinkoje, nėra sinchronizuojamos su "Azure AD DS". Norėdami apibrėžti vartotojų arba kompiuterių konfigūracijos parametrus "Azure AD DS", redaguokite vieną iš numatytųjų GPO arba sukurkite pasirinktinį GPO.

Šiame straipsnyje [Grupės strategijos valdymas](https://docs.microsoft.com/azure/active-directory-domain-services/manage-group-policy) rodoma, kaip įdiegti grupės strategijos valdymo įrankius, kaip redaguoti įtaisytąsias GPO ir kaip kurti pasirinktinius GPO.
