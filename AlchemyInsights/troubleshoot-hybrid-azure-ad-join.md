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
# <a name="troubleshoot-hybrid-azure-ad-join"></a><span data-ttu-id="99bd1-102">Hibridinio „Azure AD“ prisijungimo gedimų šalinimas</span><span class="sxs-lookup"><span data-stu-id="99bd1-102">Troubleshoot Hybrid Azure AD join</span></span>

<span data-ttu-id="99bd1-103">Labai rekomenduojama įsitikinti, kad įrenginys gali pasiekti įrenginio registracijos galinius punktus pagal sistemos paskyrą naudodamas [„Tikrinti įrenginio registracijos ryšį“](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/) scenarijų.</span><span class="sxs-lookup"><span data-stu-id="99bd1-103">Highly Recommended Ensure that a device can access Device Registration endpoints under the system account by using the [Test Device Registration Connectivity script](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/).</span></span>

1. <span data-ttu-id="99bd1-104">Jei įrenginių registraciją nustatote pirmą kartą, būtinai peržiūrėkite Į[vadas į įrenginių valdymą „Azure Active Directory“](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/), kad sužinotumėte, kaip pasiekti, kad įrenginiai būtų valdomi „Azure AD“.</span><span class="sxs-lookup"><span data-stu-id="99bd1-104">If you are setting up device registrations for the first time, be sure to review I[ntroduction to device management in Azure Active Directory](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/) to learn how to get devices under the control of Azure AD.</span></span>
1. <span data-ttu-id="99bd1-105">Jei tiesiogiai registruojate įrenginius į „Azure AD“ ir registruojate juos į „Intune“, įsitikinkite, kad [sukonfigūravote „Intune“](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment?WT.mc_id=Portal-Microsoft_Azure_Support) ir pirmiausia turite [licencijavimą](https://docs.microsoft.com/mem/intune/fundamentals/licenses-assign?WT.mc_id=Portal-Microsoft_Azure_Support).</span><span class="sxs-lookup"><span data-stu-id="99bd1-105">If you are registering devices into Azure AD directly and enrolling them into Intune, be sure that you've [configured Intune](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment?WT.mc_id=Portal-Microsoft_Azure_Support) and have the [licensing](https://docs.microsoft.com/mem/intune/fundamentals/licenses-assign?WT.mc_id=Portal-Microsoft_Azure_Support) in place first.</span></span>
1. <span data-ttu-id="99bd1-106">Įsitikinkite, kad esate įgaliotas atlikti operacijas „Azure AD“ ir vietiniame AD.</span><span class="sxs-lookup"><span data-stu-id="99bd1-106">Ensure that you are authorized to perform operations in Azure AD and on-premises AD.</span></span> <span data-ttu-id="99bd1-107">Tik visuotinis „Azure AD“ administratorius gali valdyti įrenginių registravimo parametrus.</span><span class="sxs-lookup"><span data-stu-id="99bd1-107">Only a global administrator in Azure AD can manage settings for device registrations.</span></span> <span data-ttu-id="99bd1-108">Be to, jei vietiniame „Active Directory“ nustatote automatines registracijas, turėsite būti „Active Directory“ ir „AD FS“ (jei taikoma) administratorius.</span><span class="sxs-lookup"><span data-stu-id="99bd1-108">In addition, if you are setting up automatic registrations in your on-premises Active Directory, you will need to be an administrator of Active Directory and AD FS (if applicable).</span></span>

<span data-ttu-id="99bd1-109">Norėdami gauti daugiau informacijos apie galimas hibridinio prisijungimo problemas, žr. [„Hibridinio prisijungimo gedimų šalinimas“](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-hybrid-join-windows-current), kad nustatytumėte sujungtą hibridinį „Azure AD“ ir valdytumėte įrenginius naudojant „Azure ad“ portalą, žr. [Nustatyti hibridinius „Azure AD“ sujungtus (vietinius, prijungtus prie domeno) įrenginius](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan?WT.mc_id=Portal-Microsoft_Azure_Support) ir [Valdyti įrenginius „Azure“ portale](https://docs.microsoft.com/azure/active-directory/devices/device-management-azure-portal?WT.mc_id=Portal-Microsoft_Azure_Support).</span><span class="sxs-lookup"><span data-stu-id="99bd1-109">For more details on resolve potential issues with Hybrid join, see [Troubleshoot Hybrid Join](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-hybrid-join-windows-current) for set up hybrid Azure AD joined and Manage Devices using Azure Ad portal, see [Set up hybrid Azure AD joined (on-premises domain-joined) devices](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan?WT.mc_id=Portal-Microsoft_Azure_Support) and [Manage devices using the Azure portal](https://docs.microsoft.com/azure/active-directory/devices/device-management-azure-portal?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>

<span data-ttu-id="99bd1-110">Norėdami išspręsti bendrąsias hibridinio „Azure Active Directory“ (AD) prisijungimo problemas, žr. [Hibridinio „Azure AD“ prisijungimo DUK](https://docs.microsoft.com/azure/active-directory/devices/faq#hybrid-azure-ad-join-faq).</span><span class="sxs-lookup"><span data-stu-id="99bd1-110">To resolve common issues with Hybrid Azure Active Directory (AD) join, see [Hybrid Azure AD join FAQ](https://docs.microsoft.com/azure/active-directory/devices/faq#hybrid-azure-ad-join-faq).</span></span>
