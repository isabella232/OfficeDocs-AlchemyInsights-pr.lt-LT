---
title: Šifravimas naudojant transportavimo taisykles
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002635"
- "5154"
ms.openlocfilehash: dfd77bc83b4b278e3630858f54fdfb109ade2a14
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: lt-LT
ms.lasthandoff: 04/15/2021
ms.locfileid: "51813876"
---
# <a name="encryption-with-transport-rules"></a>Šifravimas naudojant transportavimo taisykles

[„Exchange“ administravimo centre](https://go.microsoft.com/fwlink/p/?linkid=834822) (EAC) galite naudoti „Office“ pranešimų šifravimo (OME) galimybes savo pašto srauto taisyklėse, kad paleistumėte laiškų šifravimą. Pasirinkite transportavimo taisyklės sąlygos parinktį **Taikyti „Office 365“ pranešimų šifravimą ir teisių apsaugą**.

- Norėdami gauti daugiau informacijos, žr. [Šifravimui skirtos pašto srauto taisyklės apibrėžimas](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email).

- „Powershell“ naudokite „cmdlet“ [New-TransportRule](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email?view=o365-worldwide#use-exchange-online-powershell-to-create-a-mail-flow-rule-for-encrypting-email-messages-without-the-new-ome-capabilities) ir nustatykite parametrą *ApplyOME* kaip $true.
