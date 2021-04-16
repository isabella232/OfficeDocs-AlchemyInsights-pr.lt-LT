---
title: OneDrive for Business Web OneDrive redirects to Delve
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1870"
- "900072"
ms.openlocfilehash: 96f23585f7cbce672842f6330ba79816f24dbc41
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 04/15/2021
ms.locfileid: "51799997"
---
# <a name="redirected-to-delve-after-you-click-onedrive"></a><span data-ttu-id="6fe99-102">Peradresuota į "Delve" spustelėjus "OneDrive"</span><span class="sxs-lookup"><span data-stu-id="6fe99-102">Redirected to Delve after you click OneDrive</span></span>

<span data-ttu-id="6fe99-103">Žr. mūsų išsamų [trikčių diagnostikos vadovą.](https://docs.microsoft.com/sharepoint/support/sites/troubleshooting-guide-for-sites-stopped-at-provisioning)</span><span class="sxs-lookup"><span data-stu-id="6fe99-103">See our detailed [Troubleshooting Guide](https://docs.microsoft.com/sharepoint/support/sites/troubleshooting-guide-for-sites-stopped-at-provisioning).</span></span>

<span data-ttu-id="6fe99-104">Norėdami išspręsti šią problemą, administratorius turi suteikti vartotojams teisę kurti savo mano svetainių svetainę.</span><span class="sxs-lookup"><span data-stu-id="6fe99-104">To resolve this problem, the administrator must grant users the right to create their My Sites site.</span></span> <span data-ttu-id="6fe99-105">Taip yra todėl, kad "OneDrive" verslui puslapis sukuriamas mano svetainėse.</span><span class="sxs-lookup"><span data-stu-id="6fe99-105">This is because the OneDrive for Business page is created on My Sites.</span></span>

<span data-ttu-id="6fe99-106">Norėdami suteikti šią teisę, atlikite šiuos veiksmus:</span><span class="sxs-lookup"><span data-stu-id="6fe99-106">To grant this right, follow these steps:</span></span>

1. <span data-ttu-id="6fe99-107">"SharePoint" administravimo centre spustelėkite **vartotojų profiliai**.</span><span class="sxs-lookup"><span data-stu-id="6fe99-107">In the SharePoint admin center,click **user profiles**.</span></span>

2. <span data-ttu-id="6fe99-108">Sekcijoje  Žmonės spustelėkite **Valdyti vartotojo teises.**</span><span class="sxs-lookup"><span data-stu-id="6fe99-108">In the **People** section, click **Manage User Permissions**.</span></span>

3. <span data-ttu-id="6fe99-109">Įtraukite vartotojų, kuriems reikia teisių kurti savo mano svetaines.</span><span class="sxs-lookup"><span data-stu-id="6fe99-109">Add users who require permissions to create their My Sites site.</span></span> <span data-ttu-id="6fe99-110">Pagal numatytuosius nustatymus šis parametras nustatytas kaip **Visi, išskyrus išorinius vartotojus.**</span><span class="sxs-lookup"><span data-stu-id="6fe99-110">By default, this setting is set to **Everyone except external users**.</span></span>

4. <span data-ttu-id="6fe99-111">Kai įtraukėte vartotoją, vartotojus arba grupę, įsitikinkite, kad pasirinktas įtrauktas vartotojas,  vartotojai arba grupė, slinkite į teisių sekciją, tada pažymėkite žymės langelį šalia Kurti asmeninę svetainę (būtina asmeninei saugyklai, naujienų informacijos santraukoms ir **turiniui)**.</span><span class="sxs-lookup"><span data-stu-id="6fe99-111">After you have added the user, users, or group, make sure that the added user, users, or group is selected, scroll to the **permissions** section, and then select the check box next to **Create Personal Site (required for personal storage, newsfeed, and followed content)**.</span></span>

5. <span data-ttu-id="6fe99-112">Spustelėkite **Gerai**, tada eikite į "OneDrive" puslapį, kad sukurtumėte svetainę.</span><span class="sxs-lookup"><span data-stu-id="6fe99-112">Click **OK**, and then have the user browse to the OneDrive page to create the site.</span></span>
