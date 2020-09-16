---
title: Grupės įtraukimas į "SharePoint" svetainę
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
ms.assetid: f7d730bf-0d6e-424c-970c-6137c71cb50b
ms.openlocfilehash: 9bec2f71465e43e1c3cba038e0e68949672ceb8a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 09/15/2020
ms.locfileid: "47771216"
---
# <a name="issues-when-creating-a-group-connected-site-in-sharepoint"></a>Problemos kuriant grupės prijungtą svetainę "SharePoint"

1. Kai kurios Dažniausios problemos, su kuriomis susiduriama kuriant arba iš naujo kuriant grupės prijungtą svetainę.
Jei panaikinote grupę ir jos prijungtą svetainę ir norite sukurti kitą svetainę su tuo pačiu URL, turėsite visam laikui pašalinti ankstesnę svetainę.

   - Atsisiųsti [SPO valdymo aplinką](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)
   - Daugiau informacijos apie tai, kaip pradėti naudoti "PowerShell", rasite [darbo su "SharePoint Online Management Shell" Pradžia](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite).
   - Pašalinkite svetainę iš panaikintų svetainių, naudodami " [Remove-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) PowerShell" cmdlet. "PowerShell" būtina visam laikui panaikinti grupės svetaines.

1. Jei kuriate grupės prijungtą svetainę ir gaunate įspėjimą: **Kita grupė su tuo pačiu pseudonimu jau yra**, pažymėkite esamas grupes iš ["Microsoft" 365 administravimo centro](https://admin.microsoft.com/AdminPortal/Home#/groups). Norėdami išspręsti šią problemą, panaikinkite esamą grupę, jei jos nebereikia arba sukuriate svetainę su kitu pseudonimu.

1. Yra įvairių būdų, kaip kurti ir naudoti šiuolaikines grupes naudojant "SharePoint".

   - Galite prijungti esamas svetaines prie "Microsoft" 365 grupės. Daugiau informacijos ieškokite ["Microsoft 365" grupės prijungimas naudojant "SharePoint" vartotojo sąsają](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface).
   - Norėdami sukurti "Microsoft" 365 grupės prijungtą svetainę, turėsite sukurti [komandos svetainę](https://admin.microsoft.com/sharepoint).
