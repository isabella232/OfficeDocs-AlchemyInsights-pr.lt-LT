---
title: El. pašto pristatymo problemų sprendimas į pašto viešųjų aplankų
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1956
ms.assetid: ''
ms.openlocfilehash: 45665f900014c52e6a920325b0a3b0f6f79fb72d
ms.sourcegitcommit: d1c1d5bcb52ba9083e8dd7603feb72436c5154c8
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 04/17/2019
ms.locfileid: "31910613"
---
# <a name="fix-email-delivery-issues-to-mail-enabled-public-folders"></a>El. pašto pristatymo problemų sprendimas į pašto viešųjų aplankų

Jei Išoriniams siuntėjams negali siųsti pranešimus į savo pašto viešųjų aplankų ir siuntėjų gauti klaidos pranešimą: **nepavyko rasti (550 5.4.1)**, patikrinkite el. pašto domeno, nes viešasis aplankas yra sukonfigūruotas kaip vidinis perdavimo domenas, o ne su patikimą domeną:

1. Atidaryti [Exchange administravimo centro (EAC)](https://docs.microsoft.com/Exchange/exchange-admin-center).

2. Eikite į **pašto srautą** \> **priimta domenai**, pasirinkite pripažintą domeną, ir tada spustelėkite **Redaguoti**.

3. Ypatybės, atveriamas, jei domeno tipas yra nustatytas kaip **Authoritative**, reikšmę pakeiskite į **vidaus perdavimo** ir tada spustelėkite **įrašyti**.

Jei išorinių siuntėjų gauti klaidos, **jūs neturite teisės (550 5.7.13)**, vykdykite šią komandą į [Exchange Online "PowerShell"](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell) Norėdami matyti, kokias teises anoniminiams vartotojams viešajame aplanke:

`Get-PublicFolderClientPermission -Identity "<PublicFolderIdentity>" -User Anonymous`Pvz., `Get-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous`.

Išorės vartotojai gali siųsti laišką į šį viešąjį aplanką, pridėti CreateItems prieigos teisę į anoniminis vartotojas. Pvz., `Add-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous -AccessRights CreateItems`.
