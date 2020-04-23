---
title: 646 Kaip sukonfigūruoti AADConnect
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "646"
- "1300023"
ms.assetid: 599698ac-6709-477a-a66f-169b3165064e
ms.openlocfilehash: 713cda26e55f07f0438cb9ebe5aa9da86c4ebb3a
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 04/22/2020
ms.locfileid: "43722571"
---
# <a name="configure-sync-features"></a><span data-ttu-id="f920f-102">Sinchronizavimo funkcijų konfigūravimas</span><span class="sxs-lookup"><span data-stu-id="f920f-102">Configure sync features</span></span>

<span data-ttu-id="f920f-103">"Azure AD Connect" yra kelios funkcijos, kurios įgalintos pagal numatytuosius nustatymus arba kurias galite įgalinti vėliau.</span><span class="sxs-lookup"><span data-stu-id="f920f-103">Azure AD Connect includes several features that are enabled by default, or that you can enable later.</span></span> <span data-ttu-id="f920f-104">Kai kurioms funkcijoms reikia papildomos konfigūracijos konkrečiose aplinkose.</span><span class="sxs-lookup"><span data-stu-id="f920f-104">Some features require additional configuration in specific environments.</span></span>

- <span data-ttu-id="f920f-105">[Filtravimo](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-configure-filtering) apribojimai objektai sinchronizuojami su Azure AD.</span><span class="sxs-lookup"><span data-stu-id="f920f-105">[Filtering](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-configure-filtering) limits the objects are synchronized to Azure AD.</span></span> <span data-ttu-id="f920f-106">Pagal numatytuosius nustatymus sinchronizuojami visi vartotojai, kontaktai, grupės ir "Windows 10" kompiuterių abonementai.</span><span class="sxs-lookup"><span data-stu-id="f920f-106">By default, all users, contacts, groups, and Windows 10 computer accounts are synchronized.</span></span> <span data-ttu-id="f920f-107">Galite įtraukti arba išskirti objektus pagal domenus, ous ar kitus atributus.</span><span class="sxs-lookup"><span data-stu-id="f920f-107">You can include or exclude objects based on domains, OUs, or other attributes.</span></span>

- <span data-ttu-id="f920f-108">[Slaptažodžio maišos sinchronizavimas](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-implement-password-hash-synchronization) sinchronizuoja slaptažodžio maišą iš vietinės "Active Directory" į "Azure AD".</span><span class="sxs-lookup"><span data-stu-id="f920f-108">[Password hash synchronization](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-implement-password-hash-synchronization) synchronizes the password hash from the on-premises Active Directory to Azure AD.</span></span> <span data-ttu-id="f920f-109">Tai leidžia valdyti slaptažodžius vienoje vietoje, bet naudoti tą patį slaptažodį tiek vietinėje, tiek debesies aplinkoje.</span><span class="sxs-lookup"><span data-stu-id="f920f-109">This allows password management in one location, but use of the same password in both on-premises and cloud environments.</span></span> <span data-ttu-id="f920f-110">Kadangi "Active Directory" yra patikimas šaltinis, galite naudoti savo slaptažodžių strategijas.</span><span class="sxs-lookup"><span data-stu-id="f920f-110">Because Active Directory is the authoritative source, you can use your own password policies.</span></span>

- <span data-ttu-id="f920f-111">[Savitarnos slaptažodžio nustatymas iš naujo (SSPR)](https://docs.microsoft.com/azure/active-directory/authentication/quickstart-sspr) leidžia vartotojams iš naujo nustatyti savo slaptažodžius debesyje, tačiau vis dar taiko jūsų vietinę slaptažodžio politiką.</span><span class="sxs-lookup"><span data-stu-id="f920f-111">[Self-service password reset (SSPR)](https://docs.microsoft.com/azure/active-directory/authentication/quickstart-sspr) allows users to reset their own passwords in the cloud while still applying your on-premises password policy.</span></span>

- <span data-ttu-id="f920f-112">[Įrenginio perrašymas](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-device-writeback) leidžia registruotus įrenginius Azure AD galima rašyti atgal į vietinę Active Directory, kad jie gali būti naudojami sąlyginės prieigos.</span><span class="sxs-lookup"><span data-stu-id="f920f-112">[Device writeback](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-device-writeback) allows registered devices in Azure AD to be written back to the on-premises Active Directory so they can be used for conditional access.</span></span>

- <span data-ttu-id="f920f-113">[Užkirsti kelią atsitiktiniams naikinimams](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-feature-prevent-accidental-deletes) pagal numatytuosius nustatymus įgalinta, kad būtų išvengta per daug vienu metu esančių objektų naikinimų (daugiau nei 500 objektų sinchronizuojant).</span><span class="sxs-lookup"><span data-stu-id="f920f-113">[Prevent accidental deletes](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-feature-prevent-accidental-deletes) is enabled by default to help prevent too many simultaneous object deletions (more than 500 objects per synchronization).</span></span> <span data-ttu-id="f920f-114">Šį parametrą galite pakeisti, kad jis atitiktų jūsų organizacijos poreikius.</span><span class="sxs-lookup"><span data-stu-id="f920f-114">You can change this setting to meet the needs of your organization.</span></span>

- <span data-ttu-id="f920f-115">[Automatinis naujinimas](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade) yra įjungtas pagal numatytuosius nustatymus express įrenginių ir padeda užtikrinti, kad jūsų versija Azure AD Connect visada yra dabartinis.</span><span class="sxs-lookup"><span data-stu-id="f920f-115">[Automatic upgrade](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade) is enabled by default for express installations and helps ensure your version of Azure AD Connect is always current.</span></span>
