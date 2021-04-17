---
title: Grupės kūrimas
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003234"
- "7230"
ms.openlocfilehash: ec74b7c098d302d3bdeb5a412fad41efe7b82b98
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 04/15/2021
ms.locfileid: "51816364"
---
# <a name="create-a-group"></a>Grupės kūrimas

Šioje temoje aprašomas grupės kūrimas.

**Teisė kurti grupę**

Įsitikinkite, kad turite teisę kurti naują grupę. Visuotiniai administratoriai gali išjungti grupės kūrimą "Azure" portale arba "Access" skyde. Jums gali tekti administratoriaus sukurti naują grupę arba suteikti jums atitinkamas teises.

**Grupės kūrimo teisių valdymas**

1. Visuotiniai administratoriai gali valdyti grupės kūrimo teises (dėl su sauga susijusių priežasčių) arba "Office 365" grupes, sukurtas "Azure" portale arba "Access" skyde, pasirinkdami "Vartotojai gali kurti saugos grupes "Azure" portaluose" arba "Vartotojai gali kurti "Office 365" grupes "Azure" portaluose" parinktys dalyje **Visos grupės**  >  **Bendra (Parametrai)**.
2. Taip pat galite apriboti grupės kūrimą, kad pasirinktumėte vartotojų grupę, jei turite "Azure Active Directory P1 Premium" licenciją.

**Naujų "Office 365" grupės narių pasveikinimo pranešimo išjungimas**

Pasveikinimo pranešimą, išsiųstą vartotojams, įtrauktiems į "Office 365" grupes, galima išjungti "PowerShell" nustačius **UnifiedGroupWelcomeMessageEnabled** kaip False. Sužinokite apie šį parametrą [čia](https://docs.microsoft.com/powershell/module/exchange/set-unifiedgroup?view=exchange-ps&preserve-view=true).

