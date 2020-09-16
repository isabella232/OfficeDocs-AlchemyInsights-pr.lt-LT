---
title: "\"SharePoint Designer\" prisijungimo problemos"
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f2b1b6b4-10c9-4e83-b9cb-529a0b8a3c55
ms.openlocfilehash: 997ba3de58485d4fe6d24b926c33348378af8cd3
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47727179"
---
# <a name="sharepoint-designer-connection-issues"></a>"SharePoint Designer" prisijungimo problemos 

Jei "SharePoint Designer" susiduria su "SharePoint" svetainių prisijungimo problemomis, išbandykite šiuos bendruosius sprendimus.

1 veiksmas: patikrinkite, ar "SharePoint Designer 2013" atnaujinama naudojant " [SharePoint Designer" 1 pakeitimų paketą](https://support.microsoft.com/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1) ir [rugpjūčio 2 d., 2016 naujinimą, skirtą "SharePoint Designer 2013"](https://support.microsoft.com/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721).



2 veiksmas: išvalykite vietos talpyklos failus:

1. Uždarykite "SharePoint Designer" 2013.

2. Vietiniame kompiuteryje pašalinkite visus failus, esančius kiekviename iš šių aplankų.

    - %AppData%\microsoft\žiniatinklio serverio Extensions\Cache
    - %APPDATA%\Microsoft\SharePoint "Windows" proxyassemblycache
    - %USERPROFILE%\AppData\Local\Microsoft\WebsiteCache

3. Atidarykite "SharePoint Designer" 2013 ir dar kartą Įeikite į paskyrą, kad sužinotumėte, ar ji veikia.

3 veiksmas: [modernaus autentifikavimo įgalinimas "Office 2013" "Windows" įrenginiuose](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication).

4 veiksmas: administratoriams reikės **leisti pasirinktiniam scenarijui** "SharePoint" administravimo centro parametruose leisti "SharePoint Designer" ryšiui. Daugiau informacijos ieškokite [pasirinktinio scenarijaus leidimas arba neleidimas](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script) .


