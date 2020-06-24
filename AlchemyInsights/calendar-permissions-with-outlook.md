---
title: Kalendoriaus teisės
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3800009"
- "611"
ms.openlocfilehash: 78f27014c60badc801212177dd455ef2a0de5a9e
ms.sourcegitcommit: 722e9a0ed058cb1eab2dd053be2418b60f7d4aac
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 06/23/2020
ms.locfileid: "44862174"
---
# <a name="calendar-permissions"></a><span data-ttu-id="2332f-102">Kalendoriaus teisės</span><span class="sxs-lookup"><span data-stu-id="2332f-102">Calendar Permissions</span></span>

<span data-ttu-id="2332f-103">Vartotojai gali pakeisti savo kalendoriaus teises naudodami "Outlook" žiniatinklyje ar kituose klientuose, bet kaip administratorius, kurį taip pat gali reikėti ištirti.</span><span class="sxs-lookup"><span data-stu-id="2332f-103">Users can change their own Calendar Permissions with Outlook on the Web or other clients, but as an admin you may need to investigate as well.</span></span>  
<span data-ttu-id="2332f-104">Su "Exchange PowerShell" cmdlet parodys vartotojo kalendoriaus teises:</span><span class="sxs-lookup"><span data-stu-id="2332f-104">With Exchange PowerShell cmdlet will show you the permission on a user’s calendar:</span></span>

`Get-MailboxFolderPermission <SMTPAddress>:\Calendar | FT -a`

<span data-ttu-id="2332f-105">Norėdami pamatyti daugiau informacijos, žr.:</span><span class="sxs-lookup"><span data-stu-id="2332f-105">To see more information see the following:</span></span>

- [<span data-ttu-id="2332f-106">Get-MailboxFolderPermission (Get-MailboxFolderPermission)</span><span class="sxs-lookup"><span data-stu-id="2332f-106">Get-MailboxFolderPermission</span></span>](https://docs.microsoft.com/powershell/module/exchange/get-mailboxfolderpermission?view=exchange-ps)

- [<span data-ttu-id="2332f-107">Set-MailboxFolderPermission Set-MailboxFolderPermission Nustatyti MailboxFolderPermission</span><span class="sxs-lookup"><span data-stu-id="2332f-107">Set-MailboxFolderPermission</span></span>](https://docs.microsoft.com/powershell/module/exchange/set-mailboxfolderpermission?view=exchange-ps)

- [<span data-ttu-id="2332f-108">Pridėti MailboxFolderPermission</span><span class="sxs-lookup"><span data-stu-id="2332f-108">Add-MailboxFolderPermission</span></span>](https://office.visualstudio.com/DefaultCollection/MAX/_queries/query/Add-MailboxFolderPermission)

<span data-ttu-id="2332f-109">Kalendoriaus teisės naudojamos bendrinant kalendorius, norint pamatyti daugiau informacijos apie "Outlook" kalendoriaus bendrinimą, žr.</span><span class="sxs-lookup"><span data-stu-id="2332f-109">Calendar Permissions are used in the sharing of calendars, to see more information about sharing an Outlook calendar, see these articles:</span></span>

- [<span data-ttu-id="2332f-110">„Outlook“ kalendoriaus bendrinimas su kitais žmonėmis</span><span class="sxs-lookup"><span data-stu-id="2332f-110">Share an Outlook calendar with other people</span></span>](https://support.office.com/article/353ed2c1-3ec5-449d-8c73-6931a0adab88)
- [<span data-ttu-id="2332f-111">Kalendoriaus bendrinimas internetinėje "Outlook" verslui</span><span class="sxs-lookup"><span data-stu-id="2332f-111">Share your calendar in Outlook on the web for business</span></span>](https://support.office.com/article/7ecef8ae-139c-40d9-bae2-a23977ee58d5)

<span data-ttu-id="2332f-112">Norėdami pašalinti kalendoriaus teisių triktis, galite naudoti [palaikymo ir atkūrimo asistento](https://support.microsoft.com/office/e90bb691-c2a7-4697-a94f-88836856c72f) įrankį.</span><span class="sxs-lookup"><span data-stu-id="2332f-112">To troubleshoot Calendar Permission you can use the [Support and Recovery Assistant](https://support.microsoft.com/office/e90bb691-c2a7-4697-a94f-88836856c72f) tool.</span></span>