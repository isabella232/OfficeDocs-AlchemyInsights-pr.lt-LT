---
title: Taikomosios programos registracijos savininko problemos
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004352"
- "9655"
ms.openlocfilehash: 9dc3b1d54bb263d5e53e02a4e4dadc8cf3c1e400
ms.sourcegitcommit: 1f43598a726cdb9904aa501eb8db87f143020d9e
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 03/23/2021
ms.locfileid: "51404778"
---
# <a name="app-registration-owner-issues"></a><span data-ttu-id="ae7ee-102">Taikomosios programos registracijos savininko problemos</span><span class="sxs-lookup"><span data-stu-id="ae7ee-102">App Registration Owner issues</span></span>

<span data-ttu-id="ae7ee-103">Toliau pateikiami galimi būdai įtraukti vadovus kaip taikomųjų programų registracijų savininkus:</span><span class="sxs-lookup"><span data-stu-id="ae7ee-103">Following are the available methods to add principals as owners for app registrations:</span></span>

- <span data-ttu-id="ae7ee-104">"Azure AD PowerShell" modulio naudojimas –</span><span class="sxs-lookup"><span data-stu-id="ae7ee-104">Using Azure AD PowerShell Module -</span></span>

    `Connect-AzureAd`

    `Add-AzureADApplicationOwner -ObjectId <Application ObjectId>-RefObjectId <ObjectID of principal to assign as owner>`

    <span data-ttu-id="ae7ee-105">Nuoroda: [Add-AzureADApplicationOwner (AzureAD)](https://docs.microsoft.com/powershell/module/azuread/add-azureadapplicationowner)</span><span class="sxs-lookup"><span data-stu-id="ae7ee-105">Reference: [Add-AzureADApplicationOwner (AzureAD)](https://docs.microsoft.com/powershell/module/azuread/add-azureadapplicationowner)</span></span>
- <span data-ttu-id="ae7ee-106">"Azure CLI" naudojimas – `az ad app owner add`</span><span class="sxs-lookup"><span data-stu-id="ae7ee-106">Using Azure CLI - `az ad app owner add`</span></span>

    <span data-ttu-id="ae7ee-107">Nuoroda: [az ad app owner](https://docs.microsoft.com/cli/azure/ad/app/owner)</span><span class="sxs-lookup"><span data-stu-id="ae7ee-107">Reference: [az ad app owner](https://docs.microsoft.com/cli/azure/ad/app/owner)</span></span>
- <span data-ttu-id="ae7ee-108">MS Graph naudojimas –</span><span class="sxs-lookup"><span data-stu-id="ae7ee-108">Using MS Graph -</span></span>

    <span data-ttu-id="ae7ee-109">Nuoroda: [Savininko įtraukimas – "Microsoft Graph v1.0"](https://docs.microsoft.com/graph/api/application-post-owners)</span><span class="sxs-lookup"><span data-stu-id="ae7ee-109">Reference: [Add owner - Microsoft Graph v1.0](https://docs.microsoft.com/graph/api/application-post-owners)</span></span>
- <span data-ttu-id="ae7ee-110">"Azure AD" portalo naudojimas – pereikite [į portal.azure.com](https://portal.azure.com/) > Azure Active directory > App Registration > Select your application > Owners > Add Owners</span><span class="sxs-lookup"><span data-stu-id="ae7ee-110">Using the Azure AD Portal - Navigate to [portal.azure.com](https://portal.azure.com/) > Azure Active directory > App Registration > Select your application > Owners > Add Owners</span></span>

<span data-ttu-id="ae7ee-111">**Negalite peržiūrėti savo taikomosios programos "App Registrations" ašmenyje, net jei esate tos taikomosios programos savininkas?**</span><span class="sxs-lookup"><span data-stu-id="ae7ee-111">**Cannot view your application on App Registrations blade even though you are the owner of that application?**</span></span>

<span data-ttu-id="ae7ee-112">Taikomosios programos savininkas nėra administravimo vaidmuo.</span><span class="sxs-lookup"><span data-stu-id="ae7ee-112">Owner of an app is not an administrative role.</span></span> <span data-ttu-id="ae7ee-113">Jei parametras [Apriboti prieigą prie "Azure AD"](https://docs.microsoft.com/azure/active-directory/fundamentals/users-default-permissions) administravimo portalo įgalintas, tada tik administratorius galės peržiūrėti taikomąsias programas taikomųjų programų registracijos portale.</span><span class="sxs-lookup"><span data-stu-id="ae7ee-113">If the setting [Restrict access to Azure AD administration portal](https://docs.microsoft.com/azure/active-directory/fundamentals/users-default-permissions) is enabled, then only admin will be able to view the applications on App Registration portal.</span></span> <span data-ttu-id="ae7ee-114">Kad savininkas galėtų peržiūrėti taikomąsias programas, išjunkite šį parametrą (nustatykite jį kaip NE) arba priskirkite savininkui tik konkrečios taikomosios programos administratoriaus vaidmenį.</span><span class="sxs-lookup"><span data-stu-id="ae7ee-114">For an owner to be able to view the applications, either disable this setting (Set this to NO) or assign admin role to the owner for only the specific application.</span></span> <span data-ttu-id="ae7ee-115">Tačiau tam reikės "Azure AD Premium P2" licencijos ir įgalinsite [privilegijuotą tapatybės valdymą.](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-configure)</span><span class="sxs-lookup"><span data-stu-id="ae7ee-115">However for this, you will require an Azure AD Premium P2 license and enable [Privileged Identity Management](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-configure).</span></span>
