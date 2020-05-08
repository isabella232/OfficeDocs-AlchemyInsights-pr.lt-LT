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
ms.openlocfilehash: b54457427ffa563b6a6323d85e1c8800191eca11
ms.sourcegitcommit: d1aad215f8aa636ba89c93a13a0c9d90e997f752
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 05/06/2020
ms.locfileid: "44064401"
---
# <a name="issues-when-creating-a-group-connected-site-in-sharepoint"></a>Problemos kuriant grupę prijungtas svetainę SharePoint

1. Kai kurios dažniausios problemos, su kuriomis susidurta kuriant arba iš naujo kuriant grupę, prijungtą svetainę.
Jei panaikinote grupę ir su ja susijusią svetainę ir norite sukurti kitą svetainę su tuo pačiu URL, turėsite visam laikui pašalinti ankstesnę svetainę.

   - Parsisiųsti [SPO valdymo shell](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)
   - Daugiau informacijos apie darbo su "PowerShell" pradžią rasite [Darbo su "SharePoint Online Management Shell" pradžia](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite).
   - Pašalinkite svetainę iš panaikintų svetainių naudodami "PowerShell" cmdlet [Remove-SPODeletedSite.](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) Norint visam laikui panaikinti grupės svetaines, reikia "PowerShell".

1. Jei kuriate grupę, susietą svetainę ir gaunate įspėjimą: **kita grupė su tuo pačiu pseudonimu jau yra**, patikrinkite esamas grupes iš ["Microsoft 365" administravimo centro](https://admin.microsoft.com/AdminPortal/Home#/groups). Norėdami išspręsti šią problemą, panaikinkite esamą grupę, jei jos nebereikia, arba sukurkite svetainę su kitu priskirtapseudoliu.

1. Šiuolaikinės grupės su "SharePoint" kuriamos ir naudojamos įvairiais būdais.

   - Esamas svetaines galite prijungti prie "Microsoft 365" grupės. Daugiau informacijos [ieškokite "Microsoft 365" grupės prijungimas naudojant "SharePoint" vartotojo sąsają](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface).
   - Norėdami sukurti "Microsoft 365" grupės prijungtą svetainę, turėsite sukurti [komandos svetainę](https://admin.microsoft.com/sharepoint).
