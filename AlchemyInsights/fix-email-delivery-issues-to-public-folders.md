---
title: Pašto pristatymo problemų sprendimas pašto viešuosiuose aplankuose
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
ms.assetid: ''
ms.openlocfilehash: da35ae4bd911fb75f23cc1c99aacbaa2392425dd
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47677936"
---
# <a name="fix-email-delivery-issues-to-mail-enabled-public-folders"></a>Pašto pristatymo problemų sprendimas pašto viešuosiuose aplankuose

Jei išoriniai siuntėjai negali siųsti laiškų į jūsų pašto viešąjį aplanką, o siuntėjams pateikiama klaida: **nepavyko rasti (550 5.4.1)**, patikrinkite, ar viešojo aplanko el. pašto domenas sukonfigūruotas kaip vidinis perdavimo domenas, o ne kaip patikimas domenas:

1. Atidarykite " [Exchange" administravimo centrą (EAC)](https://docs.microsoft.com/Exchange/exchange-admin-center).

2. Eikite į **pašto srauto** \> **pripa ̨inti domenai**, pasirinkite pripažintą domeną, tada spustelėkite **Redaguoti**.

3. Atsidariusiame ypatybių puslapyje, jei domeno tipas nustatytas kaip **patikimas**, pakeiskite reikšmę į **Vidinė relė** ir spustelėkite **įrašyti**.

Jei išoriniai siuntėjai gauna klaidą, neturite **teisių (550 5.7.13)**, " [Exchange Online](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell) " "PowerShell" vykdykite šią komandą, kad pamatytumėte anoniminių vartotojų teises viešajame aplanke:

`Get-PublicFolderClientPermission -Identity "<PublicFolderIdentity>" -User Anonymous` Pvz., `Get-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous` .

Norėdami leisti išoriniams vartotojams siųsti laiškus į šį viešąjį aplanką, įtraukite "CreateItems" prieigą prie vartotojo anoniminių. Pvz., `Add-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous -AccessRights CreateItems` .
