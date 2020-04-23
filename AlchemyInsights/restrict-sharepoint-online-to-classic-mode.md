---
title: Apriboti "SharePoint Online" iki klasikinio režimo
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 6e99da1c-e61d-40ba-855e-1a8f346e42fd
ms.custom:
- "1835"
- "1889"
- "9000225"
ms.openlocfilehash: c5ea5d264b62e4c349623bd431776207b38da470
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 04/22/2020
ms.locfileid: "43742477"
---
# <a name="restrict-sharepoint-online-to-classic-mode"></a><span data-ttu-id="cacba-102">Apriboti "SharePoint Online" iki klasikinio režimo</span><span class="sxs-lookup"><span data-stu-id="cacba-102">Restrict SharePoint Online to classic mode</span></span>

<span data-ttu-id="cacba-103">Kai kurioms organizacijoms vis tiek reikia klasikinio režimo naudojimo.</span><span class="sxs-lookup"><span data-stu-id="cacba-103">Some organizations still require the Classic mode experience.</span></span> <span data-ttu-id="cacba-104">Nors nėra planų pašalinti klasikinį režimą granuliuoto lygio, nebegalima apriboti visos organizacijos (nuomotojo) klasikinio režimo sąrašuose ir bibliotekose.</span><span class="sxs-lookup"><span data-stu-id="cacba-104">While there are no plans to remove classic mode at a granular level, it is no longer possible to restrict an entire organization (tenant) to classic mode for lists and libraries.</span></span>

<span data-ttu-id="cacba-105">Administratorius turės šias parinktis, kaip valdyti atskirus sąrašus ir bibliotekas klasikiniu režimu, naudojant detalus atsisakymo jungiklius, kuriuos pateikiame šiais lygiais:</span><span class="sxs-lookup"><span data-stu-id="cacba-105">The admin will have the following options to manage individual lists and libraries in classic mode using granular opt-out switches that we provide at the following levels:</span></span>

- <span data-ttu-id="cacba-106">svetainių rinkinys</span><span class="sxs-lookup"><span data-stu-id="cacba-106">site collection</span></span>
- <span data-ttu-id="cacba-107">Svetainės</span><span class="sxs-lookup"><span data-stu-id="cacba-107">site</span></span>
- <span data-ttu-id="cacba-108">Sąrašus</span><span class="sxs-lookup"><span data-stu-id="cacba-108">list</span></span>
- <span data-ttu-id="cacba-109">Biblioteka</span><span class="sxs-lookup"><span data-stu-id="cacba-109">library</span></span>

<span data-ttu-id="cacba-110">Be to, sąrašai, kuriuose naudojamos tam tikros funkcijos ir tinkinimai, kurių nepalaiko modernus, vis tiek bus automatiškai perjungiami į klasikinį režimą.</span><span class="sxs-lookup"><span data-stu-id="cacba-110">Additionally, lists that use certain features and customizations that are not supported by modern will still be automatically switched to classic mode.</span></span>

<span data-ttu-id="cacba-111">Nuo 2019 m. balandžio 1 d. bus pradėtas ir tęsiamas procesas, kuriuo siekiama išjungti nuomotojo lygio atsisakymą iš šiuolaikinio sąrašo ir bibliotekų iki 2019 m. gegužės 31 d.</span><span class="sxs-lookup"><span data-stu-id="cacba-111">Beginning April 1, 2019, the process to disable the tenant level opt out of modern list and libraries will start and continue through May 31, 2019.</span></span>  <span data-ttu-id="cacba-112">Sąrašai ir bibliotekos, kurios yra klasikinio režimo dėl nuomotojo atsisakymo rezultatas bus automatiškai perkeltas į modernią.</span><span class="sxs-lookup"><span data-stu-id="cacba-112">The lists and libraries that are in classic mode as a result of tenant opt-out will automatically be shifted to modern.</span></span>

<span data-ttu-id="cacba-113">Jei jums reikia klasikinio režimo, čia rasite daugiau [informacijos](https://techcommunity.microsoft.com/t5/Microsoft-SharePoint-Blog/Delivering-SharePoint-modern-experiences/ba-p/315023) ir "PnP PowerShell" [instrukciją,](https://docs.microsoft.com/sharepoint/dev/transform/modernize-userinterface-lists-and-libraries-optout) kurioje aprašomos parinktys ir įrankiai, kuriuos galite naudoti šiandien, kad galėtumėte naudoti klasikinį režimo patirtį.</span><span class="sxs-lookup"><span data-stu-id="cacba-113">If you require classic mode please see more information [here](https://techcommunity.microsoft.com/t5/Microsoft-SharePoint-Blog/Delivering-SharePoint-modern-experiences/ba-p/315023) and PnP Powershell instruction [here](https://docs.microsoft.com/sharepoint/dev/transform/modernize-userinterface-lists-and-libraries-optout) that describes options and tools you can use today to use the classic mode experience.</span></span>
