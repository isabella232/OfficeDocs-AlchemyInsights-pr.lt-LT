---
title: Kaip įgalinti nuomojamų išteklių balso paštą
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/09/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002347"
- "7563"
ms.openlocfilehash: 4d70e92a7c1bf8f3cc62d4a310aa140ee2dfdef4c798ae17faa961736d9db500
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54055562"
---
# <a name="how-to-enable-hosted-voicemail"></a>Kaip įgalinti nuomojamų išteklių balso paštą

Norint įgalinti balso paštą, **"HostedVoicemail"** turi būti $true.

Ypatybė **HostedVoicemail** vartotojui, naudojanti nuotolinę "PowerShell" (RPS).

Daugiau informacijos apie prisijungimą prie RPS [žr. Microsoft Teams "PowerShell" apžvalga,](https://docs.microsoft.com/microsoftteams/teams-powershell-overview) jei reikia daugiau informacijos apie prisijungimą prie RPS.

1. "Teams administratorius turi būti prisijungęs prie nuotolinės "PowerShell", kad Teams.
1. Iš "PowerShell" raginimo Teams administratorius gali paleisti **set-csuser user@contoso.com -HostedVoiceMail $true,** kur sip uri priklauso tam vartotojui.

> [!NOTE]
> Strategijų pakeitimai gali užtrukti iki 24 valandų, kad būtų galima pakartoti.