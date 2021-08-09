---
title: Išplėstinės autentifikavimo sąvokos, taikomos Microsoft Edge
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
ms.openlocfilehash: 8ddec37260ec4e3bcc390dcc8adb7397368de19555ee31be458be033d3886386
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 08/05/2021
ms.locfileid: "53934373"
---
# <a name="advanced-authentication-concepts-applicable-to-microsoft-edge"></a>Išplėstinės autentifikavimo sąvokos, taikomos Microsoft Edge

Toliau nurodytos išplėstinės autentifikavimo sąvokos, taikomos Microsoft Edge:

**Aktyvus autentifikavimas**

Kai įgalinsite [strategiją ProactiveAuthEnabled,](https://go.microsoft.com/fwlink/?linkid=2134621) Microsoft Edge bandys aktyviai autentifikuoti prisijungusius vartotojus naudodami "Microsoft" paslaugos. Reguliariais intervalais ji naudos internetinę tarnybą, kad patikrins, ar yra atnaujinta deklaracija, kurioje yra konfigūracija, reglamentuojanti aktyvią autentifikavimą.

Pranašumai: aktyvus autentifikavimas įgalina autentifikavimą į pagrindines tarnybas, pvz., Office naujo skirtuko puslapį. Be to, Bing naudojamas kaip ieškos modulis, aktyvusis autentifikavimas pagerina adreso juostos našumą ir padeda generuoti ieškos rezultatus, pritaikytus jūsų įmonės poreikiams.

**Windows Hello "CredUI" NTLM autentifikavimui**

Jei bendroji autentifikacija (SSO) negalima, kai žiniatinklio svetainė bando prisijungti prie vartotojo naudodama NTLM arba negotiate mechanizmą, ši funkcija leis vartotojui bendrinti OS kredencialus su svetaine ir patenkinti autentifikavimo iššūkius naudojant "Windows Hello Cred" vartotojo sąsają. Šis prisijungimo srautas bus rodomas tik "Windows 10" ir tik tiems vartotojams, kurie NTLM arba "Negotiate" iššūkio metu negaus SSO.

**Įrašytų slaptažodžių naudojimas norint prisijungti automatiškai**

Vartotojai, įrašę slaptažodžius "Microsoft Edge" gali įgalinti automatinį prisijungimą prie svetainių, kuriose įrašė kredencialus. Vartotojai gali įjungti arba išjungti šią funkciją "edge://settings/passwords ir galite konfigūruoti ją slaptažodžių [tvarkytuvo strategijose.](https://go.microsoft.com/fwlink/?linkid=2134622)
