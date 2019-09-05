---
title: "\"SharePoint\" arba \"OneDrive\" prieigos ribojimas"
ms.author: pebaum
author: Techwriter40
ms.date: 8/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: bef0612903b9bb455aa34e90d35d6b7b9093b4e0
ms.sourcegitcommit: a65d196d00adb70045af5caca9828fe44b951f61
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 09/04/2019
ms.locfileid: "36750672"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a>"SharePoint" arba "OneDrive" prieigos ribojimas

Yra daug būdų, kaip apriboti prieigą prie SharePoint Online/OneDrive paslaugos. Šie įvairūs prieigos apribojimo metodai yra aprašyti toliau. 

**Teisių apribojimas**

"SharePoint Online" ir "OneDrive" verslui Mes ribojame prieigą prie elementų, pvz., svetainių, failų ir aplankų, suteikdami prieigą tik prie tų grupių/asmenų, kurie turi turėti prieigą.

- [Tinkinti SharePoint sąrašo arba bibliotekos teises](https://support.office.com/article/Customize-permissions-for-a-SharePoint-list-or-library-02d770f3-59eb-4910-a608-5f84cc297782)

- ["SharePoint" svetainės teisių tinkinimas](https://docs.microsoft.com/sharepoint/customize-sharepoint-site-permissions)

- [Teisių poaplankyje keitimas](https://support.office.com/article/Change-the-permissions-on-a-subfolder-5427BD7C-F20A-4F75-8CF2-5359DD45A1A6)

- [Valdykite prieigą iš nevaldomų įrenginių](https://docs.microsoft.com/sharepoint/control-access-from-unmanaged-devices)

Kaip SharePoint arba visuotinis administratorius Office 365, galite blokuoti arba apriboti prieigą prie SharePoint ir OneDrive turinį iš nevaldomų įrenginių (tų ne Hibridinis AD prisijungė arba suderinamas Intune).

**Tinklo vietos apribojimas**

Kaip IT administratorius, galite valdyti prieigą prie "SharePoint" ir "OneDrive" išteklių pagal nustatytas tinklo vietas, kuriomis pasitikite. Tai taip pat vadinama vieta grįsta politika. Daugiau informacijos rasite [Valdyti prieigą prie "SharePoint Online" ir "OneDrive" duomenų, pagrįstų tinklo vieta](https://docs.microsoft.com/sharepoint/control-access-based-on-network-location)

**Svetainės užrakto apribojimas** 

Per SharePoint Online jūs turite galimybę užrakinti žemyn svetainių rinkinio, todėl niekas neturi prieigos. Tai nustatyta per PowerShell "ir" [SharePoint Online Management Shell](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps) naudojant [Set-sposite](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) -lockstate ypatybę.

**Vartotojų apribojimas kuriant svetaines arba antrines svetaines**

Kaip SharePoint administravimo arba Office 365 visuotinio administravimo, galite leisti vartotojams kurti ir administruoti savo "SharePoint" svetaines, nustatyti, kokios svetainės jie gali kurti, ir nurodyti svetainių vietą. Norėdami gauti daugiau informacijos, žiūrėkite [tvarkyti svetainių kūrimas SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation)

