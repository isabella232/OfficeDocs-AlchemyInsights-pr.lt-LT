---
title: Grupės įtraukimas į SharePoint svetainę
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5200004"
- "5766"
ms.assetid: f7d730bf-0d6e-424c-970c-6137c71cb50b
ms.openlocfilehash: 8166c2a19e5849de6caace4eea0fee5866f5adc3bfc2c483f18fc788c1bf2fa9
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 08/11/2021
ms.locfileid: "57897724"
---
# <a name="common-issues-when-creating-a-group-connected-site-in-sharepoint"></a>Dažnai pasitaiko kuriant grupės prijungtą svetainę "SharePoint

1. Jei panaikinsite grupę ir jos prijungtą svetainę ir norite sukurti kitą svetainę su tuo pačiu URL, turėsite visam laikui pašalinti ankstesnę svetainę.

   - Atsisiųsti [SPO valdymo aplinką](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)
   - Daugiau informacijos apie darbo su "PowerShell" pradžia žr. [Darbo su "SharePoint Online Management Shell" pradžia](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite).
   - Pašalinkite svetainę iš panaikintų svetainių naudodami [cmdlet Remove-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) Powershell. Norint visam laikui panaikinti grupės svetaines, būtina "PowerShell".

1. Jei kuriate grupę prijungtą svetainę ir gaunate įspėjimą: Jau yra kita grupė su tuo pačiu pseudonimu , patikrinkite esamas grupes iš ["Microsoft 365" administravimo centras](https://admin.microsoft.com/AdminPortal/Home#/groups). Norėdami išspręsti šią problemą, panaikinkite esamą grupę, jei jos nebereikia, arba sukurkite svetainę su kitu priskirto pseudonimo.

1. Yra įvairių būdų kurti ir naudoti modernias grupes su SharePoint.

   - Esamas svetaines galite prijungti prie Microsoft 365 grupės. Daugiau informacijos žr. [Prisijungimas grupės Microsoft 365 naudodami SharePoint vartotojo sąsają](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface).
   - Norėdami sukurti Microsoft 365 grupės prijungtą svetainę, turėsite sukurti komandos [svetainę](https://admin.microsoft.com/sharepoint).
