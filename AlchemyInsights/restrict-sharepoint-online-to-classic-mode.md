---
title: "\"SharePoint Online\" apribojimas klasikinėje režimu"
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 6e99da1c-e61d-40ba-855e-1a8f346e42fd
ms.custom:
- "1835"
- "1889"
- "9000225"
ms.openlocfilehash: 1887bf64df98bf90a1902250633d5774178dfa2f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47751430"
---
# <a name="restrict-sharepoint-online-to-classic-mode"></a><span data-ttu-id="0a5b0-102">"SharePoint Online" apribojimas klasikinėje režimu</span><span class="sxs-lookup"><span data-stu-id="0a5b0-102">Restrict SharePoint Online to classic mode</span></span>

<span data-ttu-id="0a5b0-103">Kai kurioms organizacijoms reikia klasikinio režimo naudojimo patirties.</span><span class="sxs-lookup"><span data-stu-id="0a5b0-103">Some organizations still require the Classic mode experience.</span></span> <span data-ttu-id="0a5b0-104">Nors nėra planų pašalinti klasikinį režimą granuliuoto lygio, nebeįmanoma apriboti visos organizacijos (nuomotojo) iki klasikinio režimo sąrašams ir bibliotekoms.</span><span class="sxs-lookup"><span data-stu-id="0a5b0-104">While there are no plans to remove classic mode at a granular level, it is no longer possible to restrict an entire organization (tenant) to classic mode for lists and libraries.</span></span>

<span data-ttu-id="0a5b0-105">Administratorius turės šias parinktis, kad galėtų valdyti atskirus sąrašus ir bibliotekas klasikiniame režime naudodami granuliuoto atsisakymo jungiklius, kuriuos teikiame šiais lygiais:</span><span class="sxs-lookup"><span data-stu-id="0a5b0-105">The admin will have the following options to manage individual lists and libraries in classic mode using granular opt-out switches that we provide at the following levels:</span></span>

- <span data-ttu-id="0a5b0-106">svetainių rinkinys</span><span class="sxs-lookup"><span data-stu-id="0a5b0-106">site collection</span></span>
- <span data-ttu-id="0a5b0-107">svetainės</span><span class="sxs-lookup"><span data-stu-id="0a5b0-107">site</span></span>
- <span data-ttu-id="0a5b0-108">sąrašus</span><span class="sxs-lookup"><span data-stu-id="0a5b0-108">list</span></span>
- <span data-ttu-id="0a5b0-109">bibliotekos</span><span class="sxs-lookup"><span data-stu-id="0a5b0-109">library</span></span>

<span data-ttu-id="0a5b0-110">Be to, sąrašai, kuriuose naudojamos tam tikros funkcijos ir tinkinimai, nepalaikomi šiuolaikiniais, vis tiek bus automatiškai perjungti į klasikinį režimą.</span><span class="sxs-lookup"><span data-stu-id="0a5b0-110">Additionally, lists that use certain features and customizations that are not supported by modern will still be automatically switched to classic mode.</span></span>

<span data-ttu-id="0a5b0-111">Nuo balandžio 1 d., 2019, procesas išjungti nuomotojo lygį atsisakyti modernaus sąrašo ir bibliotekų pradės ir tęsis iki gegužės 31 d., 2019.</span><span class="sxs-lookup"><span data-stu-id="0a5b0-111">Beginning April 1, 2019, the process to disable the tenant level opt out of modern list and libraries will start and continue through May 31, 2019.</span></span>  <span data-ttu-id="0a5b0-112">Sąrašai ir bibliotekos, kurios yra klasikiniame režime dėl nuomotojo atsisakymo, bus automatiškai perkeltos į šiuolaikinės.</span><span class="sxs-lookup"><span data-stu-id="0a5b0-112">The lists and libraries that are in classic mode as a result of tenant opt-out will automatically be shifted to modern.</span></span>

<span data-ttu-id="0a5b0-113">Jei jums reikia klasikinio režimo, daugiau informacijos rasite [čia](https://techcommunity.microsoft.com/t5/Microsoft-SharePoint-Blog/Delivering-SharePoint-modern-experiences/ba-p/315023) ir PnP "PowerShell" instrukcija [čia](https://docs.microsoft.com/sharepoint/dev/transform/modernize-userinterface-lists-and-libraries-optout) aprašoma parinktis ir įrankius, kuriuos galite naudoti šiandien, kad galėtumėte naudoti klasikinio režimo funkcijas.</span><span class="sxs-lookup"><span data-stu-id="0a5b0-113">If you require classic mode please see more information [here](https://techcommunity.microsoft.com/t5/Microsoft-SharePoint-Blog/Delivering-SharePoint-modern-experiences/ba-p/315023) and PnP Powershell instruction [here](https://docs.microsoft.com/sharepoint/dev/transform/modernize-userinterface-lists-and-libraries-optout) that describes options and tools you can use today to use the classic mode experience.</span></span>
