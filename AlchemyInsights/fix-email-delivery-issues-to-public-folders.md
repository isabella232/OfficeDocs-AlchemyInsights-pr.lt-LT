---
title: El. pašto pristatymo problemų sprendimas viešuosiuose aplankuose, kuriuose įgalintas paštas
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1956"
- "3500007"
ms.assetid: ''
ms.openlocfilehash: e261fe60843555fa45927b0a6b36e1ccf79fb028
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 04/22/2020
ms.locfileid: "43716360"
---
# <a name="fix-email-delivery-issues-to-mail-enabled-public-folders"></a>El. pašto pristatymo problemų sprendimas viešuosiuose aplankuose, kuriuose įgalintas paštas

Jei išoriniai siuntėjai negali siųsti pranešimų į jūsų pašto viešuosius aplankus, o siuntėjai gauna klaidą: **nepavyko rasti (550 5.4.1),** patikrinkite, ar viešojo aplanko el. pašto domenas sukonfigūruotas kaip vidinis perdavimo domenas, o ne patikimas domenas:

1. Atidarykite ["Exchange" administravimo centrą (EAC).](https://docs.microsoft.com/Exchange/exchange-admin-center)

2. Eikite į **Pašto srautas** \> **Pripažinti domenai**, pasirinkite pripažintą domeną, tada spustelėkite **Redaguoti**.

3. Atsidariusiame ypatybių puslapyje, jei domeno tipas nustatytas kaip **Patikimas**, pakeiskite reikšmę į **Vidinis perdavimas,** tada spustelėkite **Įrašyti**.

Jei išoriniai siuntėjai gauna **klaidą, jūs neturite teisių (550 5.7.13),** vykdykite šią komandą Exchange Online [PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell) norėdami pamatyti anoniminių vartotojų teises viešajame aplanke:

`Get-PublicFolderClientPermission -Identity "<PublicFolderIdentity>" -User Anonymous`Pavyzd3/4iui, `Get-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous`.

Norėdami leisti išoriniams vartotojams siųsti el. laiškus į šį viešąjį aplanką, įtraukite CreateItems prieigą tiesiai vartotojui Anonimas. Pavyzd3/4iui, `Add-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous -AccessRights CreateItems`.
