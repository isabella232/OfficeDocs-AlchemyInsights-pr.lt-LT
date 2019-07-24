---
title: SharePoint Designer ryšio problemas
ms.author: efrene
author: efrene
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f2b1b6b4-10c9-4e83-b9cb-529a0b8a3c55
ms.openlocfilehash: 1d3f6ad3128292a9dbcc46cc7da23af59a63fbb4
ms.sourcegitcommit: a285c609319ade038461e090e14a701830031825
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 07/24/2019
ms.locfileid: "35840559"
---
# <a name="sharepoint-designer-connection-issues"></a>SharePoint Designer ryšio problemas 

Jei SharePoint Designer patiria ryšio problemas prie SharePoint svetainės, pabandykite šiuos bendrosios sprendimus.

1 veiksmas: Patikrinkite, ar kad SharePoint Designer 2013 m. atnaujinti [SharePoint Designer Service Pack 1](https://support.microsoft.com/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1) ir [2 rugpjūtis 2016 atnaujinti SharePoint Designer 2013](https://support.microsoft.com/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721).



2 veiksmas: Išvalykite vietinės talpyklos failus:

1. Uždarykite SharePoint Designer 2013.

2. Vietiniame kompiuteryje, pašalinkite visus failus, randami kiekviename iš šių aplankų.

    - %AppData%\Microsoft\Web serveris Extensions\Cache
    - %AppData%\Microsoft\SharePoint Designer\ProxyAssemblyCache
    - %USERPROFILE%\AppData\Local\Microsoft\WebsiteCache

3. Atidarykite SharePoint Designer 2013 ir įvesti sąskaitą, dar kartą Norėdami pamatyti, jei ji veikia.

3 veiksmas: [įgalinti šiuolaikinės autentifikavimas Office 2013 m. "Windows" įrenginiuose](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication?redirectSourcePath=/article/Enable-Modern-Authentication-for-Office-2013-on-Windows-devices-7dc1c01a-090f-4971-9677-f1b192d6c910&view=o365-worldwide).

4 žingsnis: Administratoriams reikės **Leisti Custom scenarijų** SharePoint administravimo centro parametrai leisti SharePoint Designer ryšį. Žr [leisti arba neleisti pasirinktinį scenarijų](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script) daugiau informacijos.


