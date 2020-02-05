---
title: Grupės įtraukimas į "SharePoint" svetainę
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f7d730bf-0d6e-424c-970c-6137c71cb50b
ms.openlocfilehash: e7bfabe1555bb94e915f8544d460deecce6171be
ms.sourcegitcommit: 317eeed39c7777a922442992d67733726c41d9e1
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 02/04/2020
ms.locfileid: "41770359"
---
# <a name="issues-when-creating-a-group-connected-site-in-sharepoint"></a>Problemos kuriant grupės prijungtas svetainės "SharePoint"

1. Kai kurios Dažnos problemos, su kuriomis susiduriama kuriant arba iš naujo kuriant grupę prijungtą svetainę.
Jei ištrynėte grupę ir jos prijungtą svetainę ir norite sukurti kitą svetainę naudodami tą patį URL, turėsite visam laikui pašalinti ankstesnę svetainę.

   - Atsisiųsti [SPO Management Shell](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)
   - Daugiau informacijos apie tai, kaip pradėti su "PowerShell", rasite [darbo su "SharePoint Online Management Shell" Pradžia](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite).
   - Pašalinti svetainę iš panaikintų svetainių naudojant [pašalinti SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) "PowerShell" cmdlet. "PowerShell" reikia visam laikui panaikinti grupės svetainių.

1. Jei kuriate grupę prijungtą svetainę ir gaunate įspėjimą: **Kita grupė su tuo pačiu pseudonimu jau yra**, patikrinkite esamas grupes iš [Office 365 iš administravimo centro](https://admin.microsoft.com/AdminPortal/Home#/groups). Norėdami išspręsti šią problemą, panaikinkite esamą grupę, jei ji nebereikalingi arba sukurti svetainę su kitu priskirtu pseudonimu.

1. Yra įvairių būdų, kaip kurti ir naudoti modernias grupes su "SharePoint".

   - Esamas svetaines galite prijungti prie "Office 365" grupės. Daugiau informacijos ieškokite " [Office 365" grupės prijungimas naudojant "SharePoint" vartotojo sąsają](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface).
   - Norėdami sukurti "Office 365" grupės prijungtą svetainę, turėsite sukurti [komandos svetainę](https://admin.microsoft.com/sharepoint).
