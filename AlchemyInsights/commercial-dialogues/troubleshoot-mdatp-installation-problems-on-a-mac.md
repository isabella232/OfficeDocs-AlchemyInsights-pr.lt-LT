---
title: MDATP diegimo problemų šalinimas "Mac" kompiuteryje
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
ms.openlocfilehash: 4b03361666f950a2010e4c4d8e78d156438d9e90
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 03/11/2021
ms.locfileid: "50749775"
---
# <a name="troubleshoot-mdatp-installation-problems-on-a-mac"></a>MDATP diegimo problemų šalinimas "Mac" kompiuteryje

Nepavykus įdiegti neautomatiškai, diegimo vediklio **suvestinės** puslapyje rodomas šis klaidos pranešimas:

"Diegiant įvyko klaida. Diegimo programa aptiko klaidą, dėl kurios nepavyko įdiegti. Kreipkitės pagalbos į programinės įrangos gamintoją. "

Naudojant MDM įdiegtį, puslapyje rodomas bendrasis diegimo gedimas.

Nors mes negalime Rodyti tikslių klaidų galutiniams vartotojams, mes saugome žurnalo failą su diegimo eiga, aplanke **/Library/Logs/Microsoft/mdatp/install.log**. Kiekvienas diegimo seansas prideda prie šio žurnalų failo. Norėdami išvesti tik paskutinį diegimo seansą, naudokite `sed` .

Jei norite sužinoti daugiau, peržiūrėkite ["Microsoft Defender ATP for Mac" diegimo problemų diagnostiką](https://go.microsoft.com/fwlink/?linkid=2144615).
