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
# <a name="upn-sync-disabled"></a>Išjungtas UPN sinchronizavimas

Jei pradėjote sinchronizuoti su "Azure AD" iki kovo 30 d., 2016, vykdykite šią "Azure AD PowerShell" cmdlet, kad galėtumėte įgalinti "UPN Soft Match" tik jūsų organizacijai:
  
 **Set-MsolDirSyncFeature-Feature EnableSoftMatchOnUpn – įjungti $True**
  
UPN Soft Match automatiškai įjungiamas organizacijoms, kurios pradėjo sinchronizuoti "Azure AD" arba po 30 kov, 2016.
  
Jei norite daugiau sužinoti apie tai, kaip įgalinti Soft Match UPN ir kitas sinchronizavimo funkcijas, žiūrėkite " [AZURE AD Connect" sinchronizavimo tarnybos funkcijas](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsyncservice-features).
  

