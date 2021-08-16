---
title: Transportavimo taisyklių taisymas
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
ms.openlocfilehash: d89283dec427ba3d4f55fc1f180efc13da16ae15c3d5a6c0c06a696faa6df7f8
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54034762"
---
# <a name="fix-transport-rules"></a>Transportavimo taisyklių taisymas

Pasirinktinio pašto srauto taisyklė paveikė šį pranešimą. Norėdami peržiūrėti tikslią taisyklę, atlikite šiuos veiksmus:

1. Pateikimo rezultatų dalyje Papildoma informacija **atkreipkite** dėmesį į **GUID** arba **strategijos pavadinimą**.
2. Paleiskite Exchange valdymo aplinką. Daugiau informacijos žr. [Valdymo aplinkos Exchange atidarymas.](https://go.microsoft.com/fwlink/?linkid=2101432)
3. Vykdykite šią komandą (naudodami GUID iš savo pateikimo):  **Get-TransportRule -identity "GUID" | fl * Description***
4. Peržiūrėkite aprašą, kad pamatytumėte sukonfigūruotas sąlygas, kurios paveikė pranešimą.

Norėdami sužinoti daugiau, žr. [Get-TransportRule](https://go.microsoft.com/fwlink/?linkid=2101523).
