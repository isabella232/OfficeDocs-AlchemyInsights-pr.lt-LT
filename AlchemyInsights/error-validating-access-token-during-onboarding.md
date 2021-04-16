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
ms.openlocfilehash: 12e5906ba8cbc76ba1fd99dde1cf76396c3a6942
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 04/15/2021
ms.locfileid: "51813696"
---
# <a name="there-was-an-error-validating-access-token-error-during-desktop-analytics-onboarding"></a>Klaida "Įvyko klaida bandant nustatyti prieigos atpažinimo ženklą" naudojant kompiuterio "Analytics" parengimą

Ši klaida paprastai stebima pasibaigus autentifikavimo atpažinimo ženklo galiojimui. Paprastai atnaujinant puslapį atnaujinamas atpažinimo ženklas. Tačiau ši problema gali išlikti, jei paskyrai, naudojamai kompiuterio analizės sistemoje, taikomos sąlyginės prieigos strategijos. "Azure" portale galite peržiūrėti "Azure AD" prisijungimo žurnalus, kad pamatytumėte, ar yra prisijungimo prie paskyros, kuri naudojama kompiuterio analizės parengimui, trikčių.

Daugiau informacijos apie sąlyginę prieigą rasite [Sąlyginės prieigos diegimo planas.](https://docs.microsoft.com/azure/active-directory/conditional-access/plan-conditional-access)