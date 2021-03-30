---
title: "\"Azure Active Directory\" prisijungimas"
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/24/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003257"
- "9890"
ms.openlocfilehash: 59e3798131956847a61af2416c2e4210199cffa5
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 03/29/2021
ms.locfileid: "51405055"
---
# <a name="azure-active-directory-join"></a><span data-ttu-id="d16bd-102">"Azure Active Directory" prisijungimas</span><span class="sxs-lookup"><span data-stu-id="d16bd-102">Azure Active Directory join</span></span>

1. <span data-ttu-id="d16bd-103">Jei pirmą kartą nustatote įrenginių registracijas, įsitikinkite, kad peržiūrėjote ["Azure Active Directory"](/azure/active-directory/devices/overview) įrenginių valdymo įvadas, kuri padės jums sužinoti, kaip "Azure AD" valdyti įrenginius.</span><span class="sxs-lookup"><span data-stu-id="d16bd-103">If you are setting up device registrations for the first time, ensure that you have reviewed [Introduction to device management in Azure Active Directory](/azure/active-directory/devices/overview) that will guide you on how to get Devices under the control to Azure AD.</span></span> 
1. <span data-ttu-id="d16bd-104">Jei registruosite įrenginius į "Azure AD" tiesiogiai ir užregistruosite juos "Intune", turėsite įsitikinti, kad sukonfigūravote ["Intune"](/mem/intune/enrollment/device-enrollment) ir pirmiausia [turite](/mem/intune/fundamentals/licenses-assign) licencijavimą.</span><span class="sxs-lookup"><span data-stu-id="d16bd-104">If you are registering devices into Azure AD directly and enrolling them into Intune, you will need to ensure that you have [configured Intune](/mem/intune/enrollment/device-enrollment) and have the [licensing](/mem/intune/fundamentals/licenses-assign) in place first.</span></span>
1. <span data-ttu-id="d16bd-105">Įsitikinkite, kad turite teisę atlikti operacijas "Azure AD".</span><span class="sxs-lookup"><span data-stu-id="d16bd-105">Ensure you are authorized to perform operations in Azure AD.</span></span> <span data-ttu-id="d16bd-106">Įrenginio registracijų parametrus gali valdyti tik visuotinis "Azure AD" administratorius.</span><span class="sxs-lookup"><span data-stu-id="d16bd-106">Only a global administrator in Azure AD can manage settings for device registrations.</span></span>
1. <span data-ttu-id="d16bd-107">Norėdami atlikti "Azure AD" sujungimo įgyvendinimą, [žr. "Azure AD Join" planas.](/azure/active-directory/devices/azureadjoin-plan)</span><span class="sxs-lookup"><span data-stu-id="d16bd-107">To do Azure AD join implementation, see [Plan Azure AD Join](/azure/active-directory/devices/azureadjoin-plan).</span></span>

<span data-ttu-id="d16bd-108">Daugiau informacijos apie dažnai pasitaikančių "Azure AD" prisijungimo problemų sprendimą žr. ["Azure Ad Join" DUK](/azure/active-directory/devices/faq) ir "Windows 10 pro" įrenginys, žr. Nepavyksta [prisijungti prie "Windows 10 Pro"](https://answers.microsoft.com/en-us/msoffice/forum/msoffice_install-mso_win10-mso_365hp/unable-to-join-windows-10-pro-machine-to-azure-ad/abb1ca7d-b317-45ec-a628-e1c10eae2900)įrenginio į "Azure AD" – reikia atnaujinti versiją į – "Microsoft Community".</span><span class="sxs-lookup"><span data-stu-id="d16bd-108">For more details on resolving common issues with Azure AD join, see [Azure Ad Join FAQ](/azure/active-directory/devices/faq) and for Windows 10 pro device, see [Unable to join Windows 10 Pro machine to Azure AD - Need to upgrade to - Microsoft Community](https://answers.microsoft.com/en-us/msoffice/forum/msoffice_install-mso_win10-mso_365hp/unable-to-join-windows-10-pro-machine-to-azure-ad/abb1ca7d-b317-45ec-a628-e1c10eae2900).</span></span>
