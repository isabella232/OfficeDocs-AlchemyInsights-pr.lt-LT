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
ms.openlocfilehash: db84f77208dca60c6dee98cdb0c7f1ea7fa8fe17
ms.sourcegitcommit: 204c8fadd59a597a18ebde24b3c63fbb656ec1b6
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 06/25/2019
ms.locfileid: "35223720"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a><span data-ttu-id="2e046-102">Apriboti prieigos SharePoint arba "OneDrive"</span><span class="sxs-lookup"><span data-stu-id="2e046-102">Restrict access in SharePoint or OneDrive</span></span>

<span data-ttu-id="2e046-103">Yra daug būdų, kaip apriboti prieigą prie SharePoint Online "OneDrive" paslaugas.</span><span class="sxs-lookup"><span data-stu-id="2e046-103">There are many ways to restrict access to SharePoint Online/OneDrive services.</span></span> <span data-ttu-id="2e046-104">Šie įvairių prieigos apribojimo metodai yra aprašytos žemiau.</span><span class="sxs-lookup"><span data-stu-id="2e046-104">These various access restriction methods are outlined below.</span></span> 

<span data-ttu-id="2e046-105">**Teisių apribojimas**</span><span class="sxs-lookup"><span data-stu-id="2e046-105">**Permission Restriction**</span></span>

<span data-ttu-id="2e046-106">SharePoint Online ir "OneDrive" verslui, ribojame prieigą prie daiktų, pavyzdžiui, interneto svetainių, failus ir aplankus iš tik suteikiant prieigą prie šių grupių arba asmenų, kuriems reikia.</span><span class="sxs-lookup"><span data-stu-id="2e046-106">In SharePoint Online and OneDrive for Business, we restrict access to items like sites, files and folders by only granting access to those groups/individuals who should have access.</span></span>

- [<span data-ttu-id="2e046-107">Pritaikyti teises į SharePoint sąraše arba bibliotekoje</span><span class="sxs-lookup"><span data-stu-id="2e046-107">Customize permissions for a SharePoint list or library</span></span>](https://support.office.com/article/Customize-permissions-for-a-SharePoint-list-or-library-02d770f3-59eb-4910-a608-5f84cc297782)

- [<span data-ttu-id="2e046-108">Konfigūruoti SharePoint svetainės teisės</span><span class="sxs-lookup"><span data-stu-id="2e046-108">Customize SharePoint site permissions</span></span>](https://docs.microsoft.com/sharepoint/customize-sharepoint-site-permissions)

- [<span data-ttu-id="2e046-109">Keisti teises poaplankis</span><span class="sxs-lookup"><span data-stu-id="2e046-109">Change the permissions on a subfolder</span></span>](https://support.office.com/article/Change-the-permissions-on-a-subfolder-5427BD7C-F20A-4F75-8CF2-5359DD45A1A6)

- [<span data-ttu-id="2e046-110">Valdyti prieigą iš nevaldomų įrenginių</span><span class="sxs-lookup"><span data-stu-id="2e046-110">Control access from unmanaged devices</span></span>](https://docs.microsoft.com/sharepoint/control-access-from-unmanaged-devices)

<span data-ttu-id="2e046-111">Kaip SharePoint arba Globalus administratorius "Office 365", galite blokuoti arba apriboti prieigą prie SharePoint ir "OneDrive" turinį iš nevaldomų įrenginių (tų ne hibridas sujungtos arba suderinamas Intune AD).</span><span class="sxs-lookup"><span data-stu-id="2e046-111">As a SharePoint or global admin in Office 365, you can block or limit access to SharePoint and OneDrive content from unmanaged devices (those not hybrid AD joined or compliant in Intune).</span></span>

<span data-ttu-id="2e046-112">**Tinklo vieta apribojimas**</span><span class="sxs-lookup"><span data-stu-id="2e046-112">**Network Location Restriction**</span></span>

<span data-ttu-id="2e046-113">Kaip IT administratorius gali valdyti prieigą prie SharePoint ir "OneDrive" ištekliai iš nustatytų tinklo vietas, kuriomis pasitikite.</span><span class="sxs-lookup"><span data-stu-id="2e046-113">As an IT admin, you can control access to SharePoint and OneDrive resources based on defined network locations that you trust.</span></span> <span data-ttu-id="2e046-114">Tai taip pat žinomas kaip vietos nustatymo politiką.</span><span class="sxs-lookup"><span data-stu-id="2e046-114">This is also known as location-based policy.</span></span> <span data-ttu-id="2e046-115">Norėdami gauti daugiau informacijos, žiūrėkite [Valdyti prieigą prie SharePoint Online ir "OneDrive" duomenų, atsižvelgiant į tinklo vietą](https://docs.microsoft.com/sharepoint/control-access-based-on-network-location)</span><span class="sxs-lookup"><span data-stu-id="2e046-115">For more information, please see [Control access to SharePoint Online and OneDrive data based on network location](https://docs.microsoft.com/sharepoint/control-access-based-on-network-location)</span></span>

<span data-ttu-id="2e046-116">**Svetainės užrakto apribojimas**</span><span class="sxs-lookup"><span data-stu-id="2e046-116">**Site Lock Restriction**</span></span> 

<span data-ttu-id="2e046-117">Per SharePoint Online turite galimybę užrakinti žemyn svetainių rinkinio, todėl niekas neturi prieigos.</span><span class="sxs-lookup"><span data-stu-id="2e046-117">Within SharePoint Online you have the ability to lock down a site collection, so no one has access.</span></span> <span data-ttu-id="2e046-118">Tai nustatoma per "PowerShell" ir [SharePoint Online valdymo aplinką](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps) naudojant [Set-SPOSite](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) - LockState nuosavybė.</span><span class="sxs-lookup"><span data-stu-id="2e046-118">This is set via PowerShell and the [SharePoint Online Management Shell](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps) using the [Set-SPOSite](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) -LockState property.</span></span>

<span data-ttu-id="2e046-119">**Apriboti svetainės arba antrinės svetainės**</span><span class="sxs-lookup"><span data-stu-id="2e046-119">**Restrict users from creating sites or subsites**</span></span>

<span data-ttu-id="2e046-120">Kaip SharePoint administravimo arba "Office 365" Globalus administratorius, galite leisti vartotojams kurti ir administruoti savo SharePoint svetaines, nustatyti, kokio pobūdžio svetainėse jie sukurti, ir nurodyti vietą svetaines.</span><span class="sxs-lookup"><span data-stu-id="2e046-120">As a SharePoint admin or Office 365 global admin, you can let your users create and administer their own SharePoint sites, determine what kind of sites they can create, and specify the location of the sites.</span></span> <span data-ttu-id="2e046-121">Norėdami gauti daugiau informacijos, žiūrėkite [tvarkyti svetainių kūrimą SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation)</span><span class="sxs-lookup"><span data-stu-id="2e046-121">For more information, please see [Manage site creation in SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation)</span></span>

