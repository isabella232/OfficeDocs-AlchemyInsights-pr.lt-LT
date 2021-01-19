---
title: Šalinti savininko triktis
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/16/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7815"
- "9004358"
ms.openlocfilehash: 914d5682a403197a8569bb75fda8a77449f485f6
ms.sourcegitcommit: 6d02eb533fd74199af6b20f714b3720991da2c4a
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 01/18/2021
ms.locfileid: "49901001"
---
# <a name="troubleshoot-owner-issues"></a><span data-ttu-id="7de3a-102">Šalinti savininko triktis</span><span class="sxs-lookup"><span data-stu-id="7de3a-102">Troubleshoot owner issues</span></span>

<span data-ttu-id="7de3a-103">Norėdami pašalinti su savininku susijusias problemas, atlikite šiuos veiksmus:</span><span class="sxs-lookup"><span data-stu-id="7de3a-103">To troubleshoot owner-related issues, perform the following steps:</span></span>

1. <span data-ttu-id="7de3a-104">[Įtraukite arba keiskite "Azure" prenumeratos administratorių](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-accessmanagement-managing-group-owners): "Azure Active Directory" ("Azure AD") grupės priklauso ir jas tvarko grupės savininkai.</span><span class="sxs-lookup"><span data-stu-id="7de3a-104">[Add or change Azure subscription administrators](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-accessmanagement-managing-group-owners): Azure Active Directory (Azure AD) groups are owned and managed by group owners.</span></span> <span data-ttu-id="7de3a-105">Grupės savininkai gali būti vartotojai arba paslaugų principai ir gali valdyti grupę, įskaitant narystę.</span><span class="sxs-lookup"><span data-stu-id="7de3a-105">Group owners can be users or service principals, and are able to manage the group, including membership.</span></span> <span data-ttu-id="7de3a-106">Grupės savininkai gali priskirti tik esamus grupės savininkus arba grupės valdymo administratorius.</span><span class="sxs-lookup"><span data-stu-id="7de3a-106">Only existing group owners or group-managing administrators can assign group owners.</span></span> <span data-ttu-id="7de3a-107">Grupės savininkai neprivalo būti grupės nariais.</span><span class="sxs-lookup"><span data-stu-id="7de3a-107">Group owners aren't required to be members of the group.</span></span>
2. <span data-ttu-id="7de3a-108">" [Azure" prenumeratos administratorių įtraukimas arba keitimas](https://docs.microsoft.com/azure/cost-management-billing/manage/add-change-subscription-administrator): šiame straipsnyje aprašyta, kaip įtraukti arba pakeisti vartotojo administratoriaus vaidmenį naudojant "AZURE RBAC" prenumeratos aprėptį.</span><span class="sxs-lookup"><span data-stu-id="7de3a-108">[Add or change Azure subscription administrators](https://docs.microsoft.com/azure/cost-management-billing/manage/add-change-subscription-administrator): This article describes how to add or change the administrator role for a user using Azure RBAC at the subscription scope.</span></span>
3. <span data-ttu-id="7de3a-109">Naudokite "PowerShell", kad įtrauktumėte grupės savininką arba programos savininką.</span><span class="sxs-lookup"><span data-stu-id="7de3a-109">Use PowerShell to add a group owner or an application owner.</span></span>
