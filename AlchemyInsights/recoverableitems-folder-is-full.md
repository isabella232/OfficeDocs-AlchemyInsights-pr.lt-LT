---
title: "\"1336\" Recoverableitonų aplankas yra pilnas"
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1336"
- "3700003"
ms.assetid: a3a923e8-fece-4a26-b8b6-00970d75275e
ms.openlocfilehash: 6ae608b776332402fe333315f5e4ff6072b0a651
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47741275"
---
# <a name="the-recoverable-items-folder-is-full"></a><span data-ttu-id="9afef-102">Aplankas Atkuriami elementai yra pilnas</span><span class="sxs-lookup"><span data-stu-id="9afef-102">The Recoverable Items folder is full</span></span>

<span data-ttu-id="9afef-103">"Exchange Online" pašto dėžutėms numatytoji aplanko atkuriamų elementų saugyklos riba yra 30 GB.</span><span class="sxs-lookup"><span data-stu-id="9afef-103">For Exchange Online mailboxes, the default storage limit for the Recoverable Items folder is 30 GB.</span></span> <span data-ttu-id="9afef-104">Aplanko Atkuriami elementai saugyklos limitas automatiškai padidinamas iki 100 GB, jei pašto dėžutė įtraukta į sulaikymą dėl bylinėjimosi, "el. Discovery" sulaikyta arba priskiriama saugojimo strategijai.</span><span class="sxs-lookup"><span data-stu-id="9afef-104">The storage limit for the Recoverable Items folder is automatically increased to 100 GB if the mailbox is placed on Litigation Hold, eDiscovery hold, or is assigned to a retention policy.</span></span>

<span data-ttu-id="9afef-105">Kai atkuriamų elementų aplankas pasiekia saugyklos limitą, pašto dėžutės funkcijos veikia šiais būdais:</span><span class="sxs-lookup"><span data-stu-id="9afef-105">When the Recoverable Items folder reaches the storage limit, mailbox functionality is affected in the following ways:</span></span>

- <span data-ttu-id="9afef-106">Vartotojas negali panaikinti pašto dėžutės elementų.</span><span class="sxs-lookup"><span data-stu-id="9afef-106">The user can't delete items from the mailbox.</span></span>

- <span data-ttu-id="9afef-107">Valdomojo aplanko pagalbinė priemonė negali panaikinti elementų, pagrįstų saugojimo žyme arba valdomais aplanko parametrais.</span><span class="sxs-lookup"><span data-stu-id="9afef-107">The Managed Folder Assistant can't delete items based on retention tag or managed folder settings.</span></span>

- <span data-ttu-id="9afef-108">Pašto dėžučių, kurioms įgalintas vieno elemento atkūrimas arba kurios sulaikytos, kopijavimo ir rašymo puslapio apsaugos procesas negali išlaikyti vartotojo redaguotų elementų versijų.</span><span class="sxs-lookup"><span data-stu-id="9afef-108">For mailboxes that have Single Item Recovery enabled or are placed on hold, the copy-on-write page protection process can't maintain versions of items edited by the user.</span></span>

- <span data-ttu-id="9afef-109">Pašto dėžučių, kurioms įgalintas pašto dėžučių audito registravimas, pašto dėžučių audito žurnalo įrašus galima įrašyti aplanke Atkuriami elementai.</span><span class="sxs-lookup"><span data-stu-id="9afef-109">For mailboxes that have mailbox audit logging enabled, no mailbox audit log entries can be saved in the Audits subfolder in the Recoverable Items folder.</span></span>

<span data-ttu-id="9afef-110">Jei pašto dėžutės nėra sulaikytos, administratoriai gali naudoti komandą " `Search-Mailbox -SearchDumpsterOnly -DeleteContent` Exchange Online PowerShell", kad panaikintų elementų aplanke Atkuriami elementai.</span><span class="sxs-lookup"><span data-stu-id="9afef-110">For mailboxes that aren't on hold, admins can use the `Search-Mailbox -SearchDumpsterOnly -DeleteContent` command in Exchange Online PowerShell to delete items in the Recoverable Items folder.</span></span> <span data-ttu-id="9afef-111">Norėdami gauti daugiau informacijos žr. toliau nurodytas temas:</span><span class="sxs-lookup"><span data-stu-id="9afef-111">For more information, see the following topics:</span></span>

- [<span data-ttu-id="9afef-112">Žinučių ieška ir naikinimas</span><span class="sxs-lookup"><span data-stu-id="9afef-112">Search for and delete messages</span></span>](https://docs.microsoft.com/microsoft-365/compliance/search-for-and-delete-messagesadmin-help)

- [<span data-ttu-id="9afef-113">Ieška – pašto dėžutė</span><span class="sxs-lookup"><span data-stu-id="9afef-113">Search-Mailbox</span></span>](https://docs.microsoft.com/powershell/module/exchange/mailboxes/Search-Mailbox)

<span data-ttu-id="9afef-114">Jei pašto dėžutės yra sulaikytos, administratoriai turi pašalinti sulaikymą prieš panaikindami elementus iš aplanko Atkuriami elementai.</span><span class="sxs-lookup"><span data-stu-id="9afef-114">For mailboxes that are on hold, admins have to remove the hold before they can deleted items from the Recoverable Items folder.</span></span> <span data-ttu-id="9afef-115">Daugiau informacijos ieškokite [elementų naikinimas nuotolinėmis duomenų saugyklomis pagrįstų pašto dėžučių aplanke Atkuriami elementai](https://docs.microsoft.com/microsoft-365/compliance/delete-items-in-the-recoverable-items-folder-of-mailboxes-on-hold).</span><span class="sxs-lookup"><span data-stu-id="9afef-115">For more information, see [Delete items in the Recoverable Items folder of cloud-based mailboxes on hold](https://docs.microsoft.com/microsoft-365/compliance/delete-items-in-the-recoverable-items-folder-of-mailboxes-on-hold).</span></span>

<span data-ttu-id="9afef-116">Norėdami padėti apsisaugoti nuo aplanko Atkuriami elementai iš dalies, administratoriai gali padidinti aplanko atkuriamų elementų saugyklos limitą ir nustatyti pašto dėžučių saugojimo strategiją, kuri perkelia elementus iš aplanko Atkuriami elementai į vartotojo archyvo pašto dėžutę.</span><span class="sxs-lookup"><span data-stu-id="9afef-116">To help prevent the Recoverable Items folder from becoming full, admins can increase the storage limit of the Recoverable Items folder for mailboxes on hold and set up a mailbox retention policy that moves items from the Recoverable Items folder to the user's archive mailbox.</span></span> <span data-ttu-id="9afef-117">Peržiūrėkite ["sulaikyti" pašto dėžučių grąžinamos dalies kvotas](https://docs.microsoft.com/microsoft-365/compliance/increase-the-recoverable-quota-for-mailboxes-on-hold).</span><span class="sxs-lookup"><span data-stu-id="9afef-117">See [Increase the Recoverable Items quota for mailboxes on hold](https://docs.microsoft.com/microsoft-365/compliance/increase-the-recoverable-quota-for-mailboxes-on-hold).</span></span>
