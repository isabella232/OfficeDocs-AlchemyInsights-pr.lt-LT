---
title: Grupės strategija
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8303"
- "9003234"
ms.openlocfilehash: a829a78bbe947300b6dabb9fdb36088c17809742
ms.sourcegitcommit: 6900c2b7208ca51a9873dfc2e00be6f66cb25e3c
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 02/15/2021
ms.locfileid: "50256781"
---
# <a name="group-policy"></a><span data-ttu-id="86e6e-102">Grupės strategija</span><span class="sxs-lookup"><span data-stu-id="86e6e-102">Group policy</span></span>

<span data-ttu-id="86e6e-103">Vartotojo ir kompiuterio objektų "Azure Active Directory" domenų tarnybos ("Azure AD DS") parametrai dažnai valdomi naudojant grupės strategijos objektus (GPO).</span><span class="sxs-lookup"><span data-stu-id="86e6e-103">Settings for user and computer objects in Azure Active Directory Domain Services (Azure AD DS) are often managed using Group Policy Objects (GPOs).</span></span> <span data-ttu-id="86e6e-104">"Azure AD DS" yra įtaisytosios GPOs, skirtos "AADDC" vartotojams ir "AADDC" kompiuterių konteineriams.</span><span class="sxs-lookup"><span data-stu-id="86e6e-104">Azure AD DS includes built-in GPOs for the AADDC Users and AADDC Computers containers.</span></span> <span data-ttu-id="86e6e-105">Galite tinkinti šiuos įtaisytuosius GPO, kad sukonfigūruotumėte grupės strategiją, kaip reikia jūsų aplinkai.</span><span class="sxs-lookup"><span data-stu-id="86e6e-105">You can customize these built-in GPOs to configure group policy as needed for your environment.</span></span> <span data-ttu-id="86e6e-106">"Azure AD DC" administratorių grupės nariai turi grupės strategijos administravimo teises "Azure AD DS" domene ir taip pat gali kurti pasirinktinio GPOs ir organizacijos vienetus (OUs).</span><span class="sxs-lookup"><span data-stu-id="86e6e-106">Members of the Azure AD DC administrators group have group policy administration privileges in the Azure AD DS domain, and can also create custom GPOs and organizational units (OUs).</span></span> <span data-ttu-id="86e6e-107">Daugiau informacijos apie grupės strategiją ir jos veikimą rasite [grupės strategijos apžvalga](https://docs.microsoft.com/previous-versions/windows/it-pro/windows-server-2012-R2-and-2012/hh831791(v=ws.11)).</span><span class="sxs-lookup"><span data-stu-id="86e6e-107">For more information on what group policy is and how it works, see [Group Policy overview](https://docs.microsoft.com/previous-versions/windows/it-pro/windows-server-2012-R2-and-2012/hh831791(v=ws.11)).</span></span>

<span data-ttu-id="86e6e-108">Hibridinėje aplinkoje grupės strategijos sukonfigūruotos vietinėje AD DS aplinkoje nesinchronizuojamos su "Azure AD DS".</span><span class="sxs-lookup"><span data-stu-id="86e6e-108">In a hybrid environment, group policies configured in an on-premises AD DS environment aren't synchronized to Azure AD DS.</span></span> <span data-ttu-id="86e6e-109">Norėdami apibrėžti "Azure AD DS" vartotojų arba kompiuterių konfigūracijos parametrus, redaguokite vieną iš numatytųjų GPO arba sukurkite pasirinktinę GPO.</span><span class="sxs-lookup"><span data-stu-id="86e6e-109">To define configuration settings for users or computers in Azure AD DS, edit one of the default GPOs or create a custom GPO.</span></span>

<span data-ttu-id="86e6e-110">Šiame straipsnyje [valdoma grupės strategija](https://docs.microsoft.com/azure/active-directory-domain-services/manage-group-policy) rodoma, kaip įdiegti grupės strategijos valdymo įrankius, kaip ton redaguoti įtaisytuosius GPO ir kurti pasirinktinio GPOs.</span><span class="sxs-lookup"><span data-stu-id="86e6e-110">This article [Manage Group Policy](https://docs.microsoft.com/azure/active-directory-domain-services/manage-group-policy) shows you how to install the Group Policy Management tools, how ton edit the built-in GPOs, and how to create custom GPOs.</span></span>



