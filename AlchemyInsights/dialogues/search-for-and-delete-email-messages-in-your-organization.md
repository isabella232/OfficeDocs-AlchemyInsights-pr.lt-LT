---
title: Savo organizacijos el. laiškų ieška ir naikinimas
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000260"
- "7257"
ms.openlocfilehash: e935b10083459b81fc58e12bb59c9511defefa6d
ms.sourcegitcommit: 78fe9f33438cb0c19f0dab31253b5853b73f4f47
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 03/05/2021
ms.locfileid: "50525435"
---
# <a name="search-for-and-delete-email-messages-in-your-organization"></a><span data-ttu-id="3ab41-102">Savo organizacijos el. laiškų ieška ir naikinimas</span><span class="sxs-lookup"><span data-stu-id="3ab41-102">Search for and delete email messages in your organization</span></span>

<span data-ttu-id="3ab41-103">Atlikite šiuos veiksmus:</span><span class="sxs-lookup"><span data-stu-id="3ab41-103">Follow these steps:</span></span>

1. <span data-ttu-id="3ab41-104">Jei nesate visuotinis administratorius, norėdami ieškoti pranešimo, jūsų abonementas turi būti įtrauktas į " **e" aptikimo tvarkytuvo vaidmenų grupę** arba **atitikties ieškos valdymo vaidmenį**.</span><span class="sxs-lookup"><span data-stu-id="3ab41-104">If you're not a global admin, to search for messages your account must be added to the **eDiscovery Manager role group** or **Compliance Search management role**.</span></span> <span data-ttu-id="3ab41-105">Norėdami panaikinti laišką, turite prisijungti prie **organizacijos valdymo vaidmenų grupės** arba **ieškos ir valymo valdymo vaidmens**.</span><span class="sxs-lookup"><span data-stu-id="3ab41-105">To delete messages, you'll need to join the **Organization Management role group** or the **Search and Purge management role**.</span></span> <span data-ttu-id="3ab41-106">Šių vaidmenų teisės priskirtos [saugos & atitikties centre.](https://protection.office.com)</span><span class="sxs-lookup"><span data-stu-id="3ab41-106">Permissions to these roles are assigned in the [Security & compliance center.](https://protection.office.com)</span></span>
2. <span data-ttu-id="3ab41-107">[Sukurkite turinio iešką](https://docs.microsoft.com/office365/securitycompliance/content-search) , kad rastumėte pranešimą, kurį norite panaikinti.</span><span class="sxs-lookup"><span data-stu-id="3ab41-107">[Create a content search](https://docs.microsoft.com/office365/securitycompliance/content-search) to find the message to delete.</span></span>
3. <span data-ttu-id="3ab41-108">[Prisijunkite prie saugos & atitikties centro "PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell)".</span><span class="sxs-lookup"><span data-stu-id="3ab41-108">[Connect to Security & Compliance Center PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell).</span></span> <span data-ttu-id="3ab41-109">Jei naudojate MFA, peržiūrėkite šias instrukcijas: [prisijungimas prie saugos & atitikties centro "PowerShell" naudojant kelių dalių autentifikavimą](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell)</span><span class="sxs-lookup"><span data-stu-id="3ab41-109">If you're using MFA, see these instructions: [Connect to Security & Compliance Center PowerShell using multi-factor authentication](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell)</span></span>
4. <span data-ttu-id="3ab41-110">Panaikinkite laišką: paleiskite " `New-ComplianceSearchAction` cmdlet", kad panaikintumėte pranešimą.</span><span class="sxs-lookup"><span data-stu-id="3ab41-110">Delete the message: run the `New-ComplianceSearchAction` cmdlet to delete the message.</span></span> <span data-ttu-id="3ab41-111">Pašalinti laiškai perkeliami į vartotojo atkuriamų elementų aplanką.</span><span class="sxs-lookup"><span data-stu-id="3ab41-111">Deleted messages are moved to a user's Recoverable Items folder.</span></span> <span data-ttu-id="3ab41-112">Jei turite komandą pavyzdys, žiūrėkite [3 veiksmas: panaikinkite laišką.](https://docs.microsoft.com/office365/securitycompliance/search-for-and-delete-messages-in-your-organization)</span><span class="sxs-lookup"><span data-stu-id="3ab41-112">For an example command, see [Step 3: Delete the message.](https://docs.microsoft.com/office365/securitycompliance/search-for-and-delete-messages-in-your-organization)</span></span>
