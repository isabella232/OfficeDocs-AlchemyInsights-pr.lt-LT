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
ms.openlocfilehash: e1f8227047daede71d0fa3b3557db0d95a379b99b76ab0c2fe1d6ed8cc213d4a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54079458"
---
# <a name="encryption-with-transport-rules"></a>Šifravimas naudojant transportavimo taisykles

[„Exchange“ administravimo centre](https://go.microsoft.com/fwlink/p/?linkid=834822) (EAC) galite naudoti „Office“ pranešimų šifravimo (OME) galimybes savo pašto srauto taisyklėse, kad paleistumėte laiškų šifravimą. Pasirinkite transportavimo taisyklės sąlygos parinktį **Taikyti „Office 365“ pranešimų šifravimą ir teisių apsaugą**.

- Norėdami gauti daugiau informacijos, žr. [Šifravimui skirtos pašto srauto taisyklės apibrėžimas](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email).

- „Powershell“ naudokite „cmdlet“ [New-TransportRule](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email?view=o365-worldwide#use-exchange-online-powershell-to-create-a-mail-flow-rule-for-encrypting-email-messages-without-the-new-ome-capabilities) ir nustatykite parametrą *ApplyOME* kaip $true.
