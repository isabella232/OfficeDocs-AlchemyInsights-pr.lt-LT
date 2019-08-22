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
ms.openlocfilehash: 6aea12d44a44a3e11eaf3fb1bd47ff3e9dbfd9e7
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 08/22/2019
ms.locfileid: "36507855"
---
# <a name="issues-when-creating-or-group-connected-sites-in-sharepoint-online"></a><span data-ttu-id="aa8f7-102">Problemos, kai kuriant ar grupė susijusių svetainių SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="aa8f7-102">Issues when creating or group connected sites in SharePoint Online</span></span>

<span data-ttu-id="aa8f7-103">Yra keletas dažniausiai pasitaikančių problemų, su kuriomis susiduriama kuriant ar iš naujo sukurti grupę prisijungus svetainėje.</span><span class="sxs-lookup"><span data-stu-id="aa8f7-103">There are a couple of common issues encountered when creating or re-creating a group connected site.</span></span>

 <span data-ttu-id="aa8f7-104">Jei turiu ištrinti grupę ir jo prijungtai svetainei ir norite sukurti kitą svetainę su tuo pačiu URL, reikia visam laikui pašalinti prieš tai buvusios.</span><span class="sxs-lookup"><span data-stu-id="aa8f7-104">If you have deleted a group and its connected site and wish to create another site with the same URL, you'll need to permanently remove the previous site.</span></span>

<span data-ttu-id="aa8f7-105">Parsisiųsti [SPO valdymo aplinką](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)</span><span class="sxs-lookup"><span data-stu-id="aa8f7-105">Download [SPO Management Shell](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)</span></span>

 <span data-ttu-id="aa8f7-106">Daugiau informacijos apie darbo pradžia su "PowerShell", peržiūrėkite [darbo pradžia su SharePoint Online valdymo aplinką](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps)</span><span class="sxs-lookup"><span data-stu-id="aa8f7-106">For more info on getting started with powershell, see [Getting started with SharePoint Online Management Shell](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps)</span></span>

<span data-ttu-id="aa8f7-107">Pašalinti svetainės panaikinti svetaines naudojant "PowerShell" cmdlet [Remove-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) .</span><span class="sxs-lookup"><span data-stu-id="aa8f7-107">Remove the Site from Deleted Sites using the [Remove-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) powershell cmdlet.</span></span>

<span data-ttu-id="aa8f7-108">Jei kuriate grupę prijungtai svetainei ir gauti įspėjimą, jau egzistuoja kita grupė su to paties pseudonimo, patikrinti esamų grupių iš ["Office 365" administravimo centrą](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/groups).</span><span class="sxs-lookup"><span data-stu-id="aa8f7-108">If you're creating a group connected site and receive a warning Another group with the same alias already exists, check the existing groups from the [Office 365 from the Admin Center](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/groups).</span></span> <span data-ttu-id="aa8f7-109">Išspręsti šią problemą, panaikinti esamą grupę, jei ji nebereikalinga arba sukurti svetainę su skirtingų pseudonimas priskiriamas.</span><span class="sxs-lookup"><span data-stu-id="aa8f7-109">To resolve the issue, delete the existing group if it's no longer needed or create the site with a different alias assigned.</span></span>

<span data-ttu-id="aa8f7-110">Yra įvairių būdų, kaip sukurti ir naudoti šiuolaikinių grupių su "SharePoint".</span><span class="sxs-lookup"><span data-stu-id="aa8f7-110">There are different ways to create and use modern groups with SharePoint.</span></span>

<span data-ttu-id="aa8f7-111">Esamose svetainėse galite prisijungti prie "Office 365" grupė.</span><span class="sxs-lookup"><span data-stu-id="aa8f7-111">You can connect existing sites to an Office 365 group.</span></span> <span data-ttu-id="aa8f7-112">Norėdami gauti daugiau informacijos, rasite [Prisijungimas naudojant SharePoint vartotojo ineterface ir "Office 365" grupė](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface).</span><span class="sxs-lookup"><span data-stu-id="aa8f7-112">For more info, see [Connect an Office 365 group using the SharePoint user ineterface](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface).</span></span>

<span data-ttu-id="aa8f7-113">Sukurti "Office 365" grupės prijungtą svetainę, jums reikia sukurti komandos svetainę.</span><span class="sxs-lookup"><span data-stu-id="aa8f7-113">To create an Office 365 group connected site, you'll need to create a Team Site.</span></span> <span data-ttu-id="aa8f7-114">Daugiau informacijos rasite [sukurti komandos svetainę, SharePoint](https://support.office.com/article/create-a-team-site-in-sharepoint-ef10c1e7-15f3-42a3-98aa-b5972711777d).</span><span class="sxs-lookup"><span data-stu-id="aa8f7-114">For more info, see [Create a team site in SharePoint](https://support.office.com/article/create-a-team-site-in-sharepoint-ef10c1e7-15f3-42a3-98aa-b5972711777d).</span></span>

