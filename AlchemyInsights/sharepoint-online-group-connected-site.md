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
ms.openlocfilehash: 352bad1b8fe219f95a37c9ac268c6c4dd8801dfc
ms.sourcegitcommit: 6d341637dbb14e90726a1ce1d68f077ace9bb765
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 06/04/2019
ms.locfileid: "34719489"
---
# <a name="create-group-connected-site-in-sharepoint-online"></a>Sukurti grupės prijungtai svetainei SharePoint Online

<p><strong>Yra keletas dažniausiai pasitaikančių problemų, su kuriomis susiduriama kuriant ar iš naujo sukurti grupę prisijungus svetainėje.&nbsp;</strong></p>  <p>1.Jei turiu ištrinti grupę ir jo prijungtai svetainei ir norite sukurti kitą svetainę su tuo pačiu URL, reikia visam laikui pašalinti prieš tai buvusios.</p>  <ul>  <li>Atsisiųsti <a title="SPO valdymo aplinką" href="https://support.office.com/en-ie/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429">SPO Management Shell</a> - daugiau informacijos apie darbo pradžia su "PowerShell", rasite <a title="pradėjo dirbti su SharePoint Online valdymo aplinką" href="https://docs.microsoft.com/en-us/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps">Darbo pradžia su SharePoint Online valdymo aplinką</a>. <br /><br /></li>  <li>Pašalinti svetainės panaikinti svetaines naudojant į <a title="pašalinti-SPODeletedSite" href="https://docs.microsoft.com/en-us/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps">Pašalinti-SPODeletedSite</a> "PowerShell" cmdlet.</li>  </ul>  <p>Jei kuriate grupę prijungtai svetainei ir gauti įspėjimą <strong>'kita grupė su to paties pseudonimo jau egzistuoja'</strong>, patikrinkite, ar iš esamų grupių, <a title=""Office 365" administravimo centrą" href="https://admin.microsoft.com/Adminportal/Home?source=applauncher#/groups">"Office 365" administravimo centrą</a>. Išspręsti šią problemą, panaikinti esamą grupę, jei ji nebereikalinga arba sukurti svetainę su skirtingų pseudonimas priskiriamas.&nbsp;</p>  <p><strong>Yra įvairių būdų, kaip sukurti ir naudoti šiuolaikinių grupių su "SharePoint".&nbsp;</strong></p>  <ol>  <li>Esamose svetainėse galite prisijungti prie "Office 365" grupė. Daugiau informacijos rasite <a title="prisijungti "Office 365" grupei, naudojant SharePoint vartotojo ineterface" href="https://docs.microsoft.com/en-us/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface">Prisijungti "Office 365" grupei, naudojant SharePoint vartotojo ineterface</a>.</li>  <li>Sukurti "Office 365" grupės prijungtą svetainę, jums reikia sukurti komandos svetainę. Daugiau informacijos rasite <a title="sukurti komandos svetainę, SharePoint" href="https://support.office.com/en-us/article/create-a-team-site-in-sharepoint-ef10c1e7-15f3-42a3-98aa-b5972711777d">Sukurti komandos svetainę, SharePoint.</a></li>  </ol>

