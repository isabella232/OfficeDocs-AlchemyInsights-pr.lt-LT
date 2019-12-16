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
ms.openlocfilehash: 9730bd66afd494385db3de605f5fe68d0f274ed3
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 12/15/2019
ms.locfileid: "40051721"
---
# <a name="sharepoint-designer-connection-issues"></a>"SharePoint Designer" ryšio problemos 

Jei SharePoint Designer susiduria su "SharePoint" svetainių ryšio problemomis, išbandykite toliau nurodytus bendruosius sprendimus.

1 veiksmas: patikrinkite, ar SharePoint Designer 2013 yra atnaujinama naudojant [SharePoint Designer Service Pack 1](https://support.microsoft.com/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1) ir [rugpjūčio 2, 2016 naujinimas SharePoint Designer 2013](https://support.microsoft.com/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721).



2 veiksmas: išvalykite vietos talpyklos failus:

1. Uždarykite SharePoint Designer 2013.

2. Vietiniame kompiuteryje, pašalinkite visus failus, rasti kiekviename iš šių aplankų.

    - %APPDATA%\Microsoft\Web serverio Extensions\Cache
    - %APPDATA%\Microsoft\SharePoint Designer\ProxyAssemblyCache
    - %USERPROFILE%\AppData\Local\Microsoft\WebsiteCache

3. Atidarykite "SharePoint Designer 2013" ir dar kartą įveskite paskyrą, kad sužinotumėte, ar ji veikia.

3 veiksmas: [įgalinkite šiuolaikinės autentifikavimo Office 2013 "Windows" įrenginiuose](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication?redirectSourcePath=/article/Enable-Modern-Authentication-for-Office-2013-on-Windows-devices-7dc1c01a-090f-4971-9677-f1b192d6c910&view=o365-worldwide).

4 veiksmas: administratoriai turės **leisti pasirinktinį scenarijų** SharePoint administravimo centro parametruose leisti SharePoint Designer ryšį. Norėdami gauti daugiau informacijos, žiūrėkite [leisti arba neleisti pasirinktinio scenarijaus](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script) .


