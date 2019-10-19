---
title: Grupės įtraukimas į "SharePoint" svetainę
ms.author: pebaum
author: Techwriter40
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f7d730bf-0d6e-424c-970c-6137c71cb50b
ms.openlocfilehash: 423db4e5bbb85e75aee3548d5b6b46a64ebc6fa0
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 10/18/2019
ms.locfileid: "36750528"
---
# <a name="issues-when-creating-or-group-connected-sites-in-sharepoint-online"></a><span data-ttu-id="52666-102">Problemos kuriant arba grupės prijungtas svetaines SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="52666-102">Issues when creating or group connected sites in SharePoint Online</span></span>

<span data-ttu-id="52666-103">Yra keletas bendrų problemų, su kuriomis susiduriama kuriant arba iš naujo kuriant grupę prijungtą svetainę.</span><span class="sxs-lookup"><span data-stu-id="52666-103">There are a couple of common issues encountered when creating or re-creating a group connected site.</span></span>

 <span data-ttu-id="52666-104">Jei ištrynėte grupę ir jos prijungtą svetainę ir norite sukurti kitą svetainę naudodami tą patį URL, turėsite visam laikui pašalinti ankstesnę svetainę.</span><span class="sxs-lookup"><span data-stu-id="52666-104">If you have deleted a group and its connected site and wish to create another site with the same URL, you'll need to permanently remove the previous site.</span></span>

<span data-ttu-id="52666-105">Atsisiųsti [SPO Management Shell](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)</span><span class="sxs-lookup"><span data-stu-id="52666-105">Download [SPO Management Shell](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)</span></span>

 <span data-ttu-id="52666-106">Daugiau informacijos apie tai, kaip pradėti su "PowerShell", rasite [darbo su "SharePoint Online Management Shell" Pradžia](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps)</span><span class="sxs-lookup"><span data-stu-id="52666-106">For more info on getting started with powershell, see [Getting started with SharePoint Online Management Shell](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps)</span></span>

<span data-ttu-id="52666-107">Pašalinti svetainę iš panaikintų svetainių naudojant [pašalinti SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) "PowerShell" cmdlet.</span><span class="sxs-lookup"><span data-stu-id="52666-107">Remove the Site from Deleted Sites using the [Remove-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) powershell cmdlet.</span></span>

<span data-ttu-id="52666-108">Jei kuriate grupę prijungtą svetainę ir gaunate įspėjimą kita grupė su tuo pačiu pseudonimu jau yra, patikrinkite esamas grupes iš [Office 365 iš administravimo centro](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/groups).</span><span class="sxs-lookup"><span data-stu-id="52666-108">If you're creating a group connected site and receive a warning Another group with the same alias already exists, check the existing groups from the [Office 365 from the Admin Center](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/groups).</span></span> <span data-ttu-id="52666-109">Norėdami išspręsti šią problemą, panaikinkite esamą grupę, jei ji nebereikalingi arba sukurti svetainę su kitu priskirtu pseudonimu.</span><span class="sxs-lookup"><span data-stu-id="52666-109">To resolve the issue, delete the existing group if it's no longer needed or create the site with a different alias assigned.</span></span>

<span data-ttu-id="52666-110">Yra įvairių būdų, kaip kurti ir naudoti modernias grupes su "SharePoint".</span><span class="sxs-lookup"><span data-stu-id="52666-110">There are different ways to create and use modern groups with SharePoint.</span></span>

<span data-ttu-id="52666-111">Esamas svetaines galite prijungti prie "Office 365" grupės.</span><span class="sxs-lookup"><span data-stu-id="52666-111">You can connect existing sites to an Office 365 group.</span></span> <span data-ttu-id="52666-112">Daugiau informacijos rasite [prisijungimas prie "Office 365" grupės naudojant "SharePoint" vartotojo ineterface](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface).</span><span class="sxs-lookup"><span data-stu-id="52666-112">For more info, see [Connect an Office 365 group using the SharePoint user ineterface](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface).</span></span>

<span data-ttu-id="52666-113">Norėdami sukurti "Office 365" grupės prijungtą svetainę, turėsite sukurti komandos svetainę.</span><span class="sxs-lookup"><span data-stu-id="52666-113">To create an Office 365 group connected site, you'll need to create a Team Site.</span></span> <span data-ttu-id="52666-114">Daugiau informacijos ieškokite [komandos svetainės kūrimas "SharePoint"](https://support.office.com/article/create-a-team-site-in-sharepoint-ef10c1e7-15f3-42a3-98aa-b5972711777d).</span><span class="sxs-lookup"><span data-stu-id="52666-114">For more info, see [Create a team site in SharePoint](https://support.office.com/article/create-a-team-site-in-sharepoint-ef10c1e7-15f3-42a3-98aa-b5972711777d).</span></span>

