---
title: Grupės kūrimas
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003234"
- "7230"
ms.openlocfilehash: b8cb3f1de991bfe7197607d5e8964a018e31c122
ms.sourcegitcommit: 35e2c122d8a838d98d1f0851c29b16282261580f
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 11/17/2020
ms.locfileid: "49088908"
---
# <a name="create-a-group"></a><span data-ttu-id="ef6a7-102">Grupės kūrimas</span><span class="sxs-lookup"><span data-stu-id="ef6a7-102">Create a group</span></span>

<span data-ttu-id="ef6a7-103">Šioje temoje aprašomi grupės kūrimas.</span><span class="sxs-lookup"><span data-stu-id="ef6a7-103">This topic describes group creation.</span></span>

<span data-ttu-id="ef6a7-104">**Grupės kūrimo teisė**</span><span class="sxs-lookup"><span data-stu-id="ef6a7-104">**Permission to Create a Group**</span></span>

<span data-ttu-id="ef6a7-105">Įsitikinkite, kad turite teisę kurti naują grupę.</span><span class="sxs-lookup"><span data-stu-id="ef6a7-105">Ensure you are authorized to create a new group.</span></span> <span data-ttu-id="ef6a7-106">Visuotinis administratorius gali išjungti grupės kūrimą "Azure" portale arba "Access" skyde.</span><span class="sxs-lookup"><span data-stu-id="ef6a7-106">Global administrators can disable group creation in the Azure portal or Access Panel.</span></span> <span data-ttu-id="ef6a7-107">Jums gali reikėti administratoriaus, kad galėtumėte sukurti jums naują grupę arba suteikti reikiamas teises.</span><span class="sxs-lookup"><span data-stu-id="ef6a7-107">You may need an administrator to create the new group for you, or to give you appropriate permissions.</span></span>

<span data-ttu-id="ef6a7-108">**Grupių kūrimo teisių valdymas**</span><span class="sxs-lookup"><span data-stu-id="ef6a7-108">**Manage Group creation permissions**</span></span>

1. <span data-ttu-id="ef6a7-109">Visuotiniai administratoriai gali valdyti grupių kūrimo teises (dėl su sauga susijusių priežasčių) arba "Office" 365 grupes, sukurtas "Azure" portale arba "Access" srityje, pasirinkdami "vartotojai gali kurti saugos grupes" Azure "portaluose", arba "vartotojai gali kurti" Office 365 "grupes" Azure "portaluose" parinktys " **visose grupėse**  >  **(parametrai)**.</span><span class="sxs-lookup"><span data-stu-id="ef6a7-109">Global administrators can manage group creation permissions (for security-related reasons) or Office 365 groups created in the Azure portal or Access Panel, by choosing "Users can create security groups in Azure portals" or "Users can create Office 365 groups in Azure portals" options in **All groups** > **General (Settings)**.</span></span>
2. <span data-ttu-id="ef6a7-110">Taip pat galite apriboti grupės kūrimą, kad pasirinktumėte grupę vartotojų, jei turite "Azure Active Directory P1 Premium" licenciją.</span><span class="sxs-lookup"><span data-stu-id="ef6a7-110">You can also restrict group creation to select a group of users if you have an Azure Active Directory P1 Premium license.</span></span>

<span data-ttu-id="ef6a7-111">**Pasveikinimo pranešimo išjungimas naujiems "Office 365" grupės nariams**</span><span class="sxs-lookup"><span data-stu-id="ef6a7-111">**Disabling welcome notification for new Office 365 group members**</span></span>

<span data-ttu-id="ef6a7-112">Į "Office 365" grupes įtraukti vartotojai gali būti išjungti, kai "PowerShell" nustato " **Unifiedgroupsveikiemessageenabled** ".</span><span class="sxs-lookup"><span data-stu-id="ef6a7-112">The welcome notification sent to users who are added to Office 365 groups can be disabled by setting **UnifiedGroupWelcomeMessageEnabled** to False in Powershell.</span></span> <span data-ttu-id="ef6a7-113">Sužinokite apie šį parametrą [čia](https://docs.microsoft.com/powershell/module/exchange/set-unifiedgroup?view=exchange-ps&preserve-view=true).</span><span class="sxs-lookup"><span data-stu-id="ef6a7-113">Learn about this setting [here](https://docs.microsoft.com/powershell/module/exchange/set-unifiedgroup?view=exchange-ps&preserve-view=true).</span></span>

