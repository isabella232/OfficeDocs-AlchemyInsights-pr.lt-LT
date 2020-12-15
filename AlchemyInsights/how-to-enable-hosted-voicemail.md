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
ms.openlocfilehash: 26eb22054d246a6ca5a2491c68a5d9e4ed90d45b
ms.sourcegitcommit: 523098560e54a50184a99c974809dfbfffadacb5
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 12/09/2020
ms.locfileid: "49677996"
---
# <a name="how-to-enable-hosted-voicemail"></a>Kaip įgalinti nuomojamų išteklių balso paštą

Norėdami įjungti balso paštą, **Hostedbalso paštas** turi būti nustatytas į $True.

Ypatybės **Hostedbalso paštas** , esanti vartotojui naudojant nuotolinį "PowerShell" (RPS).

Daugiau informacijos apie prisijungimą prie RPS rasite straipsnyje ["Microsoft teams PowerShell" apžvalga](https://docs.microsoft.com/microsoftteams/teams-powershell-overview) , kur rasite daugiau informacijos apie prisijungimą prie RPS.

1. Komandos administratorius turi būti prisijungęs prie "Remote PowerShell" komandoms.
1. "PowerShell" paraginti komandų administratorius gali paleisti " **Set-CsUser" User@contoso.com-Hostedbalso pašto $True** , kur yra atitinkamo vartotojo SIP URI.

> [!NOTE]
> Strategijų keitimas gali užtrukti iki 24 valandų.