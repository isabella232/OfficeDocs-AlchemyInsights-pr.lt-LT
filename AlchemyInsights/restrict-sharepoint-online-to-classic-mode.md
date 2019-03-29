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
ms.openlocfilehash: c51e48fe5694f964aef74c2973f774b44415ebb8
ms.sourcegitcommit: 21cfb213183188d32a3743f66db10a8463019965
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 03/28/2019
ms.locfileid: "30956003"
---
# <a name="restrict-sharepoint-online-to-classic-mode"></a><span data-ttu-id="75549-102">Klasikinis būdas apriboti SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="75549-102">Restrict SharePoint Online to classic mode</span></span>

<span data-ttu-id="75549-103">Kai kurios organizacijos yra reikalinga Klasikinis režimas patirtį.</span><span class="sxs-lookup"><span data-stu-id="75549-103">Some organizations still require the Classic mode experience.</span></span> <span data-ttu-id="75549-104">Nors nėra jokių planų pašalinti Klasikinis režimas granuliuotas lygiu, pradeda balandžio 1,2019, jis nebebus galima riboti visą organizacijos (nuomotojo) į klasikinį režimą sąrašuose ir bibliotekose.</span><span class="sxs-lookup"><span data-stu-id="75549-104">While there are no plans to remove classic mode at a granular level, starting April 1,2019, it will no longer be possible to restrict an entire organization (tenant) to classic mode for lists and libraries.</span></span>

<span data-ttu-id="75549-105">Administratorius turi valdyti atskirus sąrašus ir bibliotekas ir klasikinis režimas naudojant granuliuotas atsisakyti jungikliai, kad mes teikiame tokios šių parinkčių:</span><span class="sxs-lookup"><span data-stu-id="75549-105">The admin will have the following options to manage individual lists and libraries in classic mode using granular opt-out switches that we provide at the following levels:</span></span>

- <span data-ttu-id="75549-106">svetainių rinkinio</span><span class="sxs-lookup"><span data-stu-id="75549-106">site collection</span></span>
- <span data-ttu-id="75549-107">svetainė</span><span class="sxs-lookup"><span data-stu-id="75549-107">site</span></span>
- <span data-ttu-id="75549-108">sąrašas</span><span class="sxs-lookup"><span data-stu-id="75549-108">list</span></span>
- <span data-ttu-id="75549-109">biblioteka</span><span class="sxs-lookup"><span data-stu-id="75549-109">library</span></span>

<span data-ttu-id="75549-110">Be to, sąrašus, naudoti tam tikrų funkcijų ir tinkinimus, kad nepalaiko šiuolaikinių bus dar automatiškai perjungiamas į klasikinį režimą.</span><span class="sxs-lookup"><span data-stu-id="75549-110">Additionally, lists that use certain features and customizations that are not supported by modern will still be automatically switched to classic mode.</span></span>

<span data-ttu-id="75549-111">Po balandžio 1 d., sąrašų ir bibliotekų, kurios yra klasikinis režimas dėl nuomininko atsisakymo bus automatiškai valdyti svetainės lygiu ir sąrašo lygį.</span><span class="sxs-lookup"><span data-stu-id="75549-111">After April 1, lists and libraries that are in classic mode as a result of tenant opt-out will automatically be managed at the site level and list level.</span></span>

<span data-ttu-id="75549-112">Jei jums reikalingas Klasikinis režimas rasite daugiau informacijos čia ir PnP "PowerShell" instrukcija čia aprašomos parinktys ir įrankiai galite naudoti šiandien parengti ir nuomininko lygiu atsisakyti balandžio 1 d. panaikinti.</span><span class="sxs-lookup"><span data-stu-id="75549-112">If you require classic mode please see more information here and PnP Powershell instruction here that describes options and tools you can use today to prepare for the removal of the tenant level opt-out on April 1.</span></span>
