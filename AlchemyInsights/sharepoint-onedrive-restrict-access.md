---
title: "\"SharePoint\" arba \"OneDrive\" prieigos apribojimas"
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: e9eb1822a7770bc206992cc5fb7e54a5c972b7e2
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47700463"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a><span data-ttu-id="d747d-102">"SharePoint" arba "OneDrive" prieigos apribojimas</span><span class="sxs-lookup"><span data-stu-id="d747d-102">Restrict access in SharePoint or OneDrive</span></span>

<span data-ttu-id="d747d-103">Yra daug būdų, kaip apriboti prieigą prie "SharePoint Online"/"OneDrive" tarnybų.</span><span class="sxs-lookup"><span data-stu-id="d747d-103">There are many ways to restrict access to SharePoint Online/OneDrive services.</span></span> <span data-ttu-id="d747d-104">Šie įvairūs prieigos apribojimo metodai aprašyti toliau.</span><span class="sxs-lookup"><span data-stu-id="d747d-104">These various access restriction methods are outlined below.</span></span> 

<span data-ttu-id="d747d-105">**Teisių apribojimas**</span><span class="sxs-lookup"><span data-stu-id="d747d-105">**Permission Restriction**</span></span>

<span data-ttu-id="d747d-106">"SharePoint Online" ir "OneDrive" verslui ribojame prieigą prie elementų, pvz., svetainių, failų ir aplankų, tik suteikia prieigą prie tų grupių ar asmenų, kurie turėtų turėti prieigą.</span><span class="sxs-lookup"><span data-stu-id="d747d-106">In SharePoint Online and OneDrive for Business, we restrict access to items like sites, files and folders by only granting access to those groups/individuals who should have access.</span></span>

- [<span data-ttu-id="d747d-107">"SharePoint" sąrašo ar bibliotekos teisių tinkinimas</span><span class="sxs-lookup"><span data-stu-id="d747d-107">Customize permissions for a SharePoint list or library</span></span>](https://support.office.com/article/Customize-permissions-for-a-SharePoint-list-or-library-02d770f3-59eb-4910-a608-5f84cc297782)

- [<span data-ttu-id="d747d-108">"SharePoint" svetainės teisių tinkinimas</span><span class="sxs-lookup"><span data-stu-id="d747d-108">Customize SharePoint site permissions</span></span>](https://docs.microsoft.com/sharepoint/customize-sharepoint-site-permissions)

- [<span data-ttu-id="d747d-109">Poaplankių teisių keitimas</span><span class="sxs-lookup"><span data-stu-id="d747d-109">Change the permissions on a subfolder</span></span>](https://support.office.com/article/Change-the-permissions-on-a-subfolder-5427BD7C-F20A-4F75-8CF2-5359DD45A1A6)

- [<span data-ttu-id="d747d-110">Valdyti prieigą iš nevaldomų įrenginių</span><span class="sxs-lookup"><span data-stu-id="d747d-110">Control access from unmanaged devices</span></span>](https://docs.microsoft.com/sharepoint/control-access-from-unmanaged-devices)

<span data-ttu-id="d747d-111">Kaip "SharePoint" arba visuotinis administratorius galite užblokuoti arba apriboti prieigą prie "SharePoint" ir "OneDrive" turinio iš nevaldomų įrenginių (tų, kurie nėra hibridinio skelbimo arba atitinkantys "Intune").</span><span class="sxs-lookup"><span data-stu-id="d747d-111">As a SharePoint or global admin, you can block or limit access to SharePoint and OneDrive content from unmanaged devices (those not hybrid AD joined or compliant in Intune).</span></span>

<span data-ttu-id="d747d-112">**Tinklo vietos apribojimas**</span><span class="sxs-lookup"><span data-stu-id="d747d-112">**Network Location Restriction**</span></span>

<span data-ttu-id="d747d-113">Kaip IT administratorius galite valdyti prieigą prie "SharePoint" ir "OneDrive" išteklių pagal apibrėžtas tinklo vietas, kurias pasitikite.</span><span class="sxs-lookup"><span data-stu-id="d747d-113">As an IT admin, you can control access to SharePoint and OneDrive resources based on defined network locations that you trust.</span></span> <span data-ttu-id="d747d-114">Tai taip pat vadinama vietos nustatymo politika.</span><span class="sxs-lookup"><span data-stu-id="d747d-114">This is also known as location-based policy.</span></span> <span data-ttu-id="d747d-115">Daugiau informacijos ieškokite straipsnyje [prieigos prie "SharePoint Online" ir "OneDrive" duomenų valdymas, pagrįstas tinklo vieta](https://docs.microsoft.com/sharepoint/control-access-based-on-network-location)</span><span class="sxs-lookup"><span data-stu-id="d747d-115">For more information, please see [Control access to SharePoint Online and OneDrive data based on network location](https://docs.microsoft.com/sharepoint/control-access-based-on-network-location)</span></span>

<span data-ttu-id="d747d-116">**Svetainės užrakto apribojimas**</span><span class="sxs-lookup"><span data-stu-id="d747d-116">**Site Lock Restriction**</span></span> 

<span data-ttu-id="d747d-117">"SharePoint Online" turite galimybę užrakinti svetainių rinkinį, kad niekas negalėtų pasiekti.</span><span class="sxs-lookup"><span data-stu-id="d747d-117">Within SharePoint Online you have the ability to lock down a site collection, so no one has access.</span></span> <span data-ttu-id="d747d-118">Tai nustatyta "PowerShell" ir " [SharePoint Online Management Shell](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps) " naudojant ypatybę [Set-sposite](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) -lockstate.</span><span class="sxs-lookup"><span data-stu-id="d747d-118">This is set via PowerShell and the [SharePoint Online Management Shell](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps) using the [Set-SPOSite](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) -LockState property.</span></span>

<span data-ttu-id="d747d-119">**Vartotojų apribojimas kuriant svetaines arba antrines svetaines**</span><span class="sxs-lookup"><span data-stu-id="d747d-119">**Restrict users from creating sites or subsites**</span></span>

<span data-ttu-id="d747d-120">Kaip "SharePoint" administratorius arba visuotinis administratorius galite leisti vartotojams kurti ir administruoti savo "SharePoint" svetaines, nustatyti, kokias svetaines jie gali sukurti ir nurodyti svetainių vietą.</span><span class="sxs-lookup"><span data-stu-id="d747d-120">As a SharePoint admin or Global admin, you can let your users create and administer their own SharePoint sites, determine what kind of sites they can create, and specify the location of the sites.</span></span> <span data-ttu-id="d747d-121">Daugiau informacijos ieškokite " [SharePoint Online" svetainės kūrimo valdymas](https://docs.microsoft.com/sharepoint/manage-site-creation)</span><span class="sxs-lookup"><span data-stu-id="d747d-121">For more information, please see [Manage site creation in SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation)</span></span>

