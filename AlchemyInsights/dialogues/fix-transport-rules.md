---
title: Taisykite transportavimo taisykles
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: 635009ed4b78d2b05b0eef1f3298765b10f86ede
ms.sourcegitcommit: bd6a9cb5d357baee5134c0dea430afc2a035c810
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 03/09/2021
ms.locfileid: "50695868"
---
# <a name="fix-transport-rules"></a>Taisykite transportavimo taisykles

Pasirinktinio pašto srauto taisyklė turi įtakos šiam pranešimui. Norėdami peržiūrėti tikslią taisyklę, atlikite šiuos veiksmus:

1. Pateikimo rezultatuose, dalyje **papildoma informacija**, pasižymėkite **GUID** arba **strategijos pavadinimą**.
2. "Exchange Management Shell" Paleistis. Daugiau informacijos ieškokite " [Exchange" valdymo aplinkos atidarymas](https://go.microsoft.com/fwlink/?linkid=2101432).
3. Vykdykite šią komandą (naudodami savo pateiktyje esantį GUID):  **get-TransportRule-tapatybė "GUID" | FL * aprašas***
4. Peržiūrėkite aprašą ir peržiūrėkite sukonfigūruotas sąlygas, kurios paveikė laišką.

Norėdami sužinoti daugiau, peržiūrėkite [get-TransportRule](https://go.microsoft.com/fwlink/?linkid=2101523).
