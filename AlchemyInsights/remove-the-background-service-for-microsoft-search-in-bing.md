---
title: "\"Microsoft\" ieškos fone paslaugos šalinimas \"Bing\""
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/12/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9214"
- "9005302"
ms.openlocfilehash: 6447137fca9b2d48508f4e240a438c7f851c103c
ms.sourcegitcommit: 3fb39a080cc8680d960b8468ac9355389a3e2df4
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 03/12/2021
ms.locfileid: "50816204"
---
# <a name="remove-the-background-service-for-microsoft-search-in-bing"></a>"Microsoft" ieškos fone paslaugos šalinimas "Bing"

Norėdami pašalinti "Microsoft Search" fono paslaugą "Bing", galite išbandyti šias priemones:

1. Norėdami atkurti pradinius ieškos modulio parametrus, atlikite šiuos veiksmus:

    a. Perjunkite jungiklį **naudoti "Bing" kaip numatytąjį ieškos [](https://docs.microsoft.com/deployoffice/microsoft-search-bing#change-whether-bing-is-the-default-search-engine-for-google-chrome) modulį**.

    b. [Eikite į "Microsoft" 365 administravimo centrą](https://docs.microsoft.com/deployoffice/microsoft-search-bing#configure-the-setting-in-the-microsoft-365-admin-center-to-allow-the-extension-to-be-installed) ir išvalykite parametrą, kuris paveikia visus jūsų organizacijos vartotojus.

2. Kad pašalintumėte fono paslaugą iš atskiro įrenginio, atlikite šias užduotis:

    a. Pasirinkite **valdymo skydas > programos > programos ir funkcijos**.

    b. Dešiniuoju pelės mygtuku spustelėkite **"Microsoft" ieška "Bing** " įdiegtų programų sąraše, tada spustelėkite **pašalinti**.

3. Kad pašalintumėte fono paslaugą iš kelių organizacijos įrenginių, registruokitės kaip administratorius ir vykdykite šią komandą dalyje scenarijus: 

`"%ProgramFiles(x86)%\Microsoft\DefaultPackMSI\MainBootStrap.exe" uninstallAll`
