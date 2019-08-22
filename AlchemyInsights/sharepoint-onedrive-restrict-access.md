---
title: Apriboti prieigos SharePoint arba "OneDrive"
ms.author: kirks
author: Techwriter40
ms.date: 8/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: 84f2d4b6e5fd2380a2fa96e30953c68aab203cd3
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 08/22/2019
ms.locfileid: "36559885"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a>Apriboti prieigos SharePoint arba "OneDrive"

Yra daug būdų, kaip apriboti prieigą prie SharePoint Online "OneDrive" paslaugas. Šie įvairių prieigos apribojimo metodai yra aprašytos žemiau. 

**Teisių apribojimas**

SharePoint Online ir "OneDrive" verslui, ribojame prieigą prie daiktų, pavyzdžiui, interneto svetainių, failus ir aplankus iš tik suteikiant prieigą prie šių grupių arba asmenų, kuriems reikia.

- [Pritaikyti teises į SharePoint sąraše arba bibliotekoje](https://support.office.com/article/Customize-permissions-for-a-SharePoint-list-or-library-02d770f3-59eb-4910-a608-5f84cc297782)

- [Konfigūruoti SharePoint svetainės teisės](https://docs.microsoft.com/sharepoint/customize-sharepoint-site-permissions)

- [Keisti teises poaplankis](https://support.office.com/article/Change-the-permissions-on-a-subfolder-5427BD7C-F20A-4F75-8CF2-5359DD45A1A6)

- [Valdyti prieigą iš nevaldomų įrenginių](https://docs.microsoft.com/sharepoint/control-access-from-unmanaged-devices)

Kaip SharePoint arba Globalus administratorius "Office 365", galite blokuoti arba apriboti prieigą prie SharePoint ir "OneDrive" turinį iš nevaldomų įrenginių (tų ne hibridas sujungtos arba suderinamas Intune AD).

**Tinklo vieta apribojimas**

Kaip IT administratorius gali valdyti prieigą prie SharePoint ir "OneDrive" ištekliai iš nustatytų tinklo vietas, kuriomis pasitikite. Tai taip pat žinomas kaip vietos nustatymo politiką. Norėdami gauti daugiau informacijos, žiūrėkite [Valdyti prieigą prie SharePoint Online ir "OneDrive" duomenų, atsižvelgiant į tinklo vietą](https://docs.microsoft.com/sharepoint/control-access-based-on-network-location)

**Svetainės užrakto apribojimas** 

Per SharePoint Online turite galimybę užrakinti žemyn svetainių rinkinio, todėl niekas neturi prieigos. Tai nustatoma per "PowerShell" ir [SharePoint Online valdymo aplinką](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps) naudojant [Set-SPOSite](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) - LockState nuosavybė.

**Apriboti svetainės arba antrinės svetainės**

Kaip SharePoint administravimo arba "Office 365" Globalus administratorius, galite leisti vartotojams kurti ir administruoti savo SharePoint svetaines, nustatyti, kokio pobūdžio svetainėse jie sukurti, ir nurodyti vietą svetaines. Norėdami gauti daugiau informacijos, žiūrėkite [tvarkyti svetainių kūrimą SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation)

