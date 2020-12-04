---
title: Išplėstinės autentifikavimo koncepcijos, taikomos "Microsoft Edge"
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
ms.openlocfilehash: 241d594fac6664dd1e85fd60e30a6344c432555e
ms.sourcegitcommit: c069f1b53567ad14711c423740f120439a312a60
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 12/04/2020
ms.locfileid: "49573524"
---
# <a name="advanced-authentication-concepts-applicable-to-microsoft-edge"></a>Išplėstinės autentifikavimo koncepcijos, taikomos "Microsoft Edge"

Toliau pateiktos išplėstinės autentifikavimo koncepcijos, kurios taikomos "Microsoft Edge":

**Iniciatyvi autentifikacija**

Kai įgalinate strategiją [Proactiveauthenabled](https://go.microsoft.com/fwlink/?linkid=2134621) , "Microsoft Edge" bandys aktyviai autentifikuoti prisijungusiems vartotojams per "Microsoft" tarnybas. Reguliariais intervalais ji naudos internetinę paslaugą, kad tikrintų, ar yra atnaujinta deklaracija, kurioje yra aktyvi konfigūracija.

Pranašumai: aktyvus autentifikavimas įgalina autentifikavimo pagrindines tarnybas, pvz., "Office" naujo skirtuko puslapį. Be to, jei kaip ieškos modulį naudojamas "Bing", aktyvusis autentifikavimas pagerina adreso juostos veikimą ir padeda sukurti suasmenintus ieškos rezultatus pagal jūsų įmonės poreikius.

**"Windows Hello" Creipt NTLM autentifikavimui**

Jei Bendroji autentifikacija (SSO) neprieinama, kai žiniatinklio svetainė bando prisijungti vartotojui per NTLM arba Negotiate mechanizmą, ši funkcija leis vartotojui bendrinti OS kredencialus su svetaine ir patenkinti autentifikavimo iššūkį naudojant "Windows Hello" CRED UI. Šis prisijungimo srautas bus rodomas tik sistemoje "Windows 10" ir tik tiems vartotojams, kurie negauna SSO per NTLM arba Negotiate iššūkį.

**Naudokite įrašytus slaptažodžius, kad prisijungtumėte automatiškai**

Vartotojai, kurie įrašo slaptažodžius "Microsoft Edge", gali įgalinti automatinį prisiregistravimo žiniatinklio svetaines, kuriose yra įrašytų kredencialų. Vartotojai gali įjungti arba išjungti šią funkciją "edge://settings/passwords", o jūs galite ją sukonfigūruoti [slaptažodžių tvarkytuvo](https://go.microsoft.com/fwlink/?linkid=2134622) politikoje.
