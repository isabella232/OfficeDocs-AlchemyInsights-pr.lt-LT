---
title: Įvyko klaida, kai buvo įlaipinimo metu įkeliant kompiuterio analizės prieigos atpažinimo ženklo klaidą
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2536"
- "9000657"
ms.openlocfilehash: 1d6b840e731eaff537d8f74f9ce0af29af13bd390e701fb2835e8718b4521158
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 08/05/2021
ms.locfileid: "53946623"
---
# <a name="there-was-an-error-validating-access-token-error-during-desktop-analytics-onboarding"></a>Klaida "Įvyko klaida bandant nustatyti prieigos atpažinimo ženklą" naudojant kompiuterio "Analytics" parengimą

Ši klaida paprastai stebima pasibaigus autentifikavimo atpažinimo ženklo galiojimui. Paprastai atnaujinant puslapį atnaujinamas atpažinimo ženklas. Tačiau ši problema gali išlikti, jei paskyrai, naudojamai kompiuterio analizės sistemoje, taikomos sąlyginės prieigos strategijos. "Azure" portale galite peržiūrėti "Azure AD" prisijungimo žurnalus, kad pamatytumėte, ar yra prisijungimo prie paskyros, kuri naudojama kompiuterio analizės parengimui, trikčių.

Daugiau informacijos apie sąlyginę prieigą rasite [Sąlyginės prieigos diegimo planas.](https://docs.microsoft.com/azure/active-directory/conditional-access/plan-conditional-access)