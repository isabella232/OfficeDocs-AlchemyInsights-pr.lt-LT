---
title: Problemos naudojant Intune administratoriaus konsolę
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/29/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1790"
- "9000214"
ms.openlocfilehash: 7a36d502a92d360b06336ccfa6183f666f0260ab
ms.sourcegitcommit: ffbed67c0a16ec423fa1d79b71e48ea4e2d320e1
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 07/29/2020
ms.locfileid: "46555386"
---
# <a name="problems-using-the-intune-admin-console"></a><span data-ttu-id="a8f30-102">Problemos naudojant Intune administratoriaus konsolę</span><span class="sxs-lookup"><span data-stu-id="a8f30-102">Problems using the Intune admin console</span></span>

<span data-ttu-id="a8f30-103">**"Prieiga uždrausta" naršant Intune administravimo portale.**</span><span class="sxs-lookup"><span data-stu-id="a8f30-103">**"Access denied" when navigating the Intune admin portal.**</span></span>

- <span data-ttu-id="a8f30-104">Jei esate "Intune" pasirinktinio vaidmens narys, įsitikinkite, kad jūsų abonementui priskirta "Intune" arba "Enterprise Mobility Suite" (EMS) licencija.</span><span class="sxs-lookup"><span data-stu-id="a8f30-104">If you are a member of an Intune custom role, ensure that an Intune or Enterprise Mobility Suite (EMS) license is assigned to your account.</span></span>
- <span data-ttu-id="a8f30-105">Jei naudojate konfigūracijos tvarkyklė valdyti įrenginius, patikrinkite, ar nesate dalis Intune vartotojų rinkinio konfigūracijos tvarkytuvo MDM.</span><span class="sxs-lookup"><span data-stu-id="a8f30-105">If you are using Configuration Manager to manage devices, verify you are not part of the Intune user collection for Configuration Manager MDM.</span></span>
- <span data-ttu-id="a8f30-106">Patikrinkite, ar jums buvo priskirtos atitinkamos vaidmenimis pagrįstos administravimo kontrolės (RBAC) teisės intune vaidmenų ašmenys.</span><span class="sxs-lookup"><span data-stu-id="a8f30-106">Verify that you have been assigned the appropriate role-based administration control (RBAC) permissions in the Intune roles blade.</span></span>
- <span data-ttu-id="a8f30-107">Patikrinkite, ar naudojama grupė nėra siuntimo sąrašas.</span><span class="sxs-lookup"><span data-stu-id="a8f30-107">Verify the group used is not a distribution list.</span></span> <span data-ttu-id="a8f30-108">Intune Azure portalas palaiko tik vartotojų abonementus, kurie priklauso Azure Active Directory saugos grupes.</span><span class="sxs-lookup"><span data-stu-id="a8f30-108">Intune in the Azure portal only supports user accounts that belong to Azure Active Directory security groups.</span></span> <span data-ttu-id="a8f30-109">Peržiūrėkite savo grupes "Azure" portale > **"Intune**  >  **Groups"** arba "Azure" portale > **"Azure Active Directory".**</span><span class="sxs-lookup"><span data-stu-id="a8f30-109">Review your groups in the Azure portal > **Intune** > **Groups**, or in Azure portal > **Azure Active Directory**.</span></span>

<span data-ttu-id="a8f30-110">**Vartotojas turi per daug priskirtų intune vaidmens teisių**</span><span class="sxs-lookup"><span data-stu-id="a8f30-110">**User has too many permissions for assigned Intune role**</span></span>

<span data-ttu-id="a8f30-111">Patarkite vartotojui eiti į **Intune**  >  **Intune vaidmenis**  >  **Mano teisės**  >  **Eksportuoti,** kad peržiūrėtumėte suteiktas teises.</span><span class="sxs-lookup"><span data-stu-id="a8f30-111">Advise the user to go to **Intune** > **Intune roles** > **My permissions** > **Export** to review granted permissions.</span></span>

