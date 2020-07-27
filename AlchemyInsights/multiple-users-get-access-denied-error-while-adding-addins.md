---
title: Keli vartotojai gauna "Access Denied" klaidą, kai pridedate papildinius programoje "Outlook"
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/23/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5892"
- "6700008"
ms.openlocfilehash: 624d880c535b7d8888b676ff23c774c6d138a75a
ms.sourcegitcommit: 07e56267dedfc4cec1143072c791670cbf81186b
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 07/24/2020
ms.locfileid: "45424168"
---
# <a name="multiple-users-get-access-denied-error-while-adding-add-ins-in-outlook"></a><span data-ttu-id="83dfb-102">Keli vartotojai gauna "Access Denied" klaidą, kai pridedate papildinius programoje "Outlook"</span><span class="sxs-lookup"><span data-stu-id="83dfb-102">Multiple users get Access Denied error while adding add-ins in Outlook</span></span>

<span data-ttu-id="83dfb-103">Galite nurodyti, kurie jūsų organizacijos administratoriai turi teisę diegti ir tvarkyti "Outlook" priedus.</span><span class="sxs-lookup"><span data-stu-id="83dfb-103">You can specify which administrators in your organization have permissions to install and manage add-ins for Outlook.</span></span> <span data-ttu-id="83dfb-104">Taip pat galite nurodyti, kurie jūsų organizacijos vartotojai turi teisę diegti ir valdyti priedus savo reikmėms.</span><span class="sxs-lookup"><span data-stu-id="83dfb-104">You can also specify which users in your organization have permission to install and manage add-ins for their own use.</span></span>

<span data-ttu-id="83dfb-105">Daugiau informacijos [ieškokite Administratorių ir vartotojų, kurie gali įdiegti ir tvarkyti "Outlook" papildinius, nurodymas.](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins)</span><span class="sxs-lookup"><span data-stu-id="83dfb-105">For details, see [Specify the administrators and users who can install and manage add-ins for Outlook](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins).</span></span>

<span data-ttu-id="83dfb-106">Norėdami patikrinti, ar sėkmingai priskyrėte vartotojo teises, pakeiskite <Role Name> vaidmens, kurį norite patikrinti, pavadinimu ir vykdykite šią komandą "Exchange Online PowerShell":</span><span class="sxs-lookup"><span data-stu-id="83dfb-106">To verify that you've successfully assigned permissions for a user, replace <Role Name> with the name of the role to verify, and run the following command in Exchange Online PowerShell:</span></span>

<span data-ttu-id="83dfb-107">Get-ManagementRoleAssignment -Vaidmuo <Role Name> " " -GetEffectiveUsers</span><span class="sxs-lookup"><span data-stu-id="83dfb-107">Get-ManagementRoleAssignment -Role "<Role Name>" -GetEffectiveUsers</span></span>

<span data-ttu-id="83dfb-108">Šiame pavyzdyje parodyta, kaip patikrinti, kam priskyrėte teises diegti priedus iš organizacijos "Office" parduotuvės.</span><span class="sxs-lookup"><span data-stu-id="83dfb-108">This example shows you how to verify whom you've assigned permissions to install add-ins from the Office Store for the organization.</span></span>

<span data-ttu-id="83dfb-109">Powershell</span><span class="sxs-lookup"><span data-stu-id="83dfb-109">PowerShell</span></span>

<span data-ttu-id="83dfb-110">-Vaidmuo "Org Marketplace Apps" -GetEffectiveUsers</span><span class="sxs-lookup"><span data-stu-id="83dfb-110">-Role "Org Marketplace Apps" -GetEffectiveUsers</span></span>

<span data-ttu-id="83dfb-111">Rezultatuose, Get-ManagementRoleAssignment, peržiūrėkite įrašus efektyvus vartotojai stulpelyje.</span><span class="sxs-lookup"><span data-stu-id="83dfb-111">In the results, Get-ManagementRoleAssignment, review the entries in the Effective Users column.</span></span>

<span data-ttu-id="83dfb-112">Išsamesnės sintaksės ir parametrų informacijos ieškokite [Get-ManagementRoleAssignment](https://docs.microsoft.com/powershell/module/exchange/get-managementroleassignment).</span><span class="sxs-lookup"><span data-stu-id="83dfb-112">For detailed syntax and parameter information, see [Get-ManagementRoleAssignment](https://docs.microsoft.com/powershell/module/exchange/get-managementroleassignment).</span></span>
 