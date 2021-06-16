---
title: "\"Active Directory\" nesinchronizuojama"
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001688"
- "1300023"
- "3754"
- "4531"
ms.openlocfilehash: 0da512379e5a2f6ccb773e18c465e545c0660560
ms.sourcegitcommit: e42bb24c9bae1d0df8c49c424d2aa5e7466703ac
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 06/14/2021
ms.locfileid: "52930983"
---
# <a name="active-directory-not-syncing"></a><span data-ttu-id="72baf-102">"Active Directory" nesinchronizuojama</span><span class="sxs-lookup"><span data-stu-id="72baf-102">Active Directory not syncing</span></span>

<span data-ttu-id="72baf-103">Jei gaunate sinchronizavimo klaidų, pvz., "nėra naujausio sinchronizavimo", arba pastebėjote katalogų sinchronizavimo būseną "Office" administravimo portale sako: "Paskutinį kartą sinchronizuota daugiau nei prieš 3 dienas", gali būti, kad "AADConnect" turi neteisingus parametrus arba nepakankamas teises atlikti sinchronizavimą.</span><span class="sxs-lookup"><span data-stu-id="72baf-103">If you are receiving synchronization errors, such as "no recent synchronization," or notice the directory synchronization status in the Office admin portal says, "Last synced more than 3 days ago," it may be that AADConnect has incorrect settings or insufficient permissions to perform a synchronization.</span></span>  

<span data-ttu-id="72baf-104">"AADConnect" diegimas iš naujo naudojant skubius parametrus gali greitai išspręsti šią problemą:</span><span class="sxs-lookup"><span data-stu-id="72baf-104">Reinstalling AADConnect by using express settings might resolve the issue quickly:</span></span>

1. <span data-ttu-id="72baf-105">[Atsisiųskite naujausią "AADConnect" versiją.](https://go.microsoft.com/fwlink/?LinkId=615771)</span><span class="sxs-lookup"><span data-stu-id="72baf-105">[Download the latest version of AADConnect](https://go.microsoft.com/fwlink/?LinkId=615771).</span></span>

2. <span data-ttu-id="72baf-106">[Vykdykite nurodymus, kaip atlikti skubią įdiegtį.](/azure/active-directory/hybrid/how-to-connect-install-express)</span><span class="sxs-lookup"><span data-stu-id="72baf-106">[Follow the instructions for express installation](/azure/active-directory/hybrid/how-to-connect-install-express).</span></span>

<span data-ttu-id="72baf-107">„Azure AD Connect“ turi būti diegiama „Windows Server 2012“ arba naujesnėje versijoje.</span><span class="sxs-lookup"><span data-stu-id="72baf-107">Azure AD Connect must be installed on Windows Server 2012 or later.</span></span> <span data-ttu-id="72baf-108">Šis serveris turi būti prijungtas prie domeno ir gali būti domeno valdiklis arba nario serveris.</span><span class="sxs-lookup"><span data-stu-id="72baf-108">This server must be domain joined and may be a domain controller or a member server.</span></span> <span data-ttu-id="72baf-109">Visą "Azure AD" reikalavimų ir Prisijungimas sąrašą, peržiūrėkite [Būtinosios "Azure AD" Prisijungimas.](/azure/active-directory/hybrid/how-to-connect-install-prerequisites)</span><span class="sxs-lookup"><span data-stu-id="72baf-109">For a full list of Azure AD Connect requirements and pre-requisites, review [Prerequisites for Azure AD Connect](/azure/active-directory/hybrid/how-to-connect-install-prerequisites).</span></span>

<span data-ttu-id="72baf-110">Daugiau informacijos apie "AADConnect" tarnybos paskyras žr. ["Azure AD Prisijungimas: Paskyros ir teisės](/azure/active-directory/hybrid/reference-connect-accounts-permissions).</span><span class="sxs-lookup"><span data-stu-id="72baf-110">For more information about AADConnect service accounts, see [Azure AD Connect: Accounts and permissions](/azure/active-directory/hybrid/reference-connect-accounts-permissions).</span></span>
