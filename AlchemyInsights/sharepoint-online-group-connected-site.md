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
ms.openlocfilehash: e7bfabe1555bb94e915f8544d460deecce6171be
ms.sourcegitcommit: 317eeed39c7777a922442992d67733726c41d9e1
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 02/04/2020
ms.locfileid: "41770359"
---
# <a name="issues-when-creating-a-group-connected-site-in-sharepoint"></a><span data-ttu-id="f516c-102">Problemos kuriant grupės prijungtas svetainės "SharePoint"</span><span class="sxs-lookup"><span data-stu-id="f516c-102">Issues when creating a group connected site in SharePoint</span></span>

1. <span data-ttu-id="f516c-103">Kai kurios Dažnos problemos, su kuriomis susiduriama kuriant arba iš naujo kuriant grupę prijungtą svetainę.</span><span class="sxs-lookup"><span data-stu-id="f516c-103">Some common issues encountered when creating or re-creating a group connected site.</span></span>
<span data-ttu-id="f516c-104">Jei ištrynėte grupę ir jos prijungtą svetainę ir norite sukurti kitą svetainę naudodami tą patį URL, turėsite visam laikui pašalinti ankstesnę svetainę.</span><span class="sxs-lookup"><span data-stu-id="f516c-104">If you have deleted a group and its connected site and wish to create another site with the same URL, you'll need to permanently remove the previous site.</span></span>

   - <span data-ttu-id="f516c-105">Atsisiųsti [SPO Management Shell](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)</span><span class="sxs-lookup"><span data-stu-id="f516c-105">Download [SPO Management Shell](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)</span></span>
   - <span data-ttu-id="f516c-106">Daugiau informacijos apie tai, kaip pradėti su "PowerShell", rasite [darbo su "SharePoint Online Management Shell" Pradžia](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite).</span><span class="sxs-lookup"><span data-stu-id="f516c-106">For more info on getting started with Powershell, see [Getting started with SharePoint Online Management Shell](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite).</span></span>
   - <span data-ttu-id="f516c-107">Pašalinti svetainę iš panaikintų svetainių naudojant [pašalinti SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) "PowerShell" cmdlet.</span><span class="sxs-lookup"><span data-stu-id="f516c-107">Remove the Site from Deleted Sites using the [Remove-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) Powershell cmdlet.</span></span> <span data-ttu-id="f516c-108">"PowerShell" reikia visam laikui panaikinti grupės svetainių.</span><span class="sxs-lookup"><span data-stu-id="f516c-108">Powershell is required to permanently delete group sites.</span></span>

1. <span data-ttu-id="f516c-109">Jei kuriate grupę prijungtą svetainę ir gaunate įspėjimą: **Kita grupė su tuo pačiu pseudonimu jau yra**, patikrinkite esamas grupes iš [Office 365 iš administravimo centro](https://admin.microsoft.com/AdminPortal/Home#/groups).</span><span class="sxs-lookup"><span data-stu-id="f516c-109">If you're creating a group connected site and receive a warning: **Another group with the same alias already exists**, check the existing groups from the [Office 365 from the Admin Center](https://admin.microsoft.com/AdminPortal/Home#/groups).</span></span> <span data-ttu-id="f516c-110">Norėdami išspręsti šią problemą, panaikinkite esamą grupę, jei ji nebereikalingi arba sukurti svetainę su kitu priskirtu pseudonimu.</span><span class="sxs-lookup"><span data-stu-id="f516c-110">To resolve the issue, delete the existing group if it's no longer needed or create the site with a different alias assigned.</span></span>

1. <span data-ttu-id="f516c-111">Yra įvairių būdų, kaip kurti ir naudoti modernias grupes su "SharePoint".</span><span class="sxs-lookup"><span data-stu-id="f516c-111">There are different ways to create and use modern groups with SharePoint.</span></span>

   - <span data-ttu-id="f516c-112">Esamas svetaines galite prijungti prie "Office 365" grupės.</span><span class="sxs-lookup"><span data-stu-id="f516c-112">You can connect existing sites to an Office 365 group.</span></span> <span data-ttu-id="f516c-113">Daugiau informacijos ieškokite " [Office 365" grupės prijungimas naudojant "SharePoint" vartotojo sąsają](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface).</span><span class="sxs-lookup"><span data-stu-id="f516c-113">For more info, see [Connect an Office 365 group using the SharePoint user interface](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface).</span></span>
   - <span data-ttu-id="f516c-114">Norėdami sukurti "Office 365" grupės prijungtą svetainę, turėsite sukurti [komandos svetainę](https://admin.microsoft.com/sharepoint).</span><span class="sxs-lookup"><span data-stu-id="f516c-114">To create an Office 365 group connected site, you'll need to create a [Team Site](https://admin.microsoft.com/sharepoint).</span></span>
