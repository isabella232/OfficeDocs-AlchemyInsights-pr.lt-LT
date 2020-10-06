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
ms.openlocfilehash: 74a26306766ed7952a3bbbcb06f1f0113a113024
ms.sourcegitcommit: 9fd002ce49ad9a7e58c3eb997a8063e2e1feab55
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 10/06/2020
ms.locfileid: "48366472"
---
# <a name="fix-email-delivery-issues-to-mail-enabled-public-folders"></a>Pašto pristatymo problemų sprendimas pašto viešuosiuose aplankuose

Jei išoriniai siuntėjai negali siųsti laiškų į jūsų pašto viešąjį aplanką, o siuntėjams pateikiama klaida: **nepavyko rasti (550 5.4.1)**, patikrinkite, ar viešojo aplanko el. pašto domenas sukonfigūruotas kaip vidinis perdavimo domenas, o ne kaip patikimas domenas:

1. Atidarykite " [Exchange" administravimo centrą (EAC)](https://docs.microsoft.com/Exchange/exchange-admin-center).

2. Eikite į **pašto srauto** \> **pripa ̨inti domenai**, pasirinkite pripažintą domeną, tada spustelėkite **Redaguoti**.

3. Atsidariusiame ypatybių puslapyje, jei domeno tipas nustatytas kaip **patikimas**, pakeiskite reikšmę į **Vidinė relė** ir spustelėkite **įrašyti**.

Jei išoriniai siuntėjai gauna klaidą, neturite **teisių (550 5.7.13)**, " [Exchange Online](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell) " "PowerShell" vykdykite šią komandą, kad pamatytumėte anoniminių vartotojų teises viešajame aplanke:

`Get-PublicFolderClientPermission -Identity "<PublicFolderIdentity>" -User Anonymous` Pvz., `Get-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous` .

Norėdami leisti išoriniams vartotojams siųsti laiškus į šį viešąjį aplanką, įtraukite "CreateItems" prieigą prie vartotojo anoniminių. Pvz., `Add-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous -AccessRights CreateItems` .
