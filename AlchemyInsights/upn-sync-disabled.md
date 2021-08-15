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
ms.openlocfilehash: fc163fae4d348d7c7cf117bd457f999b42f96bec7c1eb9aa1435e346131d06de
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54038120"
---
# <a name="upn-sync-disabled"></a>UPN sinchronizavimas išjungtas

Jei pradėjote sinchronizuoti su "Azure AD" iki 2016 m. kovo 30 d., vykdykite šią "Azure AD PowerShell" "cmdlet", kad įgalintumėte UPN minkštą atitikmenį tik jūsų organizacijoje:
  
 **Set-MsolDirSyncFeature -Feature EnableSoftMatchOnUpn -Enable $True**
  
UPN švelnioji atitiktis automatiškai įjungiama organizacijoms, kurios pradėjo sinchronizuoti su "Azure AD" 2016 m. kovo 30 d. arba vėliau.
  
Norėdami sužinoti daugiau, kaip įgalinti švelnią atitiktį UPN ir kitoms sinchronizavimo funkcijoms, žr. ["Azure AD Prisijungimas sinchronizavimo tarnybos funkcijos.](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsyncservice-features)
  

