---
title: "\"SharePoint\" arba \"OneDrive\" prieigos apribojimas"
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: e9eb1822a7770bc206992cc5fb7e54a5c972b7e2
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47700463"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a>"SharePoint" arba "OneDrive" prieigos apribojimas

Yra daug būdų, kaip apriboti prieigą prie "SharePoint Online"/"OneDrive" tarnybų. Šie įvairūs prieigos apribojimo metodai aprašyti toliau. 

**Teisių apribojimas**

"SharePoint Online" ir "OneDrive" verslui ribojame prieigą prie elementų, pvz., svetainių, failų ir aplankų, tik suteikia prieigą prie tų grupių ar asmenų, kurie turėtų turėti prieigą.

- ["SharePoint" sąrašo ar bibliotekos teisių tinkinimas](https://support.office.com/article/Customize-permissions-for-a-SharePoint-list-or-library-02d770f3-59eb-4910-a608-5f84cc297782)

- ["SharePoint" svetainės teisių tinkinimas](https://docs.microsoft.com/sharepoint/customize-sharepoint-site-permissions)

- [Poaplankių teisių keitimas](https://support.office.com/article/Change-the-permissions-on-a-subfolder-5427BD7C-F20A-4F75-8CF2-5359DD45A1A6)

- [Valdyti prieigą iš nevaldomų įrenginių](https://docs.microsoft.com/sharepoint/control-access-from-unmanaged-devices)

Kaip "SharePoint" arba visuotinis administratorius galite užblokuoti arba apriboti prieigą prie "SharePoint" ir "OneDrive" turinio iš nevaldomų įrenginių (tų, kurie nėra hibridinio skelbimo arba atitinkantys "Intune").

**Tinklo vietos apribojimas**

Kaip IT administratorius galite valdyti prieigą prie "SharePoint" ir "OneDrive" išteklių pagal apibrėžtas tinklo vietas, kurias pasitikite. Tai taip pat vadinama vietos nustatymo politika. Daugiau informacijos ieškokite straipsnyje [prieigos prie "SharePoint Online" ir "OneDrive" duomenų valdymas, pagrįstas tinklo vieta](https://docs.microsoft.com/sharepoint/control-access-based-on-network-location)

**Svetainės užrakto apribojimas** 

"SharePoint Online" turite galimybę užrakinti svetainių rinkinį, kad niekas negalėtų pasiekti. Tai nustatyta "PowerShell" ir " [SharePoint Online Management Shell](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps) " naudojant ypatybę [Set-sposite](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) -lockstate.

**Vartotojų apribojimas kuriant svetaines arba antrines svetaines**

Kaip "SharePoint" administratorius arba visuotinis administratorius galite leisti vartotojams kurti ir administruoti savo "SharePoint" svetaines, nustatyti, kokias svetaines jie gali sukurti ir nurodyti svetainių vietą. Daugiau informacijos ieškokite " [SharePoint Online" svetainės kūrimo valdymas](https://docs.microsoft.com/sharepoint/manage-site-creation)

