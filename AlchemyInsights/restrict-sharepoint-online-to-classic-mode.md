---
title: Klasikinis būdas apriboti SharePoint Online
ms.author: kirks
author: Techwriter40
ms.date: 3/27/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 6e99da1c-e61d-40ba-855e-1a8f346e42fd
ms.openlocfilehash: 76f0b5ed67d3220559d25dfd72c7535181a4513b
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 06/07/2019
ms.locfileid: "34761767"
---
# <a name="restrict-sharepoint-online-to-classic-mode"></a><span data-ttu-id="a1e5c-102">Klasikinis būdas apriboti SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="a1e5c-102">Restrict SharePoint Online to classic mode</span></span>

<span data-ttu-id="a1e5c-103">Kai kurios organizacijos yra reikalinga Klasikinis režimas patirtį.</span><span class="sxs-lookup"><span data-stu-id="a1e5c-103">Some organizations still require the Classic mode experience.</span></span> <span data-ttu-id="a1e5c-104">Nors nėra jokių planų pašalinti Klasikinis režimas granuliuotas lygiu, tai jau galima riboti visą organizacijos (nuomotojo) į klasikinį režimą sąrašų ir bibliotekų.</span><span class="sxs-lookup"><span data-stu-id="a1e5c-104">While there are no plans to remove classic mode at a granular level, it is no longer possible to restrict an entire organization (tenant) to classic mode for lists and libraries.</span></span>

<span data-ttu-id="a1e5c-105">Administratorius turi valdyti atskirus sąrašus ir bibliotekas ir klasikinis režimas naudojant granuliuotas atsisakyti jungikliai, kad mes teikiame tokios šių parinkčių:</span><span class="sxs-lookup"><span data-stu-id="a1e5c-105">The admin will have the following options to manage individual lists and libraries in classic mode using granular opt-out switches that we provide at the following levels:</span></span>

- <span data-ttu-id="a1e5c-106">svetainių rinkinio</span><span class="sxs-lookup"><span data-stu-id="a1e5c-106">site collection</span></span>
- <span data-ttu-id="a1e5c-107">svetainė</span><span class="sxs-lookup"><span data-stu-id="a1e5c-107">site</span></span>
- <span data-ttu-id="a1e5c-108">sąrašas</span><span class="sxs-lookup"><span data-stu-id="a1e5c-108">list</span></span>
- <span data-ttu-id="a1e5c-109">biblioteka</span><span class="sxs-lookup"><span data-stu-id="a1e5c-109">library</span></span>

<span data-ttu-id="a1e5c-110">Be to, sąrašus, naudoti tam tikrų funkcijų ir tinkinimus, kad nepalaiko šiuolaikinių bus dar automatiškai perjungiamas į klasikinį režimą.</span><span class="sxs-lookup"><span data-stu-id="a1e5c-110">Additionally, lists that use certain features and customizations that are not supported by modern will still be automatically switched to classic mode.</span></span>

<span data-ttu-id="a1e5c-111">Pradžia balandžio 1, 2019, procesas išjungti nuomininko lygiu atsisakyti modernus sąrašo ir bibliotekos bus pradėti ir tęsiasi iki 2019 m. gegužės 31.</span><span class="sxs-lookup"><span data-stu-id="a1e5c-111">Beginning April 1, 2019, the process to disable the tenant level opt out of modern list and libraries will start and continue through May 31, 2019.</span></span>  <span data-ttu-id="a1e5c-112">Sąrašų ir bibliotekų, kurios yra klasikinis režimas dėl nuomininko atsisakymo bus automatiškai perkeltos į šiuolaikinės.</span><span class="sxs-lookup"><span data-stu-id="a1e5c-112">The lists and libraries that are in classic mode as a result of tenant opt-out will automatically be shifted to modern.</span></span>

<span data-ttu-id="a1e5c-113">Jei jums reikalingas Klasikinis režimas rasite daugiau informacijos [čia](https://techcommunity.microsoft.com/t5/Microsoft-SharePoint-Blog/Delivering-SharePoint-modern-experiences/ba-p/315023) ir PnP "PowerShell" instrukcija [čia](https://docs.microsoft.com/sharepoint/dev/transform/modernize-userinterface-lists-and-libraries-optout) aprašytą galimybės ir įrankius, galite naudoti šiandien į klasikinį režimą patirtį.</span><span class="sxs-lookup"><span data-stu-id="a1e5c-113">If you require classic mode please see more information [here](https://techcommunity.microsoft.com/t5/Microsoft-SharePoint-Blog/Delivering-SharePoint-modern-experiences/ba-p/315023) and PnP Powershell instruction [here](https://docs.microsoft.com/sharepoint/dev/transform/modernize-userinterface-lists-and-libraries-optout) that describes options and tools you can use today to use the classic mode experience.</span></span>
