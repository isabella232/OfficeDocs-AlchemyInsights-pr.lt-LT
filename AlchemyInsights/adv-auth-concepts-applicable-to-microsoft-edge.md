---
title: Išplėstinės autentifikavimo sąvokos, taikomos "Microsoft Edge"
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/03/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "9003931"
- "6986"
- "8329"
- "9004625"
ms.openlocfilehash: d469973c4f8605b00d32f6f625eb5fdd17e8f390
ms.sourcegitcommit: 6bfe9cd9d0b18481e0cac6f1f5bc86ed7df31037
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 03/27/2021
ms.locfileid: "51398593"
---
# <a name="advanced-authentication-concepts-applicable-to-microsoft-edge"></a>Išplėstinės autentifikavimo sąvokos, taikomos "Microsoft Edge"

Toliau nurodytos išplėstinės autentifikavimo sąvokos, taikomos "Microsoft Edge":

**Aktyvus autentifikavimas**

Kai įgalinsite ["ProactiveAuthEnabled"](https://go.microsoft.com/fwlink/?linkid=2134621) strategiją, "Microsoft Edge" bandys aktyviai autentifikuoti prisijungusius vartotojus per "Microsoft" tarnybas. Reguliariais intervalais ji naudos internetinę tarnybą, kad patikrins, ar yra atnaujinta deklaracija, kurioje yra konfigūracija, reglamentuojanti aktyvią autentifikavimą.

Pranašumai: aktyvus autentifikavimas įgalina autentifikavimą pagrindinėse tarnybose, pvz., "Office" naujo skirtuko puslapyje. Be to, jei "Bing" naudojama kaip ieškos modulis, aktyvus autentifikavimas pagerina adreso juostos našumą ir padeda generuoti ieškos rezultatus, pritaikytus jūsų verslo poreikiams.

**"Windows Hello CredUI", skirta "NTLM" autentifikavimui**

Jei bendroji autentifikacija (SSO) negalima, kai žiniatinklio svetainė bando prisijungti prie vartotojo naudodama NTLM arba "Negotiate" mechanizmą, ši funkcija leis vartotojui bendrinti OS kredencialus su svetaine ir patenkinti autentifikavimo iššūkius naudojant "Windows Hello Cred" vartotojo sąsają. Šis prisijungimo srautas bus rodomas tik "Windows 10" ir tik vartotojams, kurie negaus SSO NTLM arba "Negotiate" iššūkio metu.

**Įrašytų slaptažodžių naudojimas norint prisijungti automatiškai**

Vartotojai, įrašę slaptažodžius "Microsoft Edge", gali įgalinti automatinį prisijungimą prie svetainių, kuriose įrašė kredencialus. Vartotojai gali įjungti arba išjungti šią funkciją "edge://settings/passwords ir galite konfigūruoti ją slaptažodžių [tvarkytuvo strategijose.](https://go.microsoft.com/fwlink/?linkid=2134622)
