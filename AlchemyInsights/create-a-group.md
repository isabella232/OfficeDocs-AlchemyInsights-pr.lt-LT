---
title: Grupės kūrimas
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
- "9003234"
- "7230"
ms.openlocfilehash: ec74b7c098d302d3bdeb5a412fad41efe7b82b98
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 04/15/2021
ms.locfileid: "51816364"
---
# <a name="create-a-group"></a><span data-ttu-id="331a6-102">Grupės kūrimas</span><span class="sxs-lookup"><span data-stu-id="331a6-102">Create a group</span></span>

<span data-ttu-id="331a6-103">Šioje temoje aprašomas grupės kūrimas.</span><span class="sxs-lookup"><span data-stu-id="331a6-103">This topic describes group creation.</span></span>

<span data-ttu-id="331a6-104">**Teisė kurti grupę**</span><span class="sxs-lookup"><span data-stu-id="331a6-104">**Permission to Create a Group**</span></span>

<span data-ttu-id="331a6-105">Įsitikinkite, kad turite teisę kurti naują grupę.</span><span class="sxs-lookup"><span data-stu-id="331a6-105">Ensure you are authorized to create a new group.</span></span> <span data-ttu-id="331a6-106">Visuotiniai administratoriai gali išjungti grupės kūrimą "Azure" portale arba "Access" skyde.</span><span class="sxs-lookup"><span data-stu-id="331a6-106">Global administrators can disable group creation in the Azure portal or Access Panel.</span></span> <span data-ttu-id="331a6-107">Jums gali tekti administratoriaus sukurti naują grupę arba suteikti jums atitinkamas teises.</span><span class="sxs-lookup"><span data-stu-id="331a6-107">You may need an administrator to create the new group for you, or to give you appropriate permissions.</span></span>

<span data-ttu-id="331a6-108">**Grupės kūrimo teisių valdymas**</span><span class="sxs-lookup"><span data-stu-id="331a6-108">**Manage Group creation permissions**</span></span>

1. <span data-ttu-id="331a6-109">Visuotiniai administratoriai gali valdyti grupės kūrimo teises (dėl su sauga susijusių priežasčių) arba "Office 365" grupes, sukurtas "Azure" portale arba "Access" skyde, pasirinkdami "Vartotojai gali kurti saugos grupes "Azure" portaluose" arba "Vartotojai gali kurti "Office 365" grupes "Azure" portaluose" parinktys dalyje **Visos grupės**  >  **Bendra (Parametrai)**.</span><span class="sxs-lookup"><span data-stu-id="331a6-109">Global administrators can manage group creation permissions (for security-related reasons) or Office 365 groups created in the Azure portal or Access Panel, by choosing "Users can create security groups in Azure portals" or "Users can create Office 365 groups in Azure portals" options in **All groups** > **General (Settings)**.</span></span>
2. <span data-ttu-id="331a6-110">Taip pat galite apriboti grupės kūrimą, kad pasirinktumėte vartotojų grupę, jei turite "Azure Active Directory P1 Premium" licenciją.</span><span class="sxs-lookup"><span data-stu-id="331a6-110">You can also restrict group creation to select a group of users if you have an Azure Active Directory P1 Premium license.</span></span>

<span data-ttu-id="331a6-111">**Naujų "Office 365" grupės narių pasveikinimo pranešimo išjungimas**</span><span class="sxs-lookup"><span data-stu-id="331a6-111">**Disabling welcome notification for new Office 365 group members**</span></span>

<span data-ttu-id="331a6-112">Pasveikinimo pranešimą, išsiųstą vartotojams, įtrauktiems į "Office 365" grupes, galima išjungti "PowerShell" nustačius **UnifiedGroupWelcomeMessageEnabled** kaip False.</span><span class="sxs-lookup"><span data-stu-id="331a6-112">The welcome notification sent to users who are added to Office 365 groups can be disabled by setting **UnifiedGroupWelcomeMessageEnabled** to False in Powershell.</span></span> <span data-ttu-id="331a6-113">Sužinokite apie šį parametrą [čia](https://docs.microsoft.com/powershell/module/exchange/set-unifiedgroup?view=exchange-ps&preserve-view=true).</span><span class="sxs-lookup"><span data-stu-id="331a6-113">Learn about this setting [here](https://docs.microsoft.com/powershell/module/exchange/set-unifiedgroup?view=exchange-ps&preserve-view=true).</span></span>

