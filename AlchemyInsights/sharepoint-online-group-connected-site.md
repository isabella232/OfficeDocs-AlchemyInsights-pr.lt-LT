---
title: Grupės įtraukimas į "SharePoint" svetainę
ms.author: pebaum
author: Techwriter40
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f7d730bf-0d6e-424c-970c-6137c71cb50b
ms.openlocfilehash: 423db4e5bbb85e75aee3548d5b6b46a64ebc6fa0
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 10/18/2019
ms.locfileid: "36750528"
---
# <a name="issues-when-creating-or-group-connected-sites-in-sharepoint-online"></a>Problemos kuriant arba grupės prijungtas svetaines SharePoint Online

Yra keletas bendrų problemų, su kuriomis susiduriama kuriant arba iš naujo kuriant grupę prijungtą svetainę.

 Jei ištrynėte grupę ir jos prijungtą svetainę ir norite sukurti kitą svetainę naudodami tą patį URL, turėsite visam laikui pašalinti ankstesnę svetainę.

Atsisiųsti [SPO Management Shell](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)

 Daugiau informacijos apie tai, kaip pradėti su "PowerShell", rasite [darbo su "SharePoint Online Management Shell" Pradžia](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps)

Pašalinti svetainę iš panaikintų svetainių naudojant [pašalinti SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) "PowerShell" cmdlet.

Jei kuriate grupę prijungtą svetainę ir gaunate įspėjimą kita grupė su tuo pačiu pseudonimu jau yra, patikrinkite esamas grupes iš [Office 365 iš administravimo centro](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/groups). Norėdami išspręsti šią problemą, panaikinkite esamą grupę, jei ji nebereikalingi arba sukurti svetainę su kitu priskirtu pseudonimu.

Yra įvairių būdų, kaip kurti ir naudoti modernias grupes su "SharePoint".

Esamas svetaines galite prijungti prie "Office 365" grupės. Daugiau informacijos rasite [prisijungimas prie "Office 365" grupės naudojant "SharePoint" vartotojo ineterface](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface).

Norėdami sukurti "Office 365" grupės prijungtą svetainę, turėsite sukurti komandos svetainę. Daugiau informacijos ieškokite [komandos svetainės kūrimas "SharePoint"](https://support.office.com/article/create-a-team-site-in-sharepoint-ef10c1e7-15f3-42a3-98aa-b5972711777d).

