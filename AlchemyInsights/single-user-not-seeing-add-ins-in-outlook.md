---
title: Vienas vartotojas nemato papildinių programoje "Outlook"
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/16/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: ''
ms.openlocfilehash: 1f547c3f593b3256bd44f518aacbc36ed1c4c848
ms.sourcegitcommit: a05276bd623466ad211e1f8d9f0c616672dd3640
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 07/16/2020
ms.locfileid: "45197964"
---
# <a name="single-user-not-seeing-add-ins-in-outlook"></a><span data-ttu-id="8dcc8-102">Vienas vartotojas nemato papildinių programoje "Outlook"</span><span class="sxs-lookup"><span data-stu-id="8dcc8-102">Single user not seeing add-ins in Outlook</span></span>

<span data-ttu-id="8dcc8-103">Vartotojas gali būti vaidmens, kuris neturi tinkamo parametro AppsForOfficeEnabled, dalis.</span><span class="sxs-lookup"><span data-stu-id="8dcc8-103">The user might be part of a role that doesn’t have the correct AppsForOfficeEnabled parameter.</span></span> <span data-ttu-id="8dcc8-104">Vykdykite šį cmdlet, kad sužinotumėte, ar su vartotoju susietas teisingas vaidmuo:</span><span class="sxs-lookup"><span data-stu-id="8dcc8-104">Run this cmdlet to find out if the correct role is associated with the user:</span></span>

<span data-ttu-id="8dcc8-105">Get-ManagementRoleAssignment -RoleAssignee user@domain.com-Delegavimas $false | Formatuoti lentelę – automatinis vaidmuo,RoleAssigneeName,RoleAssigneeType</span><span class="sxs-lookup"><span data-stu-id="8dcc8-105">Get-ManagementRoleAssignment -RoleAssignee user@domain.com -Delegating $false | Format-Table -Auto Role,RoleAssigneeName,RoleAssigneeType</span></span>

<span data-ttu-id="8dcc8-106">Daugiau informacijos [ieškokite Administratorių ir vartotojų, kurie gali įdiegti ir tvarkyti "Outlook" papildinius, nurodymas.](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins)</span><span class="sxs-lookup"><span data-stu-id="8dcc8-106">For more info, see [Specify the administrators and users who can install and manage add-ins for Outlook](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins).</span></span>
