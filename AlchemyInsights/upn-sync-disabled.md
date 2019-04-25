---
title: Išjungti UPN sinchronizavimo
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 3/20/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 2a3489fe-c2a8-4e43-96c2-be4b3c5e978c
ms.openlocfilehash: 2a03ac64d92c07b523b015850251b33c58bb76f8
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 04/23/2019
ms.locfileid: "32423561"
---
# <a name="upn-sync-disabled"></a><span data-ttu-id="0a88e-102">Išjungti UPN sinchronizavimo</span><span class="sxs-lookup"><span data-stu-id="0a88e-102">UPN sync disabled</span></span>

<span data-ttu-id="0a88e-103">Jei pradėjote sinchronizavimą su Azure AD iki 2016 kovo 30 vykdyti šį Azure AD PowerShell cmdlet, kad UPN minkštas tinka jūsų organizacijai tik:</span><span class="sxs-lookup"><span data-stu-id="0a88e-103">If you started syncing to Azure AD before March 30, 2016, run the following Azure AD PowerShell cmdlet to enable UPN soft match for your organization only:</span></span>
  
 <span data-ttu-id="0a88e-104">**Rinkinys-MsolDirSyncFeature-EnableSoftMatchOnUpn funkcija-leidžia $True**</span><span class="sxs-lookup"><span data-stu-id="0a88e-104">**Set-MsolDirSyncFeature -Feature EnableSoftMatchOnUpn -Enable $True**</span></span>
  
<span data-ttu-id="0a88e-105">UPN minkštas rungtynės įjungiamas automatiškai, organizacijose, kuriose pradėti sinchronizavimą su Azure AD arba po 2016 m. kovo 30 d.</span><span class="sxs-lookup"><span data-stu-id="0a88e-105">UPN soft match is automatically turned on for organizations that started syncing to Azure AD on or after March 30, 2016.</span></span>
  
<span data-ttu-id="0a88e-106">Norėdami sužinoti daugiau apie įgalinimą minkštas rungtynės UPN ir kitus sinchronizavimo funkcijos, prašome peržiūrėti [Azure AD Connect sinchronizavimo tarnybos funkcijas](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsyncservice-features).</span><span class="sxs-lookup"><span data-stu-id="0a88e-106">To learn more about enabling soft match on UPN and other sync features, please see [Azure AD Connect sync service features](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsyncservice-features).</span></span>
  

