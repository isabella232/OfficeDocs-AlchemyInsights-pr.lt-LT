---
title: 'RBAC vaidmenys '
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003230"
- "7265"
ms.openlocfilehash: 7c4c9d1a76f395dfb2f831d555199b76c354ca57
ms.sourcegitcommit: 2e4a5153e530bf15744a52e982eeb0d99757e9d2
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 12/04/2020
ms.locfileid: "49583946"
---
# <a name="rbac-rules"></a><span data-ttu-id="50438-102">RBAC taisyklės</span><span class="sxs-lookup"><span data-stu-id="50438-102">RBAC rules</span></span>

<span data-ttu-id="50438-103">Jei gaunate teisių klaidą:</span><span class="sxs-lookup"><span data-stu-id="50438-103">If you get the permission error:</span></span> 

- <span data-ttu-id="50438-104">**Klientas su objekto ID neturi leidimo atlikti veiksmą per aprėptį (kodas: autorizacija nepavyko)**: kai bandote sukurti išteklių, patikrinkite, ar šiuo metu esate prisijungę su vartotoju, kuriam priskirtas tam tikrą vaidmenį turintis vartotojas, kuriam buvo suteikta teisė naudoti išteklius pasirinktoje srityje.</span><span class="sxs-lookup"><span data-stu-id="50438-104">**The client with object id does not have authorization to perform action over scope (code: AuthorizationFailed)**: when you try to create a resource, check that you are currently signed in with a user that is assigned a role that has write permission to the resource at the selected scope.</span></span> <span data-ttu-id="50438-105">Pavyzdžiui, norėdami valdyti virtualiąsias mašinas išteklių grupėje, turite turėti [virtualiosios mašinos bendraautoriaus](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support#virtual-machine-contributor) vaidmenį išteklių grupėje (arba pirminėje aprėptyje).</span><span class="sxs-lookup"><span data-stu-id="50438-105">For example, to manage virtual machines in a resource group, you should have the [Virtual Machine Contributor](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support#virtual-machine-contributor) role on the resource group (or parent scope).</span></span> <span data-ttu-id="50438-106">Kiekvieno įtaisytojo vaidmens teisių sąrašo ieškokite [Įtaisytieji "Azure" išteklių vaidmenys](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support).</span><span class="sxs-lookup"><span data-stu-id="50438-106">For a list of the permissions for each built-in role, see [Built-in roles for Azure resources](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>
- <span data-ttu-id="50438-107">Neturite **teisės sukurti palaikymo užklausos**: kai bandote sukurti arba atnaujinti palaikymo bilietą, patikrinkite, ar šiuo metu esate prisijungę naudodami vartotoją, kuriam priskirtas "Microsoft". support/Paramttickets/rašyti teises, pvz., [palaikymo užklausos bendraautorius](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support#support-request-contributor).</span><span class="sxs-lookup"><span data-stu-id="50438-107">**You don't have permission to create a support request**: when you try to create or update a support ticket, check that you are currently signed in with a user that is assigned a role that has the Microsoft.Support/supportTickets/write permission, such as [Support Request Contributor](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support#support-request-contributor).</span></span>
- <span data-ttu-id="50438-108">Negalima **kurti daugiau vaidmenų priskyrimų (kodas: Roleassigmentlimitviršyta)**: kai bandote priskirti vaidmenį, pabandykite sumažinti vaidmenų priskyrimų skaičių priskirdami vaidmenis grupėms, o ne.</span><span class="sxs-lookup"><span data-stu-id="50438-108">**No more role assignments can be created (code: RoleAssignmentLimitExceeded)**: when you try to assign a role, try to reduce the number of role assignments by assigning roles to groups instead.</span></span> <span data-ttu-id="50438-109">"Azure" palaiko iki **2000** vaidmenų priskyrimus per produktų paketą.</span><span class="sxs-lookup"><span data-stu-id="50438-109">Azure supports up to **2000** role assignments per subscription.</span></span>

<span data-ttu-id="50438-110">Daugiau informacijos apie "Azure RBAC" vaidmenis ieškokite " [AZURE RBAC" vaidmenys](https://docs.microsoft.com/azure/role-based-access-control/role-assignments-portal?WT.mc_id=Portal-Microsoft_Azure_Support).</span><span class="sxs-lookup"><span data-stu-id="50438-110">For more details on Azure RBAC roles, see [Azure RBAC roles](https://docs.microsoft.com/azure/role-based-access-control/role-assignments-portal?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>
