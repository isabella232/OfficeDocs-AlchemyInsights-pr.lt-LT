---
title: Grupės kūrimas
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
- "9003234"
- "7230"
ms.openlocfilehash: b8cb3f1de991bfe7197607d5e8964a018e31c122
ms.sourcegitcommit: 35e2c122d8a838d98d1f0851c29b16282261580f
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 11/17/2020
ms.locfileid: "49088908"
---
# <a name="create-a-group"></a>Grupės kūrimas

Šioje temoje aprašomi grupės kūrimas.

**Grupės kūrimo teisė**

Įsitikinkite, kad turite teisę kurti naują grupę. Visuotinis administratorius gali išjungti grupės kūrimą "Azure" portale arba "Access" skyde. Jums gali reikėti administratoriaus, kad galėtumėte sukurti jums naują grupę arba suteikti reikiamas teises.

**Grupių kūrimo teisių valdymas**

1. Visuotiniai administratoriai gali valdyti grupių kūrimo teises (dėl su sauga susijusių priežasčių) arba "Office" 365 grupes, sukurtas "Azure" portale arba "Access" srityje, pasirinkdami "vartotojai gali kurti saugos grupes" Azure "portaluose", arba "vartotojai gali kurti" Office 365 "grupes" Azure "portaluose" parinktys " **visose grupėse**  >  **(parametrai)**.
2. Taip pat galite apriboti grupės kūrimą, kad pasirinktumėte grupę vartotojų, jei turite "Azure Active Directory P1 Premium" licenciją.

**Pasveikinimo pranešimo išjungimas naujiems "Office 365" grupės nariams**

Į "Office 365" grupes įtraukti vartotojai gali būti išjungti, kai "PowerShell" nustato " **Unifiedgroupsveikiemessageenabled** ". Sužinokite apie šį parametrą [čia](https://docs.microsoft.com/powershell/module/exchange/set-unifiedgroup?view=exchange-ps&preserve-view=true).

