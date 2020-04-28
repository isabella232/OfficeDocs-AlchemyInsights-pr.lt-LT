---
title: Šifravimas naudojant transportavimo taisykles
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002635"
- "5154"
ms.openlocfilehash: 3f16c7e7be99a50cd57f47ea2801b3022c4aec95
ms.sourcegitcommit: 07725fcaf073f0ac145f98653b989afdb34c5ad0
ms.translationtype: HT
ms.contentlocale: lt-LT
ms.lasthandoff: 04/28/2020
ms.locfileid: "43915172"
---
# <a name="encryption-with-transport-rules"></a>Šifravimas naudojant transportavimo taisykles

[„Exchange“ administravimo centre](https://go.microsoft.com/fwlink/p/?linkid=834822) (EAC) galite naudoti „Office“ pranešimų šifravimo (OME) galimybes savo pašto srauto taisyklėse, kad paleistumėte laiškų šifravimą. Pasirinkite transportavimo taisyklės sąlygos parinktį **Taikyti „Office 365“ pranešimų šifravimą ir teisių apsaugą**.

- Norėdami gauti daugiau informacijos, žr. [Šifravimui skirtos pašto srauto taisyklės apibrėžimas](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email).

- „Powershell“ naudokite „cmdlet“ [New-TransportRule](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email?view=o365-worldwide#use-exchange-online-powershell-to-create-a-mail-flow-rule-for-encrypting-email-messages-without-the-new-ome-capabilities) ir nustatykite parametrą *ApplyOME* kaip $true.
