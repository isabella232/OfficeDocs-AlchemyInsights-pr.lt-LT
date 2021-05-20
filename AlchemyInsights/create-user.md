---
title: Kurti vartotoją
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/11/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003231"
- "9403"
ms.openlocfilehash: 800baae2d748708d8cb7a5fb0e73fce5dcf455cb
ms.sourcegitcommit: 2d617ae59eed0ce8b571339ceefce6473c03b94c
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 05/19/2021
ms.locfileid: "52569739"
---
# <a name="create-user"></a><span data-ttu-id="02c58-102">Kurti vartotoją</span><span class="sxs-lookup"><span data-stu-id="02c58-102">Create user</span></span>

<span data-ttu-id="02c58-103">**PRANEŠIMAS:**</span><span class="sxs-lookup"><span data-stu-id="02c58-103">**ANNOUNCEMENT:**</span></span>

- <span data-ttu-id="02c58-104">["WebView" prisijungimo palaikymo nutraukimas iš "Google" nuo 2021 m. sausio 4 d.](/azure/active-directory/external-identities/google-federation#deprecation-of-webview-sign-in-support)</span><span class="sxs-lookup"><span data-stu-id="02c58-104">[Deprecation of WebView sign-in support from Google starting January 4, 2021](/azure/active-directory/external-identities/google-federation#deprecation-of-webview-sign-in-support) .</span></span> <span data-ttu-id="02c58-105">Patikrinkite, ar jūsų programoms gali turėti įtakos ["Google" suderinamumo](https://go.microsoft.com/fwlink/?linkid=2157323) tikrinimo rekomendacijos.</span><span class="sxs-lookup"><span data-stu-id="02c58-105">Test whether your apps may be affected by following [Google’s guidance](https://go.microsoft.com/fwlink/?linkid=2157323) on testing compatibility.</span></span>
- <span data-ttu-id="02c58-106">Įsitikinkite, kad naudojate sistemos žiniatinklio rodinį arba sistemos naršyklę prisijungę prie vartotojų naudodami vartotojų "Google" paskyras.</span><span class="sxs-lookup"><span data-stu-id="02c58-106">Make sure you use the system webview or system browser when signing in your users with consumer Google accounts.</span></span> <span data-ttu-id="02c58-107">Daugiau informacijos žr. [Prisijungimo prie programos (-ų) naudojant tik "Chrome" naršyklę problemos.](/office365/troubleshoot/miscellaneous/chrome-behavior-affects-applications)</span><span class="sxs-lookup"><span data-stu-id="02c58-107">For more information, see [Issues signing in to application(s) using Chrome browser only](/office365/troubleshoot/miscellaneous/chrome-behavior-affects-applications).</span></span>

<span data-ttu-id="02c58-108">**Negaliu sukurti naujo vartotojo savo "Azure AD" kataloge**</span><span class="sxs-lookup"><span data-stu-id="02c58-108">**I can't create a new user in my Azure AD directory**</span></span>

1. <span data-ttu-id="02c58-109">Įsitikinkite, kad turite teisę sukurti naują standartinį vartotoją.</span><span class="sxs-lookup"><span data-stu-id="02c58-109">Ensure that you are authorized to create a new standard user.</span></span> <span data-ttu-id="02c58-110">Tik visuotinis administratorius arba vartotojo administratoriaus vaidmuo "Azure Active Directory" (AD) gali sukurti naują standartinį vartotoją.</span><span class="sxs-lookup"><span data-stu-id="02c58-110">Only the Global administrator or User administrator role in Azure Active Directory (AD) can create a new standard user.</span></span> <span data-ttu-id="02c58-111">Jei neturite vieno iš šių vaidmenų, paprašykite administratoriaus įtraukti jus į vieną iš šių vaidmenų arba sukurti naują vartotojo paskyrą už jus.</span><span class="sxs-lookup"><span data-stu-id="02c58-111">If you're not in one of these roles, ask an administrator to add you to one of these roles or to create the new user account for you.</span></span>
1. <span data-ttu-id="02c58-112">Įsitikinkite, kad vartotojo vardas yra domene, kuris patvirtintas jūsų "Azure AD".</span><span class="sxs-lookup"><span data-stu-id="02c58-112">Ensure that the user name is in a domain that is verified in your Azure AD.</span></span> <span data-ttu-id="02c58-113">Jei "Azure AD" neturite patikrintų pasirinktinių domenų vardų, galite naudoti "Azure AD" pradinį domeną, kuris baigiasi \*.onmicrosoft.com.</span><span class="sxs-lookup"><span data-stu-id="02c58-113">If you do not have any verified custom domain names in your Azure AD, you can use your Azure AD initial domain, which ends with \*.onmicrosoft.com.</span></span>
1. <span data-ttu-id="02c58-114">Įsitikinkite, kad vartotojo vardas yra domene, kuris nėra susietas su "Azure AD" iš jūsų vietinio AD.</span><span class="sxs-lookup"><span data-stu-id="02c58-114">Ensure that the user name is in a domain that is not federated to Azure AD from your on-premises AD.</span></span> <span data-ttu-id="02c58-115">Vartotojų negalima įtraukti į debesį su domenų vardais, kurie yra išoriniai iš vietinės.</span><span class="sxs-lookup"><span data-stu-id="02c58-115">Users cannot be added in the cloud with domain names that are federated from on-premises.</span></span>
1. <span data-ttu-id="02c58-116">Įsitikinkite, kad joks kitas vartotojas ar kontaktas dar neturi vartotojo vardo, kurį norite priskirti naujam vartotojui.</span><span class="sxs-lookup"><span data-stu-id="02c58-116">Ensure that no other user or contact already has the user name that you want to assign to the new user.</span></span> <span data-ttu-id="02c58-117">Vartotojų vardai turi būti unikalūs visoje "Azure AD".</span><span class="sxs-lookup"><span data-stu-id="02c58-117">User names must be unique across Azure AD.</span></span>
1. <span data-ttu-id="02c58-118">Žr. ["Azure AD" vaidmenys ir "Azure](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/RolesAndAdministrators) AD" administratoriai.</span><span class="sxs-lookup"><span data-stu-id="02c58-118">See [Azure AD roles and administrators](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/RolesAndAdministrators) for your Azure AD.</span></span>
1. <span data-ttu-id="02c58-119">Peržiūrėkite ["Azure](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/RolesAndAdministrators) AD" domenų vardus.</span><span class="sxs-lookup"><span data-stu-id="02c58-119">See the [domain names](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/RolesAndAdministrators) for your Azure AD.</span></span>
1. <span data-ttu-id="02c58-120">Peržiūrėkite [audito žurnalus,](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/RolesAndAdministrators) kad pamatytumėte išsamesnę informaciją apie neseniai sukurtą arba panaikintus vartotoją, pvz., kas atliko veiksmą ir kada.</span><span class="sxs-lookup"><span data-stu-id="02c58-120">Review [Audit logs](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/RolesAndAdministrators) to see more detailed information about a recently created or deleted user like who performed the action and when.</span></span>
1. <span data-ttu-id="02c58-121">Daugiau informacijos apie naujų vartotojų įtraukimą žr. ["Azure" portalo naudojimas kuriant naują vartotoją "Azure AD".](/azure/active-directory/active-directory-users-create-azure-portal)</span><span class="sxs-lookup"><span data-stu-id="02c58-121">For more information on adding new users, see [Use the Azure portal to create a new user in your Azure AD](/azure/active-directory/active-directory-users-create-azure-portal).</span></span>
1. <span data-ttu-id="02c58-122">["Azure AD" administravimo vaidmenys:](/azure/active-directory/active-directory-assign-admin-roles)administratoriaus vaidmens teisės "Azure Active Directory"</span><span class="sxs-lookup"><span data-stu-id="02c58-122">[Azure AD administrative roles](/azure/active-directory/active-directory-assign-admin-roles): Administrator role permissions in Azure Active Directory</span></span>
1. <span data-ttu-id="02c58-123">Taip pat galite [naudoti "Azure AD PowerShell", kad sukurtumėte naują vartotoją.](/powershell/module/azuread/new-azureaduser?view=azureadps-2.0)</span><span class="sxs-lookup"><span data-stu-id="02c58-123">You can also [use Azure AD PowerShell to create a new user](/powershell/module/azuread/new-azureaduser?view=azureadps-2.0).</span></span>
