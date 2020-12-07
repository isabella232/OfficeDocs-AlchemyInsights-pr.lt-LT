---
title: "\"Microsoft Edge\" palaikymas, skirtas \"Microsoft Defender\" taikomosios programos apsaugai"
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/05/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004024"
- "7090"
ms.openlocfilehash: 65cbc867ea7d1c73ca2906f51f72aa3376f31b5d
ms.sourcegitcommit: 2e4a5153e530bf15744a52e982eeb0d99757e9d2
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 12/04/2020
ms.locfileid: "49584017"
---
# <a name="microsoft-edges-support-for-microsoft-defender-application-guard"></a>"Microsoft Edge" palaikymas, skirtas "Microsoft Defender" taikomosios programos apsaugai

Skirtas "Windows 10" ir "Microsoft Edge", taikomosios programos apsauga naudoja aparatūros izoliacijos metodą, leidžiantį vartotojui naršyti nepatikimą svetainę iš izoliuoto, "Hyper-V"-įgalinto konteinerio, atskirto nuo pagrindinio kompiuterio operacinės sistemos.

Įmonės administratorius apibrėžia patikimų svetainių, debesies išteklių ir vidinių tinklų sąrašą. Kai vartotojas apsilanko svetainėje, kurios nėra sąraše, "Microsoft Edge" atidarys vietą konteineryje. Tai reiškia, kad jei svetainė tampa kenkėjiška, pagrindinis kompiuteris liks apsaugotas, o užpuolikas negalės gauti įmonės duomenų.

Konteinerio plėtinių diegimas palaikomas kaip "Microsoft Edge" 81 versija ir jį galima valdyti naudojant strategiją. UpdateURL adresas, kuris bus naudojamas ExtensionInstallForcelist strategijoje, turi būti įtrauktas kaip neutralus šaltinis tinklo izoliacijos strategijose, kurias naudoja taikomosios programos sargyba.

Daugiau informacijos ieškokite " [Microsoft Edge" palaikymas, skirtas "Microsoft Defender" taikomosios programos apsaugai](https://go.microsoft.com/fwlink/?linkid=2134229).
