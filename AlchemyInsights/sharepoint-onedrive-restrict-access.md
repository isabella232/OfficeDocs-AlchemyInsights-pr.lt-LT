---
title: Prieigos ribojimas "SharePoint" arba "OneDrive"
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: 39aa8cd6e649eca4a1e196eeb589a825364d0977
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 04/22/2020
ms.locfileid: "43692773"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a>Prieigos ribojimas "SharePoint" arba "OneDrive"

Yra daug būdų, kaip apriboti prieigą prie "SharePoint Online" / "OneDrive" paslaugų. Šie įvairūs prieigos apribojimo metodai nurodyti toliau. 

**Teisių apribojimas**

"SharePoint Online" ir "OneDrive" verslui ribojame prieigą prie elementų, pvz., svetainių, failų ir aplankų, suteikdami prieigą tik tiems grupėms / asmenims, kurie turėtų turėti prieigą.

- ["SharePoint" sąrašo arba bibliotekos teisių tinkinimas](https://support.office.com/article/Customize-permissions-for-a-SharePoint-list-or-library-02d770f3-59eb-4910-a608-5f84cc297782)

- ["SharePoint" svetainės teisių tinkinimas](https://docs.microsoft.com/sharepoint/customize-sharepoint-site-permissions)

- [Poaplankio teisių keitimas](https://support.office.com/article/Change-the-permissions-on-a-subfolder-5427BD7C-F20A-4F75-8CF2-5359DD45A1A6)

- [Prieigos iš nevaldomų įrenginių valdymas](https://docs.microsoft.com/sharepoint/control-access-from-unmanaged-devices)

Kaip "SharePoint" arba visuotinis administratorius galite blokuoti arba apriboti prieigą prie "SharePoint" ir "OneDrive" turinio iš nevaldomų įrenginių (tų, kurie neprisijungė prie "Intune" arba nėra suderinami su "Ad").

**Tinklo vietos apribojimas**

Kaip IT administratorius galite valdyti prieigą prie "SharePoint" ir "OneDrive" išteklių pagal nustatytas tinklo vietas, kuriomis pasitikite. Tai taip pat vadinama vietove pagrįsta strategija. Daugiau informacijos rasite ["SharePoint Online" ir "OneDrive" duomenų valdymas pagal tinklo vietą](https://docs.microsoft.com/sharepoint/control-access-based-on-network-location)

**Svetainės užrakto apribojimas** 

"SharePoint Online" sistemoje turite galimybę užrakinti svetainių rinkinį, todėl niekas neturi prieigos. Tai nustatyta per "PowerShell" ir ["SharePoint Online" valdymo aplinkoje](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps) naudojant [ypatybę Set-SPOSite](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) -LockState .

**Vartotojų nekūrimas nuo svetainių ar antrinių svetainių kūrimo**

Kaip "SharePoint" administratorius arba visuotinis administratorius, galite leisti vartotojams kurti ir administruoti savo "SharePoint" svetaines, nustatyti, kokias svetaines jie gali kurti, ir nurodyti svetainių vietą. Daugiau informacijos rasite [Svetainės kūrimo valdymas "SharePoint Online"](https://docs.microsoft.com/sharepoint/manage-site-creation)

