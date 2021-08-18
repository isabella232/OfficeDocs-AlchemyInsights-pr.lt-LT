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
ms.openlocfilehash: 4042e042554f78febff2073fde6f14db72a6d4e0
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 08/13/2021
ms.locfileid: "58318656"
---
# <a name="how-to-enable-hosted-voicemail"></a>Kaip įgalinti nuomojamų išteklių balso paštą

Norint įgalinti balso paštą, **"HostedVoicemail"** turi būti nustatytas kaip $true.

Ypatybė **HostedVoicemail** vartotojui, naudojanti nuotolinę "PowerShell" (RPS).

Daugiau informacijos apie prisijungimą prie RPS [žr. Microsoft Teams "PowerShell" apžvalga,](https://docs.microsoft.com/microsoftteams/teams-powershell-overview) jei reikia daugiau informacijos apie prisijungimą prie RPS.

1. "Teams administratorius turi būti prisijungęs prie nuotolinės "PowerShell", kad Teams.
1. Iš "PowerShell" raginimo Teams administratorius gali paleisti **set-csuser user@contoso.com -HostedVoiceMail $true,** kur sip uri priklauso tam vartotojui.

**Pastaba:** strategijų pakeitimai gali užtrukti iki 24 valandų, kad būtų galima pakartoti.