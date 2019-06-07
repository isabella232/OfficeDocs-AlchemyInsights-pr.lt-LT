---
title: Pridėti grupę prie SharePoint svetainės
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f7d730bf-0d6e-424c-970c-6137c71cb50b
ms.openlocfilehash: f0126f7f753275e9bbf8c3a09a6af5faf9a27862
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 06/07/2019
ms.locfileid: "34758738"
---
# <a name="create-group-connected-site-in-sharepoint-online"></a>Sukurti grupės prijungtai svetainei SharePoint Online

Yra keletas dažniausiai pasitaikančių problemų, su kuriomis susiduriama kuriant ar iš naujo sukurti grupę prisijungus svetainėje.

 Jei turiu ištrinti grupę ir jo prijungtai svetainei ir norite sukurti kitą svetainę su tuo pačiu URL, reikia visam laikui pašalinti prieš tai buvusios.

Parsisiųsti [SPO valdymo aplinką](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)

 Daugiau informacijos apie darbo pradžia su "PowerShell", peržiūrėkite [darbo pradžia su SharePoint Online valdymo aplinką](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps)

Pašalinti svetainės panaikinti svetaines naudojant "PowerShell" cmdlet [Remove-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) .

Jei kuriate grupę prijungtai svetainei ir gauti įspėjimą, jau egzistuoja kita grupė su to paties pseudonimo, patikrinti esamų grupių iš ["Office 365" administravimo centrą](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/groups). Išspręsti šią problemą, panaikinti esamą grupę, jei ji nebereikalinga arba sukurti svetainę su skirtingų pseudonimas priskiriamas.

Yra įvairių būdų, kaip sukurti ir naudoti šiuolaikinių grupių su "SharePoint".

Esamose svetainėse galite prisijungti prie "Office 365" grupė. Norėdami gauti daugiau informacijos, rasite [Prisijungimas naudojant SharePoint vartotojo ineterface ir "Office 365" grupė](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface).

Sukurti "Office 365" grupės prijungtą svetainę, jums reikia sukurti komandos svetainę. Daugiau informacijos rasite [sukurti komandos svetainę, SharePoint](https://support.office.com/article/create-a-team-site-in-sharepoint-ef10c1e7-15f3-42a3-98aa-b5972711777d).

