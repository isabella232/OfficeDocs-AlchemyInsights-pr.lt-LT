---
title: 646 kaip sukonfigūruoti AADConnect
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 6/8/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 599698ac-6709-477a-a66f-169b3165064e
ms.openlocfilehash: e4ba295cd0661c3454180dd6a15895123840389e
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 01/15/2019
ms.locfileid: "28301373"
---
# <a name="configure-sync-features"></a><span data-ttu-id="99e65-102">Konfigūruoti sinchronizavimo funkcijos</span><span class="sxs-lookup"><span data-stu-id="99e65-102">Configure sync features</span></span>

<span data-ttu-id="99e65-p101">Žydros AD jungtis yra kelios funkcijos, yra įjungta pagal numatytuosius nustatymus, arba, kad galite įgalinti vėliau. Kai kurios funkcijos reikalauja papildomos konfigūracijos konkrečių aplinkoje.</span><span class="sxs-lookup"><span data-stu-id="99e65-p101">Azure AD Connect includes several features that are enabled by default, or that you can enable later. Some features require additional configuration in specific environments.</span></span>
  
- <span data-ttu-id="99e65-p102">[Filtravimas](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-configure-filtering) ribas objektai yra sinchronizuoti su Azure AD. Iš numatytasis, visi vartotojai, kontaktus, grupes ir "Windows 10" sinchronizuojami kompiuterių sąskaitos. Jūs galite įtraukti arba pašalinti objektus, domenai, organizaciniai vienetai ar kiti atributai.</span><span class="sxs-lookup"><span data-stu-id="99e65-p102">[Filtering](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-configure-filtering) limits the objects are synchronized to Azure AD. By default, all users, contacts, groups, and Windows 10 computer accounts are synchronized. You can include or exclude objects based on domains, OUs, or other attributes.</span></span> 
    
- <span data-ttu-id="99e65-p103">[Slaptažodis maiša sinchronizavimas](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-implement-password-hash-synchronization) sinchronizuoti slaptažodį maišos iš vietinės Active Directory su Azure AD. Tokiu būdu slapta˛od˛io valdymo vienoje vietoje, bet naudoti tą patį slaptažodį, tiek vietiniame ir debesų kompiuterijos aplinkose. Todėl, kad Active Directory yra patikimas šaltinis, galite naudoti savo slaptažodžio strategijų.</span><span class="sxs-lookup"><span data-stu-id="99e65-p103">[Password hash syncronization](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-implement-password-hash-synchronization) synchronizes the password hash from the on-premises Active Directory to Azure AD. This allows password management in one location, but use of the same password in both on-premises and cloud environments. Because Active Directory is the authoritative source, you can use your own password policies.</span></span> 
    
- <span data-ttu-id="99e65-111">[Savitarnos slaptažodžio nustatymo iš naujo (SSPR)](https://docs.microsoft.com/azure/active-directory/authentication/quickstart-sspr) leidžia vartotojams iš naujo nustatyti savo slaptažodžius debesis dar taikant vietinę slaptažodžių strategija.</span><span class="sxs-lookup"><span data-stu-id="99e65-111">[Self-service password reset (SSPR)](https://docs.microsoft.com/azure/active-directory/authentication/quickstart-sspr) allows users to reset their own passwords in the cloud while still applying your on-premises password policy.</span></span> 
    
- <span data-ttu-id="99e65-112">[Įrenginio write-back](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-device-writeback) leidžia registruoti įrenginiai Azure AD įrašomi atgal į vietinės Active Directory, jie gali būti naudojami dėl sąlygine prieiga.</span><span class="sxs-lookup"><span data-stu-id="99e65-112">[Device writeback](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-device-writeback) allows registered devices in Azure AD to be written back to the on-premises Active Directory so they can be used for conditional access.</span></span> 
    
- <span data-ttu-id="99e65-p104">[Išvengti atsitiktinio panaikina](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-feature-prevent-accidental-deletes) yra įjungta pagal nutylėjimą padeda išvengti per daug vienu metu objektas naikinimus (daugiau kaip 500 objektų už sinchronizavimo). Galite pakeisti šį nustatymą, kad atitiktų jūsų organizacijos poreikius.</span><span class="sxs-lookup"><span data-stu-id="99e65-p104">[Prevent accidental deletes](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-feature-prevent-accidental-deletes) is enabled by default to help prevent too many simultaneous object deletions (more than 500 objects per synchronization). You can change this setting to meet the needs of your organization.</span></span> 
    
- <span data-ttu-id="99e65-115">[Automatinis atnaujinimas](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade) įgalintas pagal numatytuosius nustatymus aiškaus įrenginiams ir padeda užtikrinti jūsų versija Azure AD Connect visada yra dabartinė.</span><span class="sxs-lookup"><span data-stu-id="99e65-115">[Automatic upgrade](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade) is enabled by default for express installations and helps ensure your version of Azure AD Connect is always current.</span></span> 
    

