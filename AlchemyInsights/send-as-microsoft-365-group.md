---
title: "\"Microsoft 365\" grupės siuntimas"
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/19/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003200"
ms.openlocfilehash: cfb4bd5ce59eeccdd0812d013b8a444aebeb1d4c
ms.sourcegitcommit: 9818d3c8e6b10f23244e51286e2463caf48fffd5
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 08/21/2020
ms.locfileid: "46871970"
---
# <a name="send-as-microsoft-365-group"></a><span data-ttu-id="aa6af-102">"Microsoft 365" grupės siuntimas</span><span class="sxs-lookup"><span data-stu-id="aa6af-102">Send As Microsoft 365 group</span></span>

<span data-ttu-id="aa6af-103">Galite priskirti siųsti kaip teises, kad konkretūs vartotojai galėtų siųsti laišką kaip "Microsoft 365" grupę:</span><span class="sxs-lookup"><span data-stu-id="aa6af-103">You can assign Send As permissions to allow specific users to send messages as a Microsoft 365 group:</span></span>  

1. <span data-ttu-id="aa6af-104">Prisijungimas prie "Exchange Online" "PowerShell".</span><span class="sxs-lookup"><span data-stu-id="aa6af-104">Connect to Exchange Online PowerShell.</span></span>  

2. <span data-ttu-id="aa6af-105">Vykdykite toliau nurodytą komandą.</span><span class="sxs-lookup"><span data-stu-id="aa6af-105">Run the following command:</span></span>  

    <span data-ttu-id="aa6af-106">Pridėti-RecipientPermission `<GroupName>` -patikėtinis `<MailboxName>` – prieigos teisės SendAs</span><span class="sxs-lookup"><span data-stu-id="aa6af-106">Add-RecipientPermission `<GroupName>` -Trustee `<MailboxName>` -AccessRights SendAs</span></span>

<span data-ttu-id="aa6af-107">Daugiau informacijos ieškokite skyriuje [leisti nariams išsiųsti kaip arba nusiųsti grupės vardu](https://docs.microsoft.com/microsoft-365/admin/create-groups/allow-members-to-send-as-or-send-on-behalf-of-group?view=o365-worldwide).</span><span class="sxs-lookup"><span data-stu-id="aa6af-107">For more information, see [Allow members to send as or send on behalf of a group](https://docs.microsoft.com/microsoft-365/admin/create-groups/allow-members-to-send-as-or-send-on-behalf-of-group?view=o365-worldwide).</span></span>