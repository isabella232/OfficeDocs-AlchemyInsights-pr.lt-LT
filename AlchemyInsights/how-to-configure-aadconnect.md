---
title: 646 kaip sukonfigūruoti AADConnect
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 6/8/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 646
ms.assetid: 599698ac-6709-477a-a66f-169b3165064e
ms.openlocfilehash: 2dc4ae7d6809c24ce599ac128570e9354c9f2b30
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 06/07/2019
ms.locfileid: "34752569"
---
# <a name="configure-sync-features"></a><span data-ttu-id="5e06a-102">Konfigūruoti sinchronizavimo funkcijos</span><span class="sxs-lookup"><span data-stu-id="5e06a-102">Configure sync features</span></span>

<span data-ttu-id="5e06a-103">Žydros AD jungtis yra kelios funkcijos, yra įjungta pagal numatytuosius nustatymus, arba, kad galite įgalinti vėliau.</span><span class="sxs-lookup"><span data-stu-id="5e06a-103">Azure AD Connect includes several features that are enabled by default, or that you can enable later.</span></span> <span data-ttu-id="5e06a-104">Kai kurios funkcijos reikalauja papildomos konfigūracijos konkrečių aplinkoje.</span><span class="sxs-lookup"><span data-stu-id="5e06a-104">Some features require additional configuration in specific environments.</span></span>

- <span data-ttu-id="5e06a-105">[Filtravimas](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-configure-filtering) ribas objektai yra sinchronizuoti su Azure AD.</span><span class="sxs-lookup"><span data-stu-id="5e06a-105">[Filtering](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-configure-filtering) limits the objects are synchronized to Azure AD.</span></span> <span data-ttu-id="5e06a-106">Iš numatytasis, visi vartotojai, kontaktus, grupes ir "Windows 10" sinchronizuojami kompiuterių sąskaitos.</span><span class="sxs-lookup"><span data-stu-id="5e06a-106">By default, all users, contacts, groups, and Windows 10 computer accounts are synchronized.</span></span> <span data-ttu-id="5e06a-107">Jūs galite įtraukti arba pašalinti objektus, domenai, organizaciniai vienetai ar kiti atributai.</span><span class="sxs-lookup"><span data-stu-id="5e06a-107">You can include or exclude objects based on domains, OUs, or other attributes.</span></span>

- <span data-ttu-id="5e06a-108">[Slaptažodis maiša sinchronizavimas](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-implement-password-hash-synchronization) sinchronizuoti slaptažodį maišos iš vietinės Active Directory su Azure AD.</span><span class="sxs-lookup"><span data-stu-id="5e06a-108">[Password hash syncronization](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-implement-password-hash-synchronization) synchronizes the password hash from the on-premises Active Directory to Azure AD.</span></span> <span data-ttu-id="5e06a-109">Tokiu būdu slapta˛od˛io valdymo vienoje vietoje, bet naudoti tą patį slaptažodį, tiek vietiniame ir debesų kompiuterijos aplinkose.</span><span class="sxs-lookup"><span data-stu-id="5e06a-109">This allows password management in one location, but use of the same password in both on-premises and cloud environments.</span></span> <span data-ttu-id="5e06a-110">Todėl, kad Active Directory yra patikimas šaltinis, galite naudoti savo slaptažodžio strategijų.</span><span class="sxs-lookup"><span data-stu-id="5e06a-110">Because Active Directory is the authoritative source, you can use your own password policies.</span></span>

- <span data-ttu-id="5e06a-111">[Savitarnos slaptažodžio nustatymo iš naujo (SSPR)](https://docs.microsoft.com/azure/active-directory/authentication/quickstart-sspr) leidžia vartotojams iš naujo nustatyti savo slaptažodžius debesis dar taikant vietinę slaptažodžių strategija.</span><span class="sxs-lookup"><span data-stu-id="5e06a-111">[Self-service password reset (SSPR)](https://docs.microsoft.com/azure/active-directory/authentication/quickstart-sspr) allows users to reset their own passwords in the cloud while still applying your on-premises password policy.</span></span>

- <span data-ttu-id="5e06a-112">[Įrenginio write-back](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-device-writeback) leidžia registruoti įrenginiai Azure AD įrašomi atgal į vietinės Active Directory, jie gali būti naudojami dėl sąlygine prieiga.</span><span class="sxs-lookup"><span data-stu-id="5e06a-112">[Device writeback](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-device-writeback) allows registered devices in Azure AD to be written back to the on-premises Active Directory so they can be used for conditional access.</span></span>

- <span data-ttu-id="5e06a-113">[Išvengti atsitiktinio panaikina](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-feature-prevent-accidental-deletes) yra įjungta pagal nutylėjimą padeda išvengti per daug vienu metu objektas naikinimus (daugiau kaip 500 objektų už sinchronizavimo).</span><span class="sxs-lookup"><span data-stu-id="5e06a-113">[Prevent accidental deletes](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-feature-prevent-accidental-deletes) is enabled by default to help prevent too many simultaneous object deletions (more than 500 objects per synchronization).</span></span> <span data-ttu-id="5e06a-114">Galite pakeisti šį nustatymą, kad atitiktų jūsų organizacijos poreikius.</span><span class="sxs-lookup"><span data-stu-id="5e06a-114">You can change this setting to meet the needs of your organization.</span></span>

- <span data-ttu-id="5e06a-115">[Automatinis atnaujinimas](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade) įgalintas pagal numatytuosius nustatymus aiškaus įrenginiams ir padeda užtikrinti jūsų versija Azure AD Connect visada yra dabartinė.</span><span class="sxs-lookup"><span data-stu-id="5e06a-115">[Automatic upgrade](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade) is enabled by default for express installations and helps ensure your version of Azure AD Connect is always current.</span></span>
