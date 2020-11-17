---
title: Privilegijuotas tapatybės valdymo vaidmuo
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003230"
- "6825"
ms.openlocfilehash: 726511d016462f56c48a4272b57abc3e9f0cbc3d
ms.sourcegitcommit: 35e2c122d8a838d98d1f0851c29b16282261580f
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 11/17/2020
ms.locfileid: "49088879"
---
# <a name="privileged-identity-managementpim-role"></a><span data-ttu-id="26f6c-102">Privilegijuotos tapatybės valdymo (PIM) vaidmuo</span><span class="sxs-lookup"><span data-stu-id="26f6c-102">Privileged Identity Management(PIM) role</span></span>

<span data-ttu-id="26f6c-103">**Teisės nesuteikiamos suaktyvinus vaidmenį**</span><span class="sxs-lookup"><span data-stu-id="26f6c-103">**Permissions are not granted after activating a role**</span></span>

<span data-ttu-id="26f6c-104">Kai suaktyvinate "Azure AD" privilegijuoto tapatybės valdymo (PIM) vaidmenį, aktyvinimas gali būti iš karto išplatintas visiems portaluose, kuriems būtinas privilegijuotas vaidmuo.</span><span class="sxs-lookup"><span data-stu-id="26f6c-104">When you activate a role in Azure AD Privileged Identity Management (PIM), the activation may not instantly propagate to all portals that require the privileged role.</span></span> <span data-ttu-id="26f6c-105">Kartais, net jei pakeitimai dauginami, žiniatinklio kaupimas svetainėje gali sukelti pakeitimus iš karto.</span><span class="sxs-lookup"><span data-stu-id="26f6c-105">Sometimes, even if the change is propagated, web caching in a portal may result in the change not taking effect immediately.</span></span>

<span data-ttu-id="26f6c-106">Jei aktyvinimas vėluoja, atlikite šiuos veiksmus:</span><span class="sxs-lookup"><span data-stu-id="26f6c-106">If your activation is delayed, follow these steps:</span></span>

1. <span data-ttu-id="26f6c-107">Atsijunkite nuo "Azure" portalo ir vėl prisijunkite.</span><span class="sxs-lookup"><span data-stu-id="26f6c-107">Sign out of the Azure portal and then sign back in.</span></span> <span data-ttu-id="26f6c-108">Kai suaktyvinsite "Azure AD" vaidmenį arba "Azure" išteklių vaidmenį, matysite aktyvinimo etapus.</span><span class="sxs-lookup"><span data-stu-id="26f6c-108">When you activate an Azure AD role or an Azure resource role, you will see the stages of your activation.</span></span> <span data-ttu-id="26f6c-109">Kai visi etapai bus baigti, matysite saitą Atsijungti.</span><span class="sxs-lookup"><span data-stu-id="26f6c-109">Once all the stages are complete, you will see a 'Sign out' link.</span></span> <span data-ttu-id="26f6c-110">Galite naudoti šį saitą, kad atsijungtumėte. Tai padės išspręsti daugumą aktyvinimo vėlavimo atvejų.</span><span class="sxs-lookup"><span data-stu-id="26f6c-110">You can use this link to sign out. This will solve most cases for activation delay.</span></span>
2. <span data-ttu-id="26f6c-111">"PIM" Patikrinkite, ar esate sąraše kaip vaidmens narys.</span><span class="sxs-lookup"><span data-stu-id="26f6c-111">In PIM, verify that you are listed as the member of the role.</span></span>
3. <span data-ttu-id="26f6c-112">Jei aktyvinate "Exchange" administratoriaus vaidmenį, įsitikinkite, kad atsijungiate ir vėl prisijungsite.</span><span class="sxs-lookup"><span data-stu-id="26f6c-112">If you are activating the Exchange Administrator role, make sure you sign out and sign back in.</span></span> <span data-ttu-id="26f6c-113">Jei problema kartojasi, atidarykite palaikymo bilietą ir iškelkite ją kaip problemą.</span><span class="sxs-lookup"><span data-stu-id="26f6c-113">If the problem persists, open a support ticket and raise this as an issue.</span></span> <span data-ttu-id="26f6c-114">Jei naudojate "Exchange" administratoriaus vaidmenį, kad pasiektumėte saugos ir atitikties centrą, peržiūrėkite paskesnį veiksmą.</span><span class="sxs-lookup"><span data-stu-id="26f6c-114">If you are using your Exchange Administrator role to access the Security and Compliance Center, see the next step.</span></span>
4. <span data-ttu-id="26f6c-115">Jei aktyvinate vaidmenį, kad pasiektumėte saugos ir atitikties centrą, arba jei aktyvinate "SharePoint" administratoriaus vaidmenį, nuo kelių minučių iki kelių valandų bus rodomas aktyvinimo vėlavimas.</span><span class="sxs-lookup"><span data-stu-id="26f6c-115">If you are activating a role to access the Security and Compliance Center or if you are activating the SharePoint Administrator role, you will experience some activation delay from a few minutes up to a few hours.</span></span> <span data-ttu-id="26f6c-116">Tai žinoma problema ir mes aktyviai bendradarbiaujame su šiomis komandomis, kad kuo greičiau išspręstumėte šią problemą.</span><span class="sxs-lookup"><span data-stu-id="26f6c-116">This is a known issue and we are actively working with these teams to resolve this issue as soon as possible.</span></span>

