---
title: Prieigos apribojimas SharePoint arba "OneDrive"
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: fc6731d5a7747bb4fc8d6cef1b6ac0045d11917d7f97abbb21eea9613b1b1aa2
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54093842"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a>Prieigos apribojimas SharePoint arba "OneDrive"

Yra daug būdų apriboti prieigą prie "SharePoint/ "OneDrive" tarnybų. Šie įvairūs prieigos apribojimo metodai pateikiami toliau. 

**Teisių apribojimas**

"SharePoint Online" ir ""OneDrive" verslui" ribojame prieigą prie elementų, pvz., svetainių, failų ir aplankų, suteikdami prieigą tik toms grupėms / asmenims, kurie turėtų turėti prieigą.

- [Sąrašo arba bibliotekos SharePoint teisių tinkinimas](https://support.office.com/article/Customize-permissions-for-a-SharePoint-list-or-library-02d770f3-59eb-4910-a608-5f84cc297782)

- [Svetainės SharePoint tinkinimas](https://docs.microsoft.com/sharepoint/customize-sharepoint-site-permissions)

- [Poaplankio teisių keitimas](https://support.office.com/article/Change-the-permissions-on-a-subfolder-5427BD7C-F20A-4F75-8CF2-5359DD45A1A6)

- [Prieigos iš nevaldų įrenginių valdymas](https://docs.microsoft.com/sharepoint/control-access-from-unmanaged-devices)

Kaip "SharePoint" arba visuotinis administratorius, galite blokuoti arba apriboti prieigą prie "SharePoint" ir ""OneDrive"" turinio nevaldantuose įrenginiuose (kurie nėra hibridiniai AD sujungti arba suderinami su "Intune").

**Tinklo vietos apribojimas**

Kaip IT administratorius, galite valdyti prieigą prie SharePoint "OneDrive" išteklių pagal apibrėžtas tinklo vietas, kurias pasitikite. Tai taip pat vadinama vieta pagrįsta strategija. Daugiau informacijos žr. Prieigos prie interneto [ir SharePoint duomenų "OneDrive" valdymas atsižvelgiant į tinklo vietą](https://docs.microsoft.com/sharepoint/control-access-based-on-network-location)

**Svetainės užrakto apribojimas** 

Internetinėje SharePoint turite galimybę užrakinti svetainių rinkinį, todėl niekas neturi prieigos. Tai nustatyta naudojant "PowerShell" [ir "SharePoint Online Management Shell"](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps) naudojant [ypatybę Set-SPOSite](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) -LockState.

**Vartotojų galimybės kurti svetaines arba antrinius tinklalapius apribojimas**

Kaip SharePoint administratorius arba visuotinis administratorius, galite leisti vartotojams kurti ir administruoti savo "SharePoint svetaines, nustatyti, kokio tipo svetaines jie gali kurti, ir nurodyti svetainių vietą. Daugiau informacijos žr. Svetainės [kūrimo valdymas "SharePoint Online"](https://docs.microsoft.com/sharepoint/manage-site-creation)

