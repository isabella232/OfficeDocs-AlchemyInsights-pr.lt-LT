---
title: MDATP diegimo trikčių šalinimas "Mac" kompiuteryje
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
ms.openlocfilehash: 4139f47f40a89069521aaa1a3e4fdab56e9e27a2096ae0ad099be827f60d51fc
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54091056"
---
# <a name="troubleshoot-mdatp-installation-problems-on-a-mac"></a>MDATP diegimo trikčių šalinimas "Mac" kompiuteryje

Jei nepavyksta įdiegti rankiniu būdu, **diegimo** vediklio puslapyje Suvestinė rodoma ši klaida:

"Diegimo metu įvyko klaida. Diegimo programa aptiko klaidą, dėl kurios nepavyko įdiegti. Pagalbos kreipkitės į programinės įrangos gamintoją."

Naudojant MDM diegimus, puslapyje taip pat rodoma bendroji diegimo klaida.

Nors galutiniams vartotojams nerodome tikslių klaidų, mes laikome žurnalo failą su diegimo eiga, **naudojant /Library/Logs/Microsoft/mdatp/install.log**. Kiekvienas diegimo seansas pridedamas prie šio žurnalo failo. Norėdami išvesti tik paskutinį diegimo seansą, naudokite `sed` .

Norėdami sužinoti daugiau, žr. ["Microsoft" sargybos ATP, skirta "Mac", diegimo trikčių šalinimas.](https://go.microsoft.com/fwlink/?linkid=2144615)