<span data-ttu-id="a8f30-112">**Į vaidmenį įtraukiau aprėpties grupę, bet to vaidmens vartotojai vis dar mato kitus vartotojus arba įrenginius.**</span><span class="sxs-lookup"><span data-stu-id="a8f30-112">**I added a scope group to a role, but users in that role still see other users or devices.**</span></span>

<span data-ttu-id="a8f30-113">Aprėpties grupės neišfiltruoja vartotojų arba įrenginių.</span><span class="sxs-lookup"><span data-stu-id="a8f30-113">Scope groups do not filter out users or devices.</span></span> <span data-ttu-id="a8f30-114">Aprėpties grupės:</span><span class="sxs-lookup"><span data-stu-id="a8f30-114">Scope groups:</span></span>

- <span data-ttu-id="a8f30-115">Apribokite, kam vartotojai gali priskirti strategijas arba programas.</span><span class="sxs-lookup"><span data-stu-id="a8f30-115">Limit who users can assign policies or applications to.</span></span>
- <span data-ttu-id="a8f30-116">Leisti tik konkretiems vartotojams vykdyti nuotolines užduotis įrenginiuose.</span><span class="sxs-lookup"><span data-stu-id="a8f30-116">Allow only specific users to run remote tasks on devices.</span></span>

<span data-ttu-id="a8f30-117">Daugiau informacijos apie aprėpties grupes ieškokite [Vaidmenimis pagrįstas prieigos valdymas (RBAC) su "Microsoft Intune".](https://docs.microsoft.com/intune/role-based-access-control)</span><span class="sxs-lookup"><span data-stu-id="a8f30-117">For more information about scope groups, see  [Role-based access control (RBAC) with Microsoft Intune](https://docs.microsoft.com/intune/role-based-access-control).</span></span>

<span data-ttu-id="a8f30-118">**Aš pridėjo vartotoją Intune vaidmenį, bet jie vis dar turi visišką prieigą prie Intune admin konsolės.**</span><span class="sxs-lookup"><span data-stu-id="a8f30-118">**I added a user to an Intune role but they still have full access to the Intune admin console.**</span></span>

<span data-ttu-id="a8f30-119">Eikite į Intune > **vartotojai** Azure portalas ir patikrinkite, ar vartotojas nėra priskirtas bet kurį iš šių vaidmenų Azure portalas:</span><span class="sxs-lookup"><span data-stu-id="a8f30-119">Navigate to Intune > **Users** in the Azure portal and verify that the user is not assigned to any of the following roles in the Azure portal:</span></span>

- <span data-ttu-id="a8f30-120">Visuotinis administratorius</span><span class="sxs-lookup"><span data-stu-id="a8f30-120">Global administrator</span></span>
- <span data-ttu-id="a8f30-121">Intune tarnybos administratorius</span><span class="sxs-lookup"><span data-stu-id="a8f30-121">Intune service administrator</span></span>
- <span data-ttu-id="a8f30-122">"SharePoint" administratorius</span><span class="sxs-lookup"><span data-stu-id="a8f30-122">SharePoint administrator</span></span>

<span data-ttu-id="a8f30-123">Daugiau informacijos ieškokite [Vaidmenimis pagrįstas prieigos valdymas (RBAC) su "Microsoft Intune".](https://docs.microsoft.com/intune/role-based-access-control)</span><span class="sxs-lookup"><span data-stu-id="a8f30-123">For more info, see [Role-based access control (RBAC) with Microsoft Intune](https://docs.microsoft.com/intune/role-based-access-control).</span></span>

<span data-ttu-id="a8f30-124">**Prieigos problemos**</span><span class="sxs-lookup"><span data-stu-id="a8f30-124">**Access Issues**</span></span>

<span data-ttu-id="a8f30-125">Daugiau informacijos rasite [Negalite prisijungti prie "Office 365", "Azure" arba "Intune".](https://support.microsoft.com/help/2412085/you-can-t-sign-in-to-office-365-azure-or-intune)</span><span class="sxs-lookup"><span data-stu-id="a8f30-125">For more info, see [You can't sign in to Office 365, Azure, or Intune](https://support.microsoft.com/help/2412085/you-can-t-sign-in-to-office-365-azure-or-intune).</span></span>