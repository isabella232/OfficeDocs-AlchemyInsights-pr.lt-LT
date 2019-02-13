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
ms.custom: Adm_O365
ms.assetid: 2a3489fe-c2a8-4e43-96c2-be4b3c5e978c
ms.openlocfilehash: 983796ce8fb7e8b52c0ce31aa13597b53cc9e038
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 02/12/2019
ms.locfileid: "29921716"
---
# <a name="upn-sync-disabled"></a>Išjungti UPN sinchronizavimo

Jei pradėjote sinchronizavimą su Azure AD iki 2016 kovo 30 vykdyti šį Azure AD PowerShell cmdlet, kad UPN minkštas tinka jūsų organizacijai tik:
  
 **Rinkinys-MsolDirSyncFeature-EnableSoftMatchOnUpn funkcija-leidžia $True**
  
UPN minkštas rungtynės įjungiamas automatiškai, organizacijose, kuriose pradėti sinchronizavimą su Azure AD arba po 2016 m. kovo 30 d.
  
Norėdami sužinoti daugiau apie įgalinimą minkštas rungtynės UPN ir kitus sinchronizavimo funkcijos, prašome peržiūrėti [Azure AD Connect sinchronizavimo tarnybos funkcijas](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsyncservice-features).
  

