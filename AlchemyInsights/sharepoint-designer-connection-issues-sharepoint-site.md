---
title: SharePoint Online teisių lygiai
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f2b1b6b4-10c9-4e83-b9cb-529a0b8a3c55
ms.openlocfilehash: 356fef8e02f2c1fd9d209c68194685bb0acaa367
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 06/07/2019
ms.locfileid: "34760700"
---
# <a name="sharepoint-designer-connection-issues"></a>SharePoint Designer ryšio problemas 

Jei SharePoint Designer patiria ryšio problemas prie SharePoint svetainės, prašome pabandyti šiuos bendrus sprendimus.

1 veiksmas: Patikrinkite, ar atnaujinta SharePoint Designer.

- [SharePoint Designer 2013](https://www.microsoft.com/download/details.aspx?id=35491)

- [SharePoint Designer pakeitimų paketas 1 (SP1)](https://support.microsoft.com/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1)

- [Naujinimas SharePoint Designer 2013 (KB3114721)](https://support.microsoft.com/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721)

2 veiksmas: Išvalykite vietinės talpyklos failus

- Uždarykite SharePoint Designer 2013.

- Vietiniame kompiuteryje, eikite į šiuos aplankus, kuriuos norite pašalinti talpyklos failus.

- Spustelėkite pradėti, paleisti ir panaikinti visus failus rasti kiekvieno į žemiau vietose.

%AppData%\Microsoft\Web server Extensions\Cache %APPDATA%\Microsoft\SharePoint Designer\ProxyAssemblyCache %USERPROFILE%\AppData\Local\Microsoft\WebsiteCache

Atidarykite SharePoint Designer 2013 ir įvesti sąskaitą, dar kartą Norėdami pamatyti, jei ji veikia.

3 veiksmas: [įgalinti šiuolaikinės autentifikavimas Office 2013 m. "Windows" įrenginiuose](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication?redirectSourcePath=/article/Enable-Modern-Authentication-for-Office-2013-on-Windows-devices-7dc1c01a-090f-4971-9677-f1b192d6c910&view=o365-worldwide)

4 žingsnis: Administratoriams reikės leisti Custom scenarijų leisti SharePoint Designer ryšį.

Išsamius veiksmus, pavyzdžiai ir svarstymus žr [leisti arba neleisti pasirinktinį scenarijų](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).