<span data-ttu-id="26f6c-117">Daugiau informacijos rasite:</span><span class="sxs-lookup"><span data-stu-id="26f6c-117">For more information, see:</span></span>

- [<span data-ttu-id="26f6c-118">"Azure AD" vaidmenų aktyvinimas "PIM"</span><span class="sxs-lookup"><span data-stu-id="26f6c-118">Activate my Azure AD roles in PIM</span></span>](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-how-to-activate-role?WT.mc_id=Portal-Microsoft_Azure_Support "https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-how-to-activate-role?wt.mc_id=portal-microsoft_azure_support")
- [<span data-ttu-id="26f6c-119">"Azure" išteklių vaidmenų aktyvinimas "PIM"</span><span class="sxs-lookup"><span data-stu-id="26f6c-119">Activate my Azure resource roles in PIM</span></span>](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-resource-roles-activate-your-roles?WT.mc_id=Portal-Microsoft_Azure_Support "https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-resource-roles-activate-your-roles?wt.mc_id=portal-microsoft_azure_support")

<span data-ttu-id="26f6c-120">**Teisės nepašalinamos po to, kai deaktyvintas vaidmuo arba vaidmens aktyvinimas baigiasi**</span><span class="sxs-lookup"><span data-stu-id="26f6c-120">**Permissions are not removed after deactivating a role or the role activation expires**</span></span>

<span data-ttu-id="26f6c-121">Kai išjungsite vaidmenį "Azure AD" privilegijuotoje tapatybės tvarkyme arba pasibaigus vaidmenų aktyvinimo laikotarpiui, gali būti, kad galite atidėti "Access".</span><span class="sxs-lookup"><span data-stu-id="26f6c-121">When you deactivate a role in Azure AD Privileged Identity Management or when a role activation period expires, there might be a delay where you continue to have access.</span></span>

<span data-ttu-id="26f6c-122">Jei jūsų aktyvinimas vėluoja, atlikite šiuos veiksmus:</span><span class="sxs-lookup"><span data-stu-id="26f6c-122">If your deactivation is delayed, follow these steps:</span></span>

1. <span data-ttu-id="26f6c-123">Jei išjungsite "Exchange" administratoriaus vaidmenį arba suaktyvinate vaidmens aktyvinimo laikotarpį, o jūs pastebėjote reikšmingą vėlavimą prieš panaikinant teises, atidarykite palaikymo bilietą ir praneškite savo palaikymo inžinieriui, kad padėtumėte jums gauti bilietą su privilegijuoto "Access Management" (PAM) komanda, esanti "Office" "Office" apie šią problemą.</span><span class="sxs-lookup"><span data-stu-id="26f6c-123">If you are deactivating the Exchange Administrator role or the role activation period expires, and you notice a significant delay before the permissions are removed, open a support ticket and tell your support engineer to help you file a ticket with the Privileged Access Management (PAM) team inside Office about this issue.</span></span>
2. <span data-ttu-id="26f6c-124">Jei baigėsi aktyvinimo laikotarpis, bet vis tiek atidaromas naršyklės seansas, uždarykite naršyklę.</span><span class="sxs-lookup"><span data-stu-id="26f6c-124">If the activation period has expired, but you still have the browser session open, close your browser.</span></span> <span data-ttu-id="26f6c-125">Galite toliau naudoti vaidmenį, kol uždarysite šį seansą.</span><span class="sxs-lookup"><span data-stu-id="26f6c-125">You can continue to use the role until you close that session.</span></span> <span data-ttu-id="26f6c-126">Tai žinoma problema ir mes ieškome galimų pataisų, kad aktyviai atšauktumėte kiekvieną seansą, kai aktyvinimas baigėsi.</span><span class="sxs-lookup"><span data-stu-id="26f6c-126">This is a known issue and we are looking at a potential fix to actively revoke each session once activation has expired.</span></span>

<span data-ttu-id="26f6c-127">Jei vėlavimas skiriasi nuo šių dviejų scenarijų, atidarykite palaikymo bilietą.</span><span class="sxs-lookup"><span data-stu-id="26f6c-127">If your delay is different than these two scenarios, please open a support ticket.</span></span>
