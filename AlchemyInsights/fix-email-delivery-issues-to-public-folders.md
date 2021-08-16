---
title: El. pašto pristatymo problemų šalinimas viešuosiuose aplankuose su įgalintais laiškais
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1956"
- "3500007"
ms.openlocfilehash: ff1400f694ae037a8658356af068b4c20b8fa9d9908dafedb90db7bb6859530f
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54068820"
---
# <a name="fix-email-delivery-issues-to-mail-enabled-public-folders"></a>El. pašto pristatymo problemų šalinimas viešuosiuose aplankuose su įgalintais laiškais

Jei išoriniai siuntėjai negali siųsti laiškų į viešuosius aplankus, kuriuose įgalintas paštas, o siuntėjai gauna klaidą: nepavyko **rasti (550 5.4.1),** patikrinkite, ar viešojo aplanko el. pašto domenas sukonfigūruotas kaip "vidinio perdavimo domenas", o ne patikimas domenas:

1. Atidarykite [Exchange centrą (EAC)](https://docs.microsoft.com/Exchange/exchange-admin-center).

2. Eikite **į Pašto srautas** Pripažinti \> **domenai**, pasirinkite pripažintą domeną, tada spustelėkite **Redaguoti**.

3. Atidaromame puslapyje Ypatybės, jei domeno tipas nustatytas kaip **Patikimas,** pakeiskite reikšmę į **Vidinis** perdavimas, tada spustelėkite **Įrašyti**.

Jei išoriniai siuntėjai gauna klaidą, kurios neturite **teisių (550 5.7.13),** vykdykite šią komandą ["Exchange Online PowerShell",](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell) kad pamatytumėte anoniminių vartotojų teises viešajame aplanke:

`Get-PublicFolderClientPermission -Identity "<PublicFolderIdentity>" -User Anonymous` Pvz., `Get-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous` .

Norėdami leisti išoriniams vartotojams siųsti el. laiškus į šį viešąjį aplanką, įtraukite "CreateItems" prieigą prie vartotojo anoniminio. Pvz., `Add-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous -AccessRights CreateItems` .
