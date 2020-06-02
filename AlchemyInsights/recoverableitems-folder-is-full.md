---
title: 1336 RecoverableItems aplankas yra pilnas
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1336"
- "3700003"
ms.assetid: a3a923e8-fece-4a26-b8b6-00970d75275e
ms.openlocfilehash: 4f0cba480fcc05114abd8f370b84e9a37e5f2804
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 06/02/2020
ms.locfileid: "44510760"
---
# <a name="the-recoverable-items-folder-is-full"></a><span data-ttu-id="206ac-102">Atkuriamų elementų aplankas pilnas</span><span class="sxs-lookup"><span data-stu-id="206ac-102">The Recoverable Items folder is full</span></span>

<span data-ttu-id="206ac-103">Exchange Online pašto dėžučių, numatytasis saugyklos riba atkuriamų elementų aplanko yra 30 GB.</span><span class="sxs-lookup"><span data-stu-id="206ac-103">For Exchange Online mailboxes, the default storage limit for the Recoverable Items folder is 30 GB.</span></span> <span data-ttu-id="206ac-104">Atkuriamų elementų aplanko saugyklos limitas automatiškai padidinamas iki 100 GB, jei pašto dėžutė yra sulaikytas bylinėjimosi, el. duomenų aptikimo sulaikymas arba priskirtas saugojimo strategijai.</span><span class="sxs-lookup"><span data-stu-id="206ac-104">The storage limit for the Recoverable Items folder is automatically increased to 100 GB if the mailbox is placed on Litigation Hold, eDiscovery hold, or is assigned to a retention policy.</span></span>

<span data-ttu-id="206ac-105">Kai atkuriamų elementų aplankas pasiekia saugyklos ribą, pašto dėžutės funkcija turi įtakos šiais būdais:</span><span class="sxs-lookup"><span data-stu-id="206ac-105">When the Recoverable Items folder reaches the storage limit, mailbox functionality is affected in the following ways:</span></span>

- <span data-ttu-id="206ac-106">Vartotojas negali panaikinti elementų iš pašto dėžutės.</span><span class="sxs-lookup"><span data-stu-id="206ac-106">The user can't delete items from the mailbox.</span></span>

- <span data-ttu-id="206ac-107">Valdomojo aplanko asistentas negali panaikinti elementų pagal saugojimo žymę arba valdomo aplanko parametrus.</span><span class="sxs-lookup"><span data-stu-id="206ac-107">The Managed Folder Assistant can't delete items based on retention tag or managed folder settings.</span></span>

- <span data-ttu-id="206ac-108">Pašto dėžučių, kuriose įgalintas vieno elemento atkūrimas arba kurios yra sulaikytos, kopijavimo rašymo puslapio apsaugos procesas negali išlaikyti vartotojo redaguotų elementų versijų.</span><span class="sxs-lookup"><span data-stu-id="206ac-108">For mailboxes that have Single Item Recovery enabled or are placed on hold, the copy-on-write page protection process can't maintain versions of items edited by the user.</span></span>

- <span data-ttu-id="206ac-109">Pašto dėžučių, kuriose įgalintas pašto dėžučių audito registravimas, nėra pašto dėžutės audito žurnalo įrašus galima įrašyti į aplanką Atkuriami elementai poaplankyje Audito.</span><span class="sxs-lookup"><span data-stu-id="206ac-109">For mailboxes that have mailbox audit logging enabled, no mailbox audit log entries can be saved in the Audits subfolder in the Recoverable Items folder.</span></span>

<span data-ttu-id="206ac-110">Pašto dėžučių, kurios nėra sulaikytas, administratoriai gali naudoti `Search-Mailbox -SearchDumpsterOnly -DeleteContent` komandą Exchange Online PowerShell panaikinti elementus į atkuriami elementai aplanke.</span><span class="sxs-lookup"><span data-stu-id="206ac-110">For mailboxes that aren't on hold, admins can use the `Search-Mailbox -SearchDumpsterOnly -DeleteContent` command in Exchange Online PowerShell to delete items in the Recoverable Items folder.</span></span> <span data-ttu-id="206ac-111">Norėdami gauti daugiau informacijos žr. toliau nurodytas temas:</span><span class="sxs-lookup"><span data-stu-id="206ac-111">For more information, see the following topics:</span></span>

- [<span data-ttu-id="206ac-112">Pranešimų ieška ir naikinimas</span><span class="sxs-lookup"><span data-stu-id="206ac-112">Search for and delete messages</span></span>](https://docs.microsoft.com/microsoft-365/compliance/search-for-and-delete-messagesadmin-help)

- [<span data-ttu-id="206ac-113">Ieškos pašto dėžutė</span><span class="sxs-lookup"><span data-stu-id="206ac-113">Search-Mailbox</span></span>](https://docs.microsoft.com/powershell/module/exchange/mailboxes/Search-Mailbox)

<span data-ttu-id="206ac-114">Sulaikytoms pašto dėžutėms administratoriai turi pašalinti sulaikymą, kad galėtų panaikinti elementus iš aplanko Atkuriami elementai.</span><span class="sxs-lookup"><span data-stu-id="206ac-114">For mailboxes that are on hold, admins have to remove the hold before they can deleted items from the Recoverable Items folder.</span></span> <span data-ttu-id="206ac-115">Daugiau informacijos [ieškokite Naikinti elementus, esančius nuotolinių išteklių saugyklomis pagrįstų pašto dėžučių aplanke Atkuriami elementai](https://docs.microsoft.com/microsoft-365/compliance/delete-items-in-the-recoverable-items-folder-of-mailboxes-on-hold).</span><span class="sxs-lookup"><span data-stu-id="206ac-115">For more information, see [Delete items in the Recoverable Items folder of cloud-based mailboxes on hold](https://docs.microsoft.com/microsoft-365/compliance/delete-items-in-the-recoverable-items-folder-of-mailboxes-on-hold).</span></span>

<span data-ttu-id="206ac-116">Kad aplankas Atkuriami elementai netaptų pilnas, administratoriai gali padidinti sulaikytų pašto dėžučių aplanko Atkuriami elementai saugyklos ribą ir nustatyti pašto dėžutės saugojimo strategiją, kuri perkelia elementus iš aplanko Atkuriami elementai į vartotojo archyvo pašto dėžutę.</span><span class="sxs-lookup"><span data-stu-id="206ac-116">To help prevent the Recoverable Items folder from becoming full, admins can increase the storage limit of the Recoverable Items folder for mailboxes on hold and set up a mailbox retention policy that moves items from the Recoverable Items folder to the user's archive mailbox.</span></span> <span data-ttu-id="206ac-117">Peržiūrėkite [padidinti sulaikytų pašto dėžučių atkuriamų elementų kvotą](https://docs.microsoft.com/microsoft-365/compliance/increase-the-recoverable-quota-for-mailboxes-on-hold).</span><span class="sxs-lookup"><span data-stu-id="206ac-117">See [Increase the Recoverable Items quota for mailboxes on hold](https://docs.microsoft.com/microsoft-365/compliance/increase-the-recoverable-quota-for-mailboxes-on-hold).</span></span>
