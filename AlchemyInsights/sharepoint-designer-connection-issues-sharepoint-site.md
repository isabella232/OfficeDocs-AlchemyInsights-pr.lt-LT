---
title: SharePoint Dizaino įrankio ryšio problemos
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
ms.openlocfilehash: d55f7c1902bb623900fa74bdae70695b6e04ad84ce7b6ea314db614283ec436d
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 08/05/2021
ms.locfileid: "53942033"
---
# <a name="sharepoint-designer-connection-issues"></a>SharePoint Dizaino įrankio ryšio problemos 

Jei SharePoint dizaino įrankis susiduria su ryšio su SharePoint problemomis, išbandykite šiuos bendruosius sprendimus.

1 veiksmas: patikrinkite, ar "SharePoint Designer 2013" atnaujinama [naudojant "SharePoint Designer Service Pack 1"](https://support.microsoft.com/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1) ir [2016 m. rugpjūčio 2 d. "SharePoint Designer 2013" naujinimą.](https://support.microsoft.com/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721)



2 veiksmas: išvalykite vietinės talpyklos failus:

1. Uždarykite SharePoint Designer 2013".

2. Vietiniame kompiuteryje pašalinkite visus failus, esančius kiekviename iš šių aplankų.

    - %APPDATA%\Microsoft\Web Server Extensions\Cache
    - %APPDATA%\Microsoft\SharePoint Designer\ProxyAssemblyCache
    - %USERPROFILE%\AppData\Local\Microsoft\WebsiteCache

3. Atidarykite SharePoint Designer 2013" ir dar kartą įveskite paskyrą, kad pamatytumėte, ar ji veikia.

3 veiksmas: [2013 m. Office autentifikavimo įgalinkite Windows įrenginiuose.](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication)

4 veiksmas: Administratoriai turės leisti pasirinktinį **scenarijų** "SharePoint" administravimo centro parametruose, kad SharePoint dizaino įrankio ryšį. Daugiau [informacijos žr. Pasirinktinio scenarijaus leidimas arba užkirstas](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script) kelias jam.


