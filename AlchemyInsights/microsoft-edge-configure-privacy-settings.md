---
title: Microsoft Edge konfigūruoti privatumo parametrus
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003843"
- "6892"
ms.openlocfilehash: 24721325aefd4a8c0dbeb7864ce6da637c4df932694d4b6fff80cab5bb5b4319
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54114180"
---
# <a name="microsoft-edge-configure-privacy-settings"></a>Microsoft Edge konfigūruoti privatumo parametrus

Pagal numatytuosius parametrus, Microsoft Edge įdiegta ne "Windows platformose, diagnostikos duomenys ir svetainės informacija nesiunčiami "Microsoft". Tačiau, Microsoft Edge įdiegta "Windows 10", diagnostikos duomenys ir svetainės informacija siunčiami pagal [vartotojų diagnostikos Windows parametrus.](https://docs.microsoft.com/windows/privacy/configure-windows-diagnostic-data-in-your-organization)

Norėdami konfigūruoti, Microsoft Edge tvarko jūsų organizacijos duomenų rinkimą, naudokite šias grupės strategijas:
- [MetricsReportingEnabled](https://docs.microsoft.com/DeployEdge/microsoft-edge-policies#metricsreportingenabled): Ši strategija leidžia pranešti apie naudojimą ir su gedimu susijusius duomenis.
- [SendSiteInfoToImproveServices](https://docs.microsoft.com/DeployEdge/microsoft-edge-policies#sendsiteinfotoimproveservices): Ši strategija siunčia svetainės informaciją, kuri naudojama "Microsoft" paslaugos.

Norėdami sužinoti daugiau, [žr. Strategijos parametrų konfigūravimas](https://docs.microsoft.com/deployedge/microsoft-edge-enterprise-privacy-settings#configure-policy-settings).