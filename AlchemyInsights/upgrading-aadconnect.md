---
title: "\"932\" \"AADConnect\" naujinimas"
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "932"
- "1300025"
ms.assetid: 8f43f36c-9722-43a4-b0de-c5341c06dac5
ms.openlocfilehash: 5c8ec5d9282c53c655e28f5d38fe36fc3ab005b8
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 09/15/2020
ms.locfileid: "47806047"
---
# <a name="upgrade-azure-ad-connect"></a><span data-ttu-id="e2419-102">"Azure AD Connect" versijos naujinimas</span><span class="sxs-lookup"><span data-stu-id="e2419-102">Upgrade Azure AD Connect</span></span>

<span data-ttu-id="e2419-103">Pagal numatytuosius "Azure AD Connect" įgalintas automatinis versijos naujinimas, kuris padeda užtikrinti, kad naudojate naujausią versiją.</span><span class="sxs-lookup"><span data-stu-id="e2419-103">By default, automatic upgrade is enabled for Azure AD Connect, which helps to ensure you're running the latest version.</span></span> <span data-ttu-id="e2419-104">Norėdami patikrinti automatinio versijos naujinimo parametrus, naudokite "Azure AD PowerShell" cmdlet **get-ADSyncAutoUpgrade** .</span><span class="sxs-lookup"><span data-stu-id="e2419-104">To verify the automatic upgrade settings, use the **Get-ADSyncAutoUpgrade** cmdlet in Azure AD PowerShell.</span></span> <span data-ttu-id="e2419-105">Cmdlet pateiks vieną iš šių reikšmių:</span><span class="sxs-lookup"><span data-stu-id="e2419-105">The cmdlet will return one of following values:</span></span>

- <span data-ttu-id="e2419-106">**Įgalinta**: automatinis versijos naujinimas įgalintas.</span><span class="sxs-lookup"><span data-stu-id="e2419-106">**Enabled**: Automatic upgrade is enabled.</span></span>

- <span data-ttu-id="e2419-107">**Išjungta**: automatinis versijos naujinimas išjungtas.</span><span class="sxs-lookup"><span data-stu-id="e2419-107">**Disabled**: Automatic upgrade is disabled.</span></span>

- <span data-ttu-id="e2419-108">**Sustabdyta**: sistema nebeturi teisės gauti automatinius naujinius.</span><span class="sxs-lookup"><span data-stu-id="e2419-108">**Suspended**: The system is no longer eligible to receive automatic upgrades.</span></span> <span data-ttu-id="e2419-109">Negalite sukonfigūruoti šios reikšmės; ją nustato sistema.</span><span class="sxs-lookup"><span data-stu-id="e2419-109">You can't configure this value; it's set by the system.</span></span>

<span data-ttu-id="e2419-110">Daugiau informacijos ieškokite [Automatinis versijos naujinimas](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade).</span><span class="sxs-lookup"><span data-stu-id="e2419-110">For more information, see [Automatic upgrade](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade).</span></span>

<span data-ttu-id="e2419-111">Norėdami atsisiųsti naujausią "Azure AD Connect" versiją, eikite į [https://www.microsoft.com/download/details.aspx?id=47594](https://www.microsoft.com/download/details.aspx?id=47594) .</span><span class="sxs-lookup"><span data-stu-id="e2419-111">To download the latest version of Azure AD Connect, go to [https://www.microsoft.com/download/details.aspx?id=47594](https://www.microsoft.com/download/details.aspx?id=47594).</span></span>
