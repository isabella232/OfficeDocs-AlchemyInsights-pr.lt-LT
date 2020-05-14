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
ms.openlocfilehash: b54457427ffa563b6a6323d85e1c8800191eca11
ms.sourcegitcommit: a98b25fa3cac9ebba983f4932881d774880aca93
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 05/13/2020
ms.locfileid: "44064401"
---
# <a name="issues-when-creating-a-group-connected-site-in-sharepoint"></a><span data-ttu-id="0f7cb-102">Problemos kuriant grupę prijungtas svetainę SharePoint</span><span class="sxs-lookup"><span data-stu-id="0f7cb-102">Issues when creating a group connected site in SharePoint</span></span>

1. <span data-ttu-id="0f7cb-103">Kai kurios dažniausios problemos, su kuriomis susidurta kuriant arba iš naujo kuriant grupę, prijungtą svetainę.</span><span class="sxs-lookup"><span data-stu-id="0f7cb-103">Some common issues encountered when creating or re-creating a group connected site.</span></span>
<span data-ttu-id="0f7cb-104">Jei panaikinote grupę ir su ja susijusią svetainę ir norite sukurti kitą svetainę su tuo pačiu URL, turėsite visam laikui pašalinti ankstesnę svetainę.</span><span class="sxs-lookup"><span data-stu-id="0f7cb-104">If you have deleted a group and its connected site and wish to create another site with the same URL, you'll need to permanently remove the previous site.</span></span>

   - <span data-ttu-id="0f7cb-105">Parsisiųsti [SPO valdymo shell](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)</span><span class="sxs-lookup"><span data-stu-id="0f7cb-105">Download [SPO Management Shell](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)</span></span>
   - <span data-ttu-id="0f7cb-106">Daugiau informacijos apie darbo su "PowerShell" pradžią rasite [Darbo su "SharePoint Online Management Shell" pradžia](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite).</span><span class="sxs-lookup"><span data-stu-id="0f7cb-106">For more info on getting started with Powershell, see [Getting started with SharePoint Online Management Shell](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite).</span></span>
   - <span data-ttu-id="0f7cb-107">Pašalinkite svetainę iš panaikintų svetainių naudodami "PowerShell" cmdlet [Remove-SPODeletedSite.](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps)</span><span class="sxs-lookup"><span data-stu-id="0f7cb-107">Remove the Site from Deleted Sites using the [Remove-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) Powershell cmdlet.</span></span> <span data-ttu-id="0f7cb-108">Norint visam laikui panaikinti grupės svetaines, reikia "PowerShell".</span><span class="sxs-lookup"><span data-stu-id="0f7cb-108">Powershell is required to permanently delete group sites.</span></span>

1. <span data-ttu-id="0f7cb-109">Jei kuriate grupę, susietą svetainę ir gaunate įspėjimą: **kita grupė su tuo pačiu pseudonimu jau yra**, patikrinkite esamas grupes iš ["Microsoft 365" administravimo centro](https://admin.microsoft.com/AdminPortal/Home#/groups).</span><span class="sxs-lookup"><span data-stu-id="0f7cb-109">If you're creating a group connected site and receive a warning: **Another group with the same alias already exists**, check the existing groups from the [Microsoft 365 admin center](https://admin.microsoft.com/AdminPortal/Home#/groups).</span></span> <span data-ttu-id="0f7cb-110">Norėdami išspręsti šią problemą, panaikinkite esamą grupę, jei jos nebereikia, arba sukurkite svetainę su kitu priskirtapseudoliu.</span><span class="sxs-lookup"><span data-stu-id="0f7cb-110">To resolve the issue, delete the existing group if it's no longer needed or create the site with a different alias assigned.</span></span>

1. <span data-ttu-id="0f7cb-111">Šiuolaikinės grupės su "SharePoint" kuriamos ir naudojamos įvairiais būdais.</span><span class="sxs-lookup"><span data-stu-id="0f7cb-111">There are different ways to create and use modern groups with SharePoint.</span></span>

   - <span data-ttu-id="0f7cb-112">Esamas svetaines galite prijungti prie "Microsoft 365" grupės.</span><span class="sxs-lookup"><span data-stu-id="0f7cb-112">You can connect existing sites to an Microsoft 365 group.</span></span> <span data-ttu-id="0f7cb-113">Daugiau informacijos [ieškokite "Microsoft 365" grupės prijungimas naudojant "SharePoint" vartotojo sąsają](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface).</span><span class="sxs-lookup"><span data-stu-id="0f7cb-113">For more info, see [Connect an Microsoft 365 group using the SharePoint user interface](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface).</span></span>
   - <span data-ttu-id="0f7cb-114">Norėdami sukurti "Microsoft 365" grupės prijungtą svetainę, turėsite sukurti [komandos svetainę](https://admin.microsoft.com/sharepoint).</span><span class="sxs-lookup"><span data-stu-id="0f7cb-114">To create an Microsoft 365 group connected site, you'll need to create a [Team Site](https://admin.microsoft.com/sharepoint).</span></span>
