---
title: Riboti "SharePoint Online" klasikinį režimą
ms.author: pebaum
author: pebaum
ms.date: 3/27/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 6e99da1c-e61d-40ba-855e-1a8f346e42fd
ms.custom:
- "1835"
- "1889"
- "9000225"
ms.openlocfilehash: b58a1c3fc331c739080542917d8945c090ec0d94
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 12/15/2019
ms.locfileid: "40048768"
---
# <a name="restrict-sharepoint-online-to-classic-mode"></a><span data-ttu-id="b4b5a-102">Riboti "SharePoint Online" klasikinį režimą</span><span class="sxs-lookup"><span data-stu-id="b4b5a-102">Restrict SharePoint Online to classic mode</span></span>

<span data-ttu-id="b4b5a-103">Kai kurios organizacijos vis dar reikalauja Klasikinis režimas patirtį.</span><span class="sxs-lookup"><span data-stu-id="b4b5a-103">Some organizations still require the Classic mode experience.</span></span> <span data-ttu-id="b4b5a-104">Nors nėra jokių planų pašalinti klasikinį režimą granuliuoto lygio, tai nebėra įmanoma apriboti visą organizaciją (nuomotojo) Klasikinis režimas sąrašų ir bibliotekų.</span><span class="sxs-lookup"><span data-stu-id="b4b5a-104">While there are no plans to remove classic mode at a granular level, it is no longer possible to restrict an entire organization (tenant) to classic mode for lists and libraries.</span></span>

<span data-ttu-id="b4b5a-105">Administratorius turės šias galimybes valdyti atskirus sąrašus ir bibliotekų Klasikinis režimas naudojant granulių atsisakymo jungikliai, kad mes teikiame šiuos lygius:</span><span class="sxs-lookup"><span data-stu-id="b4b5a-105">The admin will have the following options to manage individual lists and libraries in classic mode using granular opt-out switches that we provide at the following levels:</span></span>

- <span data-ttu-id="b4b5a-106">svetainių rinkinys</span><span class="sxs-lookup"><span data-stu-id="b4b5a-106">site collection</span></span>
- <span data-ttu-id="b4b5a-107">Svetainės</span><span class="sxs-lookup"><span data-stu-id="b4b5a-107">site</span></span>
- <span data-ttu-id="b4b5a-108">Sąrašus</span><span class="sxs-lookup"><span data-stu-id="b4b5a-108">list</span></span>
- <span data-ttu-id="b4b5a-109">Biblioteka</span><span class="sxs-lookup"><span data-stu-id="b4b5a-109">library</span></span>

<span data-ttu-id="b4b5a-110">Be to, sąrašai, kuriuose naudojamos tam tikros funkcijos ir tinkinimai, kurių nepalaiko šiuolaikinė, vis tiek bus automatiškai perjungiami į klasikinį režimą.</span><span class="sxs-lookup"><span data-stu-id="b4b5a-110">Additionally, lists that use certain features and customizations that are not supported by modern will still be automatically switched to classic mode.</span></span>

<span data-ttu-id="b4b5a-111">Pradžia balandis 1, 2019, procesas išjungti nuomininkas lygio atsisakyti šiuolaikinės sąrašą ir bibliotekos pradės ir toliau iki gegužės 31, 2019.</span><span class="sxs-lookup"><span data-stu-id="b4b5a-111">Beginning April 1, 2019, the process to disable the tenant level opt out of modern list and libraries will start and continue through May 31, 2019.</span></span>  <span data-ttu-id="b4b5a-112">Sąrašai ir bibliotekos, kurios yra klasikiniame režime dėl nuomininko atsisakymo, bus automatiškai perkeltos į modernią.</span><span class="sxs-lookup"><span data-stu-id="b4b5a-112">The lists and libraries that are in classic mode as a result of tenant opt-out will automatically be shifted to modern.</span></span>

<span data-ttu-id="b4b5a-113">Jei jums reikia Klasikinis režimas, prašome Peržiūrėti daugiau informacijos [čia](https://techcommunity.microsoft.com/t5/Microsoft-SharePoint-Blog/Delivering-SharePoint-modern-experiences/ba-p/315023) ir PnP PowerShell instrukcija [čia](https://docs.microsoft.com/sharepoint/dev/transform/modernize-userinterface-lists-and-libraries-optout) aprašoma galimybes ir įrankius, kuriuos galite naudoti šiandien naudoti klasikinį režimą patirtį.</span><span class="sxs-lookup"><span data-stu-id="b4b5a-113">If you require classic mode please see more information [here](https://techcommunity.microsoft.com/t5/Microsoft-SharePoint-Blog/Delivering-SharePoint-modern-experiences/ba-p/315023) and PnP Powershell instruction [here](https://docs.microsoft.com/sharepoint/dev/transform/modernize-userinterface-lists-and-libraries-optout) that describes options and tools you can use today to use the classic mode experience.</span></span>
