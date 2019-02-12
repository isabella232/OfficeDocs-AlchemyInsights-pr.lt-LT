---
title: 1336 RecoverableItems aplankas yra visiškai
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: a3a923e8-fece-4a26-b8b6-00970d75275e
ms.openlocfilehash: dbf4930c34e4175a14b77fab4eafc953bb37cc02
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 02/12/2019
ms.locfileid: "29909296"
---
# <a name="the-recoverable-items-folder-is-full"></a><span data-ttu-id="07889-102">Aplanko Atkuriami elementai yra visiškai</span><span class="sxs-lookup"><span data-stu-id="07889-102">The Recoverable Items folder is full</span></span>

<span data-ttu-id="07889-p101">Exchange Online pašto dėžutes "Office 365", numatytosios saugyklos aplanko Atkuriami elementai yra 30 GB. Saugyklos aplanko Atkuriami elementai automatiškai padidinama iki 100 GB skiriamas sulaikymas dėl bylinėjimosi, eDiscovery laikyti, ar priskirtas "Office 365" saugojimo strategijos pašto dėžutės.</span><span class="sxs-lookup"><span data-stu-id="07889-p101">For Exchange Online mailboxes in Office 365, the default storage limit for the Recoverable Items folder is 30 GB. The storage limit for the Recoverable Items folder is automatically increased to 100 GB if the mailbox is placed on Litigation Hold, eDiscovery hold, or is assigned to an Office 365 retention policy.</span></span>
  
<span data-ttu-id="07889-105">Aplanko Atkuriami elementai pasiekus saugyklos ribą, pašto dėžutės funkcijas veikia vienu iš šių būdų:</span><span class="sxs-lookup"><span data-stu-id="07889-105">When the Recoverable Items folder reaches the storage limit, mailbox functionality is affected in the following ways:</span></span>
  
- <span data-ttu-id="07889-106">Vartotojas negali panaikinti elementus iš pašto dėžutės.</span><span class="sxs-lookup"><span data-stu-id="07889-106">The user can't delete items from the mailbox.</span></span>
    
- <span data-ttu-id="07889-107">Valdomojo aplanko asistentas negali naikinti elementus saugojimo žymę arba valdomojo aplanko parametrai.</span><span class="sxs-lookup"><span data-stu-id="07889-107">The Managed Folder Assistant can't delete items based on retention tag or managed folder settings.</span></span>
    
- <span data-ttu-id="07889-108">Pašto dėžučių, kurios vieno elemento atkūrimas įgalintas arba yra laikinieji, kopija rašant puslapis apsaugos procesas negali išlaikyti prekių vartotojas redagavo versijas.</span><span class="sxs-lookup"><span data-stu-id="07889-108">For mailboxes that have Single Item Recovery enabled or are placed on hold, the copy-on-write page protection process can't maintain versions of items edited by the user.</span></span>
    
- <span data-ttu-id="07889-109">Pašto dėžučių ar pašto dėžutės audito žurnalo pildymo funkcija įjungta, pašto dėžutės audito žurnalo įrašai gali būti saugomi audito poaplankį aplanke Atkuriami elementai.</span><span class="sxs-lookup"><span data-stu-id="07889-109">For mailboxes that have mailbox audit logging enabled, no mailbox audit log entries can be saved in the Audits subfolder in the Recoverable Items folder.</span></span>
    
<span data-ttu-id="07889-p102">Pašto dėžučių, kuris nėra sulaikytas, administratoriai gali naudoti ir `Search-Mailbox -SearchDumpsterOnly -DeleteContent` komanda Exchange Online "PowerShell" Norėdami naikinti elementus aplanke Atkuriami elementai. Daugiau informacijos ieškokite šiose temose:</span><span class="sxs-lookup"><span data-stu-id="07889-p102">For mailboxes that aren't on hold, admins can use the  `Search-Mailbox -SearchDumpsterOnly -DeleteContent` command in Exchange Online PowerShell to delete items in the Recoverable Items folder. For more information, see the following topics:</span></span> 
  
- [<span data-ttu-id="07889-112">Ieškoti ir panaikinti laiškus</span><span class="sxs-lookup"><span data-stu-id="07889-112">Search for and delete messages</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-for-and-delete-messagesadmin-help)
    
- [<span data-ttu-id="07889-113">Paieška-dėžutės</span><span class="sxs-lookup"><span data-stu-id="07889-113">Search-Mailbox</span></span>](https://docs.microsoft.com/powershell/module/exchange/mailboxes/Search-Mailbox)
    
<span data-ttu-id="07889-p103">Pašto dėžučių, kurios yra sustabdytos, administratoriai turi pašalinti sulaikymą, kol jie gali panaikinti elementus iš aplanko Atkuriami elementai. Daugiau informacijos rasite [Naikinti elementus aplanke nuotolinių išteklių saugyklomis pagrįstos pašto dėžučių laikykite Atkuriami elementai](https://docs.microsoft.com/office365/securitycompliance/delete-items-in-the-recoverable-items-folder-of-mailboxes-on-hold).</span><span class="sxs-lookup"><span data-stu-id="07889-p103">For mailboxes that are on hold, admins have to remove the hold before they can deleted items from the Recoverable Items folder. For more information, see [Delete items in the Recoverable Items folder of cloud-based mailboxes on hold](https://docs.microsoft.com/office365/securitycompliance/delete-items-in-the-recoverable-items-folder-of-mailboxes-on-hold).</span></span>
  
<span data-ttu-id="07889-p104">Siekiant padėti užkirsti kelią aplanko Atkuriami elementai tampa pilna, administratoriai gali padidinti atkuriamų elementų aplanko pašto dėžutės palaikykite ir nustatyti pašto dėžutės saugojimo strategija, kuri perkelia elementus iš aplanko Atkuriami elementai į vartotojo archyvo saugyklos pašto dėžutės. Peržiūrėkite [padidinti Atkuriami elementai kvota pašto dėžučių, laikykite](https://docs.microsoft.com/office365/securitycompliance/increase-the-recoverable-quota-for-mailboxes-on-hold).</span><span class="sxs-lookup"><span data-stu-id="07889-p104">To help prevent the Recoverable Items folder from becoming full, admins can increase the storage limit of the Recoverable Items folder for mailboxes on hold and set up a mailbox retention policy that moves items from the Recoverable Items folder to the user's archive mailbox. See [Increase the Recoverable Items quota for mailboxes on hold](https://docs.microsoft.com/office365/securitycompliance/increase-the-recoverable-quota-for-mailboxes-on-hold).</span></span>
  

