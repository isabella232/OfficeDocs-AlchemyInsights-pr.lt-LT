---
title: Hibridinio „Azure AD“ prisijungimo gedimų šalinimas
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/06/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6162"
- "6158"
- "9003244"
- "9003246"
ms.openlocfilehash: 18d0ce6bdf3df96e07cc6607b9ae6142d548dabe
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: HT
ms.contentlocale: lt-LT
ms.lasthandoff: 03/29/2021
ms.locfileid: "51401915"
---
# <a name="troubleshoot-hybrid-azure-ad-join"></a>Hibridinio „Azure AD“ prisijungimo gedimų šalinimas

Labai rekomenduojama įsitikinti, kad įrenginys gali pasiekti įrenginio registracijos galinius punktus pagal sistemos paskyrą naudodamas [„Tikrinti įrenginio registracijos ryšį“](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/) scenarijų.

1. Jei įrenginių registraciją nustatote pirmą kartą, būtinai peržiūrėkite Į[vadas į įrenginių valdymą „Azure Active Directory“](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/), kad sužinotumėte, kaip pasiekti, kad įrenginiai būtų valdomi „Azure AD“.
1. Jei tiesiogiai registruojate įrenginius į „Azure AD“ ir registruojate juos į „Intune“, įsitikinkite, kad [sukonfigūravote „Intune“](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment?WT.mc_id=Portal-Microsoft_Azure_Support) ir pirmiausia turite [licencijavimą](https://docs.microsoft.com/mem/intune/fundamentals/licenses-assign?WT.mc_id=Portal-Microsoft_Azure_Support).
1. Įsitikinkite, kad esate įgaliotas atlikti operacijas „Azure AD“ ir vietiniame AD. Tik visuotinis „Azure AD“ administratorius gali valdyti įrenginių registravimo parametrus. Be to, jei vietiniame „Active Directory“ nustatote automatines registracijas, turėsite būti „Active Directory“ ir „AD FS“ (jei taikoma) administratorius.

Norėdami gauti daugiau informacijos apie galimas hibridinio prisijungimo problemas, žr. [„Hibridinio prisijungimo gedimų šalinimas“](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-hybrid-join-windows-current), kad nustatytumėte sujungtą hibridinį „Azure AD“ ir valdytumėte įrenginius naudojant „Azure ad“ portalą, žr. [Nustatyti hibridinius „Azure AD“ sujungtus (vietinius, prijungtus prie domeno) įrenginius](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan?WT.mc_id=Portal-Microsoft_Azure_Support) ir [Valdyti įrenginius „Azure“ portale](https://docs.microsoft.com/azure/active-directory/devices/device-management-azure-portal?WT.mc_id=Portal-Microsoft_Azure_Support).

Norėdami išspręsti bendrąsias hibridinio „Azure Active Directory“ (AD) prisijungimo problemas, žr. [Hibridinio „Azure AD“ prisijungimo DUK](https://docs.microsoft.com/azure/active-directory/devices/faq#hybrid-azure-ad-join-faq).
