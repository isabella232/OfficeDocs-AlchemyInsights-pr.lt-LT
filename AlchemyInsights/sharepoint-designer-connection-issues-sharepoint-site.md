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
ms.openlocfilehash: 7451cfe957545537298f57feb5b47bd6d43cddbf
ms.sourcegitcommit: 6d341637dbb14e90726a1ce1d68f077ace9bb765
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 06/04/2019
ms.locfileid: "34716899"
---
# <a name="sharepoint-designer-connection-issues"></a>SharePoint Designer ryšio problemas 

<p>Jei SharePoint Designer patiria ryšio problemas prie SharePoint svetainės, prašome pabandyti šiuos bendrus sprendimus.</p> <p><strong>1-as žingsnis:</strong> <strong>Patikrinti SharePoint Designer atnaujinama&nbsp; </strong></p> <ul> <li><a href="https://www.microsoft.com/en-us/download/details.aspx?id=35491">SharePoint Designer 2013</a></li> <li><a href="https://support.microsoft.com/en-us/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1">SharePoint Designer pakeitimų paketas 1 (SP1)</a></li> <li><a href="https://support.microsoft.com/en-us/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721">Naujinimas SharePoint Designer 2013 (KB3114721)</a></li> </ul> <p><strong>2-as žingsnis:</strong> <strong>Išvalykite vietinės talpyklos failus</strong>&nbsp;</p> <ol> <li style="font-weight: 400;">Uždarykite SharePoint Designer 2013.&nbsp;</li> <li style="font-weight: 400;">Vietiniame kompiuteryje, eikite į šiuos aplankus, kuriuos norite pašalinti talpyklos failus.&nbsp;</li> <li style="font-weight: 400;">Spustelėkite <strong>Start -&gt; paleisti</strong> ir panaikinkite visus failus, rasta pagal kiekvieną į žemiau vietose.&nbsp;<br /><br />%AppData%\Microsoft\Web serveris Extensions\Cache<br />%AppData%\Microsoft\SharePoint Designer\ProxyAssemblyCache<br />%USERPROFILE%\AppData\Local\Microsoft\WebsiteCache</li> <li style="font-weight: 400;">Atidarykite SharePoint Designer 2013 ir įvesti sąskaitą, dar kartą Norėdami pamatyti, jei ji veikia.</li> </ol> <p><strong>3 veiksmas:</strong> <a href="https://docs.microsoft.com/en-us/office365/admin/security-and-compliance/enable-modern-authentication?redirectSourcePath=%252fen-us%252farticle%252fEnable-Modern-Authentication-for-Office-2013-on-Windows-devices-7dc1c01a-090f-4971-9677-f1b192d6c910&amp;view=o365-worldwide">, <strong>Kad šiuolaikinės autentifikavimas Office 2013 m. "Windows" įrenginiuose</strong></a>&nbsp;</p> <p><strong>4 žingsnis:</strong> <strong>Administratoriai turi leisti Custom scenarijus leidžia SharePoint Designer ryšį</strong>.</p> <p>Išsamius veiksmus, pavyzdžiai ir svarstymus žr <a href="https://docs.microsoft.com/en-us/sharepoint/allow-or-prevent-custom-script">leisti arba neleisti pasirinktinį scenarijų</a>.&nbsp;</p>


