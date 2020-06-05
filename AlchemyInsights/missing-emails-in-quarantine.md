---
title: Nėra el. laiškų karantine
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5668"
- "9002625"
ms.openlocfilehash: 61a926c363c62bc7acb5efefe42b834f33c78eb6
ms.sourcegitcommit: 8fdcd2acd31e8a4b9a8a0b91674f397d2f7889c1
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 06/03/2020
ms.locfileid: "44569234"
---
# <a name="missing-emails-in-quarantine"></a><span data-ttu-id="19a02-102">Trūksta el. laiškų karantine"</span><span class="sxs-lookup"><span data-stu-id="19a02-102">Missing emails in quarantine"</span></span>

<span data-ttu-id="19a02-103">Administratoriai gali [peržiūrėti, paleisti arba naikinti šiuos pranešimus.](https://docs.microsoft.com/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files?view=o365-worldwide)</span><span class="sxs-lookup"><span data-stu-id="19a02-103">Administrators can [view, release, or delete these messages.](https://docs.microsoft.com/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files?view=o365-worldwide)</span></span>

<span data-ttu-id="19a02-104">Norėdami atidaryti saugos & atitikties centrą, eikite į [https://protection.office.com](https://protection.office.com/) .</span><span class="sxs-lookup"><span data-stu-id="19a02-104">To open the Security & Compliance Center, go to [https://protection.office.com](https://protection.office.com/).</span></span> <span data-ttu-id="19a02-105">Norėdami tiesiogiai atidaryti puslapį Karantinas, eikite į [https://protection.office.com/quarantine](https://protection.office.com/quarantine) .</span><span class="sxs-lookup"><span data-stu-id="19a02-105">To open the Quarantine page directly, go to [https://protection.office.com/quarantine](https://protection.office.com/quarantine).</span></span>  

<span data-ttu-id="19a02-106">Galite ieškoti pagal šias reikšmes:</span><span class="sxs-lookup"><span data-stu-id="19a02-106">You can search by the following values:</span></span>  

- <span data-ttu-id="19a02-107">**Pranešimo ID**: visame pasaulyje unikalus pranešimo identifikatorius.</span><span class="sxs-lookup"><span data-stu-id="19a02-107">**Message ID**: The globally unique identifier of the message.</span></span> <span data-ttu-id="19a02-108">Jei sąraše pasirinksite pranešimą, pasirodžiusioje **išsamios informacijos iškeliamajoje** srityje bus rodoma **pranešimo ID** reikšmė.</span><span class="sxs-lookup"><span data-stu-id="19a02-108">If you select a message in the list, the  **Message ID**  value appears in the  **Details**  flyout pane that appears.</span></span> <span data-ttu-id="19a02-109">Administratoriai gali naudoti [pranešimų sekimą,](https://docs.microsoft.com/microsoft-365/security/office-365-security/message-trace-scc?view=o365-worldwide) kad rastų pranešimus ir atitinkamas pranešimo ID reikšmes.</span><span class="sxs-lookup"><span data-stu-id="19a02-109">Admins can use [message trace](https://docs.microsoft.com/microsoft-365/security/office-365-security/message-trace-scc?view=o365-worldwide) to find messages and their corresponding Message ID values.</span></span>
- <span data-ttu-id="19a02-110">**Siuntėjo el. pašto adresas**: Vieno siuntėjo el. pašto adresas.</span><span class="sxs-lookup"><span data-stu-id="19a02-110">**Sender email address**: A single sender's email address.</span></span>
- <span data-ttu-id="19a02-111">**Gavėjo el. pašto adresas**: Vieno gavėjo el. pašto adresas.</span><span class="sxs-lookup"><span data-stu-id="19a02-111">**Recipient email address**: A single recipient's email address.</span></span>
- <span data-ttu-id="19a02-112">**Tema**: Naudokite visą pranešimo temą.</span><span class="sxs-lookup"><span data-stu-id="19a02-112">**Subject**: Use the entire subject of the message.</span></span> <span data-ttu-id="19a02-113">Ieškaneskiriamos didžiąsias ir mažąsias raides.</span><span class="sxs-lookup"><span data-stu-id="19a02-113">The search is not case-sensitive.</span></span>

<span data-ttu-id="19a02-114">Įvedę ieškos kriterijus, spustelėkite ![ Atnaujinti mygtuką ](https://docs.microsoft.com/microsoft-365/media/scc-quarantine-refresh.png?view=o365-worldwide) **Atnaujinti,** kad filtruotumėte rezultatus.  </span><span class="sxs-lookup"><span data-stu-id="19a02-114">After you've entered the search criteria, click  ![Refresh button](https://docs.microsoft.com/microsoft-365/media/scc-quarantine-refresh.png?view=o365-worldwide)  **Refresh**  to filter the results.</span></span>

<span data-ttu-id="19a02-115">Cmdlet, kurias naudojate peržiūrėti ir tvarkyti pranešimus ir failus karantine yra:</span><span class="sxs-lookup"><span data-stu-id="19a02-115">The cmdlets you use to view and manages messages and files in quarantine are:</span></span>
- [<span data-ttu-id="19a02-116">Naikinti sulaikymo pranešimą</span><span class="sxs-lookup"><span data-stu-id="19a02-116">Delete-QuarantineMessage</span></span>](https://docs.microsoft.com/powershell/module/exchange/delete-quarantinemessage)
- [<span data-ttu-id="19a02-117">Eksportuoti-quarantineMessage</span><span class="sxs-lookup"><span data-stu-id="19a02-117">Export-QuarantineMessage</span></span>](https://docs.microsoft.com/powershell/module/exchange/export-quarantinemessage)
- [<span data-ttu-id="19a02-118">Gauti KarantinePranešimą</span><span class="sxs-lookup"><span data-stu-id="19a02-118">Get-QuarantineMessage</span></span>](https://docs.microsoft.com/powershell/module/exchange/get-quarantinemessage)
- <span data-ttu-id="19a02-119">[Preview-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/preview-quarantinemessage): Atkreipkite dėmesį, kad ši cmdlet skirta tik pranešimams, o ne kenkėjiškų programų failams iš ATP, skirtam "SharePoint Online", "OneDrive" verslui arba "Teams".</span><span class="sxs-lookup"><span data-stu-id="19a02-119">[Preview-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/preview-quarantinemessage): Note that this cmdlet is only for messages, not malware files from ATP for SharePoint Online, OneDrive for Business, or Teams.</span></span>
- [<span data-ttu-id="19a02-120">Išleidimo-QuarantineMessage</span><span class="sxs-lookup"><span data-stu-id="19a02-120">Release-QuarantineMessage</span></span>](https://docs.microsoft.com/powershell/module/exchange/release-quarantinemessage)