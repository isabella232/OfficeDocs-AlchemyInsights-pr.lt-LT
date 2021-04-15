---
title: UPN sinchronizavimas išjungtas
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 2a3489fe-c2a8-4e43-96c2-be4b3c5e978c
ms.openlocfilehash: 2b1ba772459091ce1a796884997fe2516d0407eb
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 04/15/2021
ms.locfileid: "51782159"
---
# <a name="upn-sync-disabled"></a>UPN sinchronizavimas išjungtas

Jei pradėjote sinchronizuoti su "Azure AD" iki 2016 m. kovo 30 d., vykdykite šią "Azure AD PowerShell" "cmdlet", kad įgalintumėte UPN minkštą atitikmenį tik jūsų organizacijoje:
  
 **Set-MsolDirSyncFeature -Feature EnableSoftMatchOnUpn -Enable $True**
  
UPN švelnioji atitiktis automatiškai įjungiama organizacijoms, kurios pradėjo sinchronizuoti su "Azure AD" 2016 m. kovo 30 d. arba vėliau.
  
Norėdami sužinoti daugiau apie tai, kaip įgalinti švelnią atitiktį UPN ir kitoms sinchronizavimo funkcijoms, žr. ["Azure AD Connect" sinchronizavimo tarnybos funkcijos](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsyncservice-features).
  

