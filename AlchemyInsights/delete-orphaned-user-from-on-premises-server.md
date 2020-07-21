---
title: Naikinti pavienį vartotoją iš vietinio serverio
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/20/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1725"
- "9000179"
ms.openlocfilehash: 7927c0684d2f5289f92506d7d05d5b1a3b43b658
ms.sourcegitcommit: b0b050a83db28566b68e3ec09810c6b94280008e
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 07/20/2020
ms.locfileid: "45198180"
---
# <a name="delete-orphaned-user-from-on-premises-server"></a><span data-ttu-id="aa847-102">Naikinti pavienį vartotoją iš vietinio serverio</span><span class="sxs-lookup"><span data-stu-id="aa847-102">Delete orphaned user from on-premises server</span></span>

<span data-ttu-id="aa847-103">Norėdami pašalinti pavienį vartotoją, atlikite šiuos veiksmus:</span><span class="sxs-lookup"><span data-stu-id="aa847-103">To remove an orphaned user, follow these steps:</span></span>

1. <span data-ttu-id="aa847-104">Priversti katalogų sinchronizavimas vadovaudamiesi instrukcijomis [Kas yra hibridinė tapatybė su Azure Active Directory?](https://technet.microsoft.com/library/jj151771.aspx#bkmk_synchronizedirectories).</span><span class="sxs-lookup"><span data-stu-id="aa847-104">Force directory synchronization by following the instructions in [What is hybrid identity with Azure Active Directory?](https://technet.microsoft.com/library/jj151771.aspx#bkmk_synchronizedirectories).</span></span>

2. <span data-ttu-id="aa847-105">Norėdami patikrinti katalogų sinchronizavimą, peržiūrėkite [Kas yra hibridinė tapatybė su Azure Active Directory?](https://technet.microsoft.com/library/jj151797.aspx).</span><span class="sxs-lookup"><span data-stu-id="aa847-105">To verify directory synchronization, see [What is hybrid identity with Azure Active Directory?](https://technet.microsoft.com/library/jj151797.aspx).</span></span>

3. <span data-ttu-id="aa847-106">Jei sinchronizavimas veikia tinkamai, bet Active Directory objekto naikinimas nėra platinti Azure AD, rankiniu būdu pašalinti pavienių objektą naudodami vieną iš šių Azure Active Directory modulis, skirtas "Windows PowerShell" cmdlet:</span><span class="sxs-lookup"><span data-stu-id="aa847-106">If sync functions correctly but the Active Directory object deletion does not propagate to Azure AD, manually remove the orphaned object by using one of the following Azure Active Directory Module for Windows PowerShell cmdlets:</span></span>

    <span data-ttu-id="aa847-107">Pašalinti-MsolKontaktas</span><span class="sxs-lookup"><span data-stu-id="aa847-107">Remove-MsolContact</span></span>  
    <span data-ttu-id="aa847-108">Šalinti MsolGroup</span><span class="sxs-lookup"><span data-stu-id="aa847-108">Remove-MsolGroup</span></span>  
    <span data-ttu-id="aa847-109">Pašalinti MsolUser</span><span class="sxs-lookup"><span data-stu-id="aa847-109">Remove-MsolUser</span></span>

    <span data-ttu-id="aa847-110">Pvz., norėdami pašalinti našlaičiai vartotojo ID john.smith@contoso.com, iš pradžių sukurtas naudojant katalogų sinchronizavimą, vykdykite cmdlet:</span><span class="sxs-lookup"><span data-stu-id="aa847-110">For example, to remove orphaned user ID john.smith@contoso.com, originally created by using directory synchronization, run the cmdlet:</span></span>

    <span data-ttu-id="aa847-111">Pašalinti MsolUser –UserPrincipalName John.Smith@Contoso.com</span><span class="sxs-lookup"><span data-stu-id="aa847-111">Remove-MsolUser –UserPrincipalName John.Smith@Contoso.com</span></span>