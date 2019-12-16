---
title: "\"SharePoint\" arba \"OneDrive\" prieigos ribojimas"
ms.author: pebaum
author: pebaum
ms.date: 8/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: 242388af3ae8887616fc123f24502a8e5ac8dfbe
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 12/15/2019
ms.locfileid: "40053773"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a><span data-ttu-id="fce9e-102">"SharePoint" arba "OneDrive" prieigos ribojimas</span><span class="sxs-lookup"><span data-stu-id="fce9e-102">Restrict access in SharePoint or OneDrive</span></span>

<span data-ttu-id="fce9e-103">Yra daug būdų, kaip apriboti prieigą prie SharePoint Online/OneDrive paslaugos.</span><span class="sxs-lookup"><span data-stu-id="fce9e-103">There are many ways to restrict access to SharePoint Online/OneDrive services.</span></span> <span data-ttu-id="fce9e-104">Šie įvairūs prieigos apribojimo metodai yra aprašyti toliau.</span><span class="sxs-lookup"><span data-stu-id="fce9e-104">These various access restriction methods are outlined below.</span></span> 

<span data-ttu-id="fce9e-105">**Teisių apribojimas**</span><span class="sxs-lookup"><span data-stu-id="fce9e-105">**Permission Restriction**</span></span>

<span data-ttu-id="fce9e-106">"SharePoint Online" ir "OneDrive" verslui Mes ribojame prieigą prie elementų, pvz., svetainių, failų ir aplankų, suteikdami prieigą tik prie tų grupių/asmenų, kurie turi turėti prieigą.</span><span class="sxs-lookup"><span data-stu-id="fce9e-106">In SharePoint Online and OneDrive for Business, we restrict access to items like sites, files and folders by only granting access to those groups/individuals who should have access.</span></span>

- [<span data-ttu-id="fce9e-107">Tinkinti SharePoint sąrašo arba bibliotekos teises</span><span class="sxs-lookup"><span data-stu-id="fce9e-107">Customize permissions for a SharePoint list or library</span></span>](https://support.office.com/article/Customize-permissions-for-a-SharePoint-list-or-library-02d770f3-59eb-4910-a608-5f84cc297782)

- [<span data-ttu-id="fce9e-108">"SharePoint" svetainės teisių tinkinimas</span><span class="sxs-lookup"><span data-stu-id="fce9e-108">Customize SharePoint site permissions</span></span>](https://docs.microsoft.com/sharepoint/customize-sharepoint-site-permissions)

- [<span data-ttu-id="fce9e-109">Teisių poaplankyje keitimas</span><span class="sxs-lookup"><span data-stu-id="fce9e-109">Change the permissions on a subfolder</span></span>](https://support.office.com/article/Change-the-permissions-on-a-subfolder-5427BD7C-F20A-4F75-8CF2-5359DD45A1A6)

- [<span data-ttu-id="fce9e-110">Valdykite prieigą iš nevaldomų įrenginių</span><span class="sxs-lookup"><span data-stu-id="fce9e-110">Control access from unmanaged devices</span></span>](https://docs.microsoft.com/sharepoint/control-access-from-unmanaged-devices)

<span data-ttu-id="fce9e-111">Kaip SharePoint arba visuotinis administratorius Office 365, galite blokuoti arba apriboti prieigą prie SharePoint ir OneDrive turinį iš nevaldomų įrenginių (tų ne Hibridinis AD prisijungė arba suderinamas Intune).</span><span class="sxs-lookup"><span data-stu-id="fce9e-111">As a SharePoint or global admin in Office 365, you can block or limit access to SharePoint and OneDrive content from unmanaged devices (those not hybrid AD joined or compliant in Intune).</span></span>

<span data-ttu-id="fce9e-112">**Tinklo vietos apribojimas**</span><span class="sxs-lookup"><span data-stu-id="fce9e-112">**Network Location Restriction**</span></span>

<span data-ttu-id="fce9e-113">Kaip IT administratorius, galite valdyti prieigą prie "SharePoint" ir "OneDrive" išteklių pagal nustatytas tinklo vietas, kuriomis pasitikite.</span><span class="sxs-lookup"><span data-stu-id="fce9e-113">As an IT admin, you can control access to SharePoint and OneDrive resources based on defined network locations that you trust.</span></span> <span data-ttu-id="fce9e-114">Tai taip pat vadinama vieta grįsta politika.</span><span class="sxs-lookup"><span data-stu-id="fce9e-114">This is also known as location-based policy.</span></span> <span data-ttu-id="fce9e-115">Daugiau informacijos rasite [Valdyti prieigą prie "SharePoint Online" ir "OneDrive" duomenų, pagrįstų tinklo vieta](https://docs.microsoft.com/sharepoint/control-access-based-on-network-location)</span><span class="sxs-lookup"><span data-stu-id="fce9e-115">For more information, please see [Control access to SharePoint Online and OneDrive data based on network location](https://docs.microsoft.com/sharepoint/control-access-based-on-network-location)</span></span>

<span data-ttu-id="fce9e-116">**Svetainės užrakto apribojimas**</span><span class="sxs-lookup"><span data-stu-id="fce9e-116">**Site Lock Restriction**</span></span> 

<span data-ttu-id="fce9e-117">Per SharePoint Online jūs turite galimybę užrakinti žemyn svetainių rinkinio, todėl niekas neturi prieigos.</span><span class="sxs-lookup"><span data-stu-id="fce9e-117">Within SharePoint Online you have the ability to lock down a site collection, so no one has access.</span></span> <span data-ttu-id="fce9e-118">Tai nustatyta per PowerShell "ir" [SharePoint Online Management Shell](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps) naudojant [Set-sposite](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) -lockstate ypatybę.</span><span class="sxs-lookup"><span data-stu-id="fce9e-118">This is set via PowerShell and the [SharePoint Online Management Shell](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps) using the [Set-SPOSite](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) -LockState property.</span></span>

<span data-ttu-id="fce9e-119">**Vartotojų apribojimas kuriant svetaines arba antrines svetaines**</span><span class="sxs-lookup"><span data-stu-id="fce9e-119">**Restrict users from creating sites or subsites**</span></span>

<span data-ttu-id="fce9e-120">Kaip SharePoint administravimo arba Office 365 visuotinio administravimo, galite leisti vartotojams kurti ir administruoti savo "SharePoint" svetaines, nustatyti, kokios svetainės jie gali kurti, ir nurodyti svetainių vietą.</span><span class="sxs-lookup"><span data-stu-id="fce9e-120">As a SharePoint admin or Office 365 global admin, you can let your users create and administer their own SharePoint sites, determine what kind of sites they can create, and specify the location of the sites.</span></span> <span data-ttu-id="fce9e-121">Norėdami gauti daugiau informacijos, žiūrėkite [tvarkyti svetainių kūrimas SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation)</span><span class="sxs-lookup"><span data-stu-id="fce9e-121">For more information, please see [Manage site creation in SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation)</span></span>

