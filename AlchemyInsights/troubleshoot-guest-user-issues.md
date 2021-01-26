---
title: Svečio vartotojų problemų šalinimas
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/18/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004358"
- "7822"
ms.openlocfilehash: 0f2a10b918fee067b167ab58ac2544a89e0c8ea1
ms.sourcegitcommit: 7b213fd5e8a3fdb5c602673dc194d576d372ac96
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 01/18/2021
ms.locfileid: "49901596"
---
# <a name="troubleshoot-guest-user-issues"></a><span data-ttu-id="f20cd-102">Svečio vartotojų problemų šalinimas</span><span class="sxs-lookup"><span data-stu-id="f20cd-102">Troubleshoot guest user issues</span></span>

1. <span data-ttu-id="f20cd-103">Patarimų, kaip valdyti svečio prieigą prie taikomųjų programų, ieškokite [svečio prieigos valdymas naudojant "AZURE ad Access" atsiliepimus](https://docs.microsoft.com/azure/active-directory/governance/manage-guest-access-with-access-reviews).</span><span class="sxs-lookup"><span data-stu-id="f20cd-103">For guidance on managing guest access to applications, see [Manage guest access with Azure AD access reviews](https://docs.microsoft.com/azure/active-directory/governance/manage-guest-access-with-access-reviews).</span></span>
1. <span data-ttu-id="f20cd-104">[Įtraukite Svečių vartotojus į savo katalogą "Azure" portale](https://docs.microsoft.com/azure/active-directory/external-identities/b2b-quickstart-add-guest-users-portal): šiame "QuickStart" į "Azure AD" katalogą į "Azure AD" portalą įtrauksite naują svečio portalą naudodami "Azure" portalą, išsiųstumėte kvietimą ir pamatytumėte, kaip atrodo svečio vartotojo kvietimo išpirkimo procesas.</span><span class="sxs-lookup"><span data-stu-id="f20cd-104">[Add guest users to your directory in the Azure portal](https://docs.microsoft.com/azure/active-directory/external-identities/b2b-quickstart-add-guest-users-portal): In this quickstart, you'll add a new guest user to your Azure AD directory via the Azure portal, send an invitation, and see what the guest user's invitation redemption process looks like.</span></span>
1. <span data-ttu-id="f20cd-105">[Įtraukti svečio vartotoją su "PowerShell](https://docs.microsoft.com/azure/active-directory/external-identities/b2b-quickstart-invite-powershell)": šiame "QuickStart" naudokite komandą New-AzureADMSInvitation, kad įtrauktumėte vieną svečio vartotoją į savo "Azure" nuomotoją.</span><span class="sxs-lookup"><span data-stu-id="f20cd-105">[Add a guest user with PowerShell](https://docs.microsoft.com/azure/active-directory/external-identities/b2b-quickstart-invite-powershell): In this quickstart, you’ll use the New-AzureADMSInvitation command to add one guest user to your Azure tenant.</span></span>
1. <span data-ttu-id="f20cd-106">Norėdami sužinoti, kaip priskirti vartotojus ir grupes, įmonės taikomąsias programas "Azure Active Directory" ("Azure AD"), iš "Azure" portalo arba naudodami "PowerShell", žr. ["Azure Active Directory" taikomosios programos vartotojo priskyrimo valdymas](https://docs.microsoft.com/azure/active-directory/manage-apps/assign-user-or-group-access-portal).</span><span class="sxs-lookup"><span data-stu-id="f20cd-106">To learn how to assign users, and groups, to enterprise applications in Azure Active Directory (Azure AD), either from within the Azure portal or by using PowerShell, see [Manage user assignment for an app in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/manage-apps/assign-user-or-group-access-portal).</span></span> 
1. <span data-ttu-id="f20cd-107">"Azure Active Directory" ("Azure AD") B2B bendradarbiavimas veikia su daugeliu programų, kurios integruojasi su "Azure AD".</span><span class="sxs-lookup"><span data-stu-id="f20cd-107">Azure Active Directory (Azure AD) B2B collaboration works with most apps that integrate with Azure AD.</span></span> <span data-ttu-id="f20cd-108">Šiame [straipsnyje](https://docs.microsoft.com/azure/active-directory/external-identities/configure-saas-apps)pateikiame instrukcijas, kaip konfigūruoti kai kurias populiarias "SaaS" taikomąsias programas, skirtas naudoti su "AZURE ad B2B".</span><span class="sxs-lookup"><span data-stu-id="f20cd-108">In this [article](https://docs.microsoft.com/azure/active-directory/external-identities/configure-saas-apps), we walk through instructions for configuring some popular SaaS apps for use with Azure AD B2B.</span></span>
1. <span data-ttu-id="f20cd-109">Kaip organizacija, naudojanti "Azure Active Directory" ("Azure AD") B2B bendradarbiavimo galimybes, siekiant pakviesti Svečių vartotojus iš partnerių organizacijų į "Azure AD", dabar galite pateikti šiems B2B vartotojams prieigą prie vietinių taikomųjų programų.</span><span class="sxs-lookup"><span data-stu-id="f20cd-109">As an organization that uses Azure Active Directory (Azure AD) B2B collaboration capabilities to invite guest users from partner organizations to your Azure AD, you can now provide these B2B users access to on-premises apps.</span></span> <span data-ttu-id="f20cd-110">Šios vietinio naudojimo programos gali naudoti SAML pagrįstą autentifikavimą arba integruotą "Windows" autentifikavimą (IWA) su "Kerberos" ribojtu perdavimu (KCD).</span><span class="sxs-lookup"><span data-stu-id="f20cd-110">These on-premises apps can use SAML-based authentication or Integrated Windows Authentication (IWA) with Kerberos constrained delegation (KCD).</span></span> <span data-ttu-id="f20cd-111">Daugiau informacijos ieškokite ["AZURE AD" prieigos prie vietinių taikomųjų programų B2B vartotojų suteikimas](https://docs.microsoft.com/azure/active-directory/external-identities/hybrid-cloud-to-on-premises).</span><span class="sxs-lookup"><span data-stu-id="f20cd-111">For more information, see [Grant B2B users in Azure AD access to your on-premises applications](https://docs.microsoft.com/azure/active-directory/external-identities/hybrid-cloud-to-on-premises).</span></span>
1. <span data-ttu-id="f20cd-112">Sužinokite, kaip [suteikti vietinio valdymo partnerio paskyras prieigą prie debesies išteklių naudojant "AZURE ad B2B Collaboration](https://docs.microsoft.com/azure/active-directory/external-identities/hybrid-on-premises-to-cloud)".</span><span class="sxs-lookup"><span data-stu-id="f20cd-112">Learn how to [grant locally-managed partner accounts access to cloud resources using Azure AD B2B collaboration](https://docs.microsoft.com/azure/active-directory/external-identities/hybrid-on-premises-to-cloud).</span></span>