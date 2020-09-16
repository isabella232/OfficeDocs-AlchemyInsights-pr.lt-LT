---
title: Išjungtas UPN sinchronizavimas
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 2a3489fe-c2a8-4e43-96c2-be4b3c5e978c
ms.openlocfilehash: 31947d7c491e4116ffdb9baadf286cd4fbb50f2a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47749522"
---
# <a name="upn-sync-disabled"></a><span data-ttu-id="57f0f-102">Išjungtas UPN sinchronizavimas</span><span class="sxs-lookup"><span data-stu-id="57f0f-102">UPN sync disabled</span></span>

<span data-ttu-id="57f0f-103">Jei pradėjote sinchronizuoti su "Azure AD" iki kovo 30 d., 2016, vykdykite šią "Azure AD PowerShell" cmdlet, kad galėtumėte įgalinti "UPN Soft Match" tik jūsų organizacijai:</span><span class="sxs-lookup"><span data-stu-id="57f0f-103">If you started syncing to Azure AD before March 30, 2016, run the following Azure AD PowerShell cmdlet to enable UPN soft match for your organization only:</span></span>
  
 <span data-ttu-id="57f0f-104">**Set-MsolDirSyncFeature-Feature EnableSoftMatchOnUpn – įjungti $True**</span><span class="sxs-lookup"><span data-stu-id="57f0f-104">**Set-MsolDirSyncFeature -Feature EnableSoftMatchOnUpn -Enable $True**</span></span>
  
<span data-ttu-id="57f0f-105">UPN Soft Match automatiškai įjungiamas organizacijoms, kurios pradėjo sinchronizuoti "Azure AD" arba po 30 kov, 2016.</span><span class="sxs-lookup"><span data-stu-id="57f0f-105">UPN soft match is automatically turned on for organizations that started syncing to Azure AD on or after March 30, 2016.</span></span>
  
<span data-ttu-id="57f0f-106">Jei norite daugiau sužinoti apie tai, kaip įgalinti Soft Match UPN ir kitas sinchronizavimo funkcijas, žiūrėkite " [AZURE AD Connect" sinchronizavimo tarnybos funkcijas](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsyncservice-features).</span><span class="sxs-lookup"><span data-stu-id="57f0f-106">To learn more about enabling soft match on UPN and other sync features, please see [Azure AD Connect sync service features](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsyncservice-features).</span></span>
  

