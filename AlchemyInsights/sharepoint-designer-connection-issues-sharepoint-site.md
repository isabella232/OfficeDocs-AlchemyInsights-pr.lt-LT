---
title: SharePoint Online teisių lygiai
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f2b1b6b4-10c9-4e83-b9cb-529a0b8a3c55
ms.openlocfilehash: 356fef8e02f2c1fd9d209c68194685bb0acaa367
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 06/07/2019
ms.locfileid: "34760700"
---
# <a name="sharepoint-designer-connection-issues"></a><span data-ttu-id="001cb-102">SharePoint Designer ryšio problemas</span><span class="sxs-lookup"><span data-stu-id="001cb-102">SharePoint Designer connection issues</span></span> 

<span data-ttu-id="001cb-103">Jei SharePoint Designer patiria ryšio problemas prie SharePoint svetainės, prašome pabandyti šiuos bendrus sprendimus.</span><span class="sxs-lookup"><span data-stu-id="001cb-103">If SharePoint Designer is experiencing connection issues to SharePoint sites, please attempt the following common solutions.</span></span>

<span data-ttu-id="001cb-104">1 veiksmas: Patikrinkite, ar atnaujinta SharePoint Designer.</span><span class="sxs-lookup"><span data-stu-id="001cb-104">Step 1: Verify SharePoint Designer is updated.</span></span>

- [<span data-ttu-id="001cb-105">SharePoint Designer 2013</span><span class="sxs-lookup"><span data-stu-id="001cb-105">SharePoint Designer 2013</span></span>](https://www.microsoft.com/download/details.aspx?id=35491)

- [<span data-ttu-id="001cb-106">SharePoint Designer pakeitimų paketas 1 (SP1)</span><span class="sxs-lookup"><span data-stu-id="001cb-106">SharePoint Designer Service Pack 1 (SP1)</span></span>](https://support.microsoft.com/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1)

- [<span data-ttu-id="001cb-107">Naujinimas SharePoint Designer 2013 (KB3114721)</span><span class="sxs-lookup"><span data-stu-id="001cb-107">Update for SharePoint Designer 2013 (KB3114721)</span></span>](https://support.microsoft.com/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721)

<span data-ttu-id="001cb-108">2 veiksmas: Išvalykite vietinės talpyklos failus</span><span class="sxs-lookup"><span data-stu-id="001cb-108">Step 2: Clear the local cache files</span></span>

- <span data-ttu-id="001cb-109">Uždarykite SharePoint Designer 2013.</span><span class="sxs-lookup"><span data-stu-id="001cb-109">Close SharePoint Designer 2013.</span></span>

- <span data-ttu-id="001cb-110">Vietiniame kompiuteryje, eikite į šiuos aplankus, kuriuos norite pašalinti talpyklos failus.</span><span class="sxs-lookup"><span data-stu-id="001cb-110">On the local computer, browse to the following folders to remove cached files.</span></span>

- <span data-ttu-id="001cb-111">Spustelėkite pradėti, paleisti ir panaikinti visus failus rasti kiekvieno į žemiau vietose.</span><span class="sxs-lookup"><span data-stu-id="001cb-111">Click Start, Run and delete all files found under each of the below locations.</span></span>

<span data-ttu-id="001cb-112">%AppData%\Microsoft\Web server Extensions\Cache %APPDATA%\Microsoft\SharePoint Designer\ProxyAssemblyCache %USERPROFILE%\AppData\Local\Microsoft\WebsiteCache</span><span class="sxs-lookup"><span data-stu-id="001cb-112">%APPDATA%\Microsoft\Web Server Extensions\Cache %APPDATA%\Microsoft\SharePoint Designer\ProxyAssemblyCache %USERPROFILE%\AppData\Local\Microsoft\WebsiteCache</span></span>

<span data-ttu-id="001cb-113">Atidarykite SharePoint Designer 2013 ir įvesti sąskaitą, dar kartą Norėdami pamatyti, jei ji veikia.</span><span class="sxs-lookup"><span data-stu-id="001cb-113">Open SharePoint Designer 2013 and enter the account again to see if it works.</span></span>

<span data-ttu-id="001cb-114">3 veiksmas: [įgalinti šiuolaikinės autentifikavimas Office 2013 m. "Windows" įrenginiuose](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication?redirectSourcePath=/article/Enable-Modern-Authentication-for-Office-2013-on-Windows-devices-7dc1c01a-090f-4971-9677-f1b192d6c910&view=o365-worldwide)</span><span class="sxs-lookup"><span data-stu-id="001cb-114">Step 3: [Enable Modern Authentication for Office 2013 on Windows Devices](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication?redirectSourcePath=/article/Enable-Modern-Authentication-for-Office-2013-on-Windows-devices-7dc1c01a-090f-4971-9677-f1b192d6c910&view=o365-worldwide)</span></span>

<span data-ttu-id="001cb-115">4 žingsnis: Administratoriams reikės leisti Custom scenarijų leisti SharePoint Designer ryšį.</span><span class="sxs-lookup"><span data-stu-id="001cb-115">Step 4: Administrators will need to Allow Custom Script to allow the SharePoint Designer connection.</span></span>

<span data-ttu-id="001cb-116">Išsamius veiksmus, pavyzdžiai ir svarstymus žr [leisti arba neleisti pasirinktinį scenarijų](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).</span><span class="sxs-lookup"><span data-stu-id="001cb-116">For detailed steps, examples and considerations see [Allow or prevent custom script](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).</span></span>


