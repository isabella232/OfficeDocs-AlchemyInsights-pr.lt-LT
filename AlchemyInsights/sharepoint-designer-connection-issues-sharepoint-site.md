---
title: "\"SharePoint Designer\" ryšio problemos"
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f2b1b6b4-10c9-4e83-b9cb-529a0b8a3c55
ms.openlocfilehash: 01ccc6bc28148f397fb6cd2b7a0eaaeb5b51973f
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 06/02/2020
ms.locfileid: "44511552"
---
# <a name="sharepoint-designer-connection-issues"></a>"SharePoint Designer" ryšio problemos 

Jei SharePoint Designer kyla ryšio su SharePoint svetainėmis problemų, išbandykite šiuos bendruosius sprendimus.

1 veiksmas: Patikrinkite, ar SharePoint Designer 2013 yra atnaujintas [su SharePoint Designer 1 pakeitimų paketas](https://support.microsoft.com/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1) ir [2016 m. rugpjūčio 2 naujinimas SharePoint Designer 2013](https://support.microsoft.com/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721).



2 veiksmas: išvalykite vietinės talpyklos failus:

1. Uždarykite SharePoint Designer 2013.

2. Vietiniame kompiuteryje pašalinkite visus failus, rastą kiekviename iš šių aplankų.

    - %APPDATA%\Microsoft\Web serverio plėtiniai\talpykla
    - %APPDATA%\Microsoft\SharePoint Designer\ProxyAssemblyCache %APPDATA%\Microsoft\SharePoint Designer\ProxyAssemblyCache %APPDATA%\Microsoft\SharePoint Designer\ProxyAssemblyCache %APP
    - %USERPROFILE%\AppData\Local\Microsoft\WebsiteCache %USERPROFILE%\AppData\Local\Microsoft\WebsiteCache %USERPROFILE%\AppData\Local\Microsoft\WebsiteCache %USER

3. Atidarykite SharePoint Designer 2013 ir dar kartą įveskite abonementą, kad sužinotumėte, ar jis veikia.

3 veiksmas: [Įgalinkite šiuolaikinės autentifikavimas Office 2013 "Windows" įrenginiuose](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication).

4 veiksmas: Administratoriai turės **leisti pasirinktinį scenarijų** "SharePoint" administravimo centro parametruose, kad "SharePoint Designer" ryšys būtų leidžiamas. Daugiau informacijos rasite [Pasirinktinio scenarijaus leidimas arba draudimas.](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script)


