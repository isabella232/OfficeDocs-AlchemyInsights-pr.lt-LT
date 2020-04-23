---
title: 932 AADConnect versijos naujinimas
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "932"
- "1300025"
ms.assetid: 8f43f36c-9722-43a4-b0de-c5341c06dac5
ms.openlocfilehash: fcc5fddb5cfd15407d0533449035317d187931ed
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 04/22/2020
ms.locfileid: "43766501"
---
# <a name="upgrade-azure-ad-connect"></a><span data-ttu-id="79983-102">Atnaujinkite Azure AD Prisijungti</span><span class="sxs-lookup"><span data-stu-id="79983-102">Upgrade Azure AD Connect</span></span>

<span data-ttu-id="79983-103">Pagal numatytuosius nustatymus automatinis naujinimas įgalintas "Azure AD Connect", kuris padeda užtikrinti, kad naudojate naujausią versiją.</span><span class="sxs-lookup"><span data-stu-id="79983-103">By default, automatic upgrade is enabled for Azure AD Connect, which helps to ensure you're running the latest version.</span></span> <span data-ttu-id="79983-104">Norėdami patikrinti automatinio naujinimo parametrus, naudokite **Get-ADSyncAutoUpgrade** cmdlet Azure AD PowerShell.</span><span class="sxs-lookup"><span data-stu-id="79983-104">To verify the automatic upgrade settings, use the **Get-ADSyncAutoUpgrade** cmdlet in Azure AD PowerShell.</span></span> <span data-ttu-id="79983-105">Cmdlet grąžins vieną iš šių reikšmių:</span><span class="sxs-lookup"><span data-stu-id="79983-105">The cmdlet will return one of following values:</span></span>

- <span data-ttu-id="79983-106">**Įgalinta:** automatinis naujinimas įgalintas.</span><span class="sxs-lookup"><span data-stu-id="79983-106">**Enabled**: Automatic upgrade is enabled.</span></span>

- <span data-ttu-id="79983-107">**Išjungta:** automatinis naujinimas išjungtas.</span><span class="sxs-lookup"><span data-stu-id="79983-107">**Disabled**: Automatic upgrade is disabled.</span></span>

- <span data-ttu-id="79983-108">**Sustabdyta**: sistema nebeturi teisės gauti automatinių naujinimų.</span><span class="sxs-lookup"><span data-stu-id="79983-108">**Suspended**: The system is no longer eligible to receive automatic upgrades.</span></span> <span data-ttu-id="79983-109">Negalite konfigūruoti šios reikšmės; jis nustatytas sistemos.</span><span class="sxs-lookup"><span data-stu-id="79983-109">You can't configure this value; it's set by the system.</span></span>

<span data-ttu-id="79983-110">Daugiau informacijos ieškokite [Automatic upgrade](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade).</span><span class="sxs-lookup"><span data-stu-id="79983-110">For more information, see [Automatic upgrade](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade).</span></span>

<span data-ttu-id="79983-111">Norėdami atsisiųsti naujausią Azure AD [https://www.microsoft.com/download/details.aspx?id=47594](https://www.microsoft.com/download/details.aspx?id=47594)Connect versiją, eikite į .</span><span class="sxs-lookup"><span data-stu-id="79983-111">To download the latest version of Azure AD Connect, go to [https://www.microsoft.com/download/details.aspx?id=47594](https://www.microsoft.com/download/details.aspx?id=47594).</span></span>
