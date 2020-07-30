---
title: Saugojimo strategijos Exchange administravimo centro neveikia
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "308"
- "3100007"
ms.assetid: a48fd5fd-4af7-4d5f-b617-b0f9334ccaa7
ms.openlocfilehash: 4d3ca121c8d22a0900f136f7f2a754dfb5b435f5
ms.sourcegitcommit: ffbed67c0a16ec423fa1d79b71e48ea4e2d320e1
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 07/29/2020
ms.locfileid: "46522815"
---
# <a name="retention-policies-in-exchange-admin-center"></a><span data-ttu-id="c9016-102">Saugojimo strategijos "Exchange" administravimo centre</span><span class="sxs-lookup"><span data-stu-id="c9016-102">Retention Policies in Exchange Admin Center</span></span>

<span data-ttu-id="c9016-103">Jei norite, kad mes vykdome toliau nurodytų parametrų automatinius patikrinimus, šio puslapio viršuje pasirinkite mygtuką "Atgal" <-- ir įveskite vartotojo, turinčio problemų dėl saugojimo strategijų, el. pašto adresą.</span><span class="sxs-lookup"><span data-stu-id="c9016-103">If you want us to run automated checks for the settings mentioned below, select the back button <-- at the top of this page, and then enter the email address of the user who has problems with retention policies.</span></span>

 <span data-ttu-id="c9016-104">**Problema:** Naujai sukurtos arba atnaujintos saugojimo strategijos Exchange administravimo centro netaikomos pašto dėžutės arba elementai nėra perkeliami į archyvo pašto dėžutę arba panaikinami.</span><span class="sxs-lookup"><span data-stu-id="c9016-104">**Issue:** Newly created or updated retention policies in the Exchange Admin Center are not applying to mailboxes or items are not moved to the archive mailbox or deleted.</span></span> 
  
 <span data-ttu-id="c9016-105">**Priežastis:**</span><span class="sxs-lookup"><span data-stu-id="c9016-105">**Root Causes:**</span></span>
  
- <span data-ttu-id="c9016-106">Taip gali būti dėl to, kad **valdomojo aplanko asistentas** neapdorojo vartotojo pašto dėžutės.</span><span class="sxs-lookup"><span data-stu-id="c9016-106">This may be because the **Managed Folder Assistant** has not processed the user's mailbox.</span></span> <span data-ttu-id="c9016-107">Valdomojo aplanko asistentas bando apdoroti kiekvieną pašto dėžutę nuotolinių išteklių saugyklomis pagrįstoje organizacijoje kartą per septynias dienas.</span><span class="sxs-lookup"><span data-stu-id="c9016-107">The Managed Folder Assistant tries to process every mailbox in your cloud-based organization once every seven days.</span></span> <span data-ttu-id="c9016-108">Jei pakeisite saugojimo žymę arba pritaikysite kitą saugojimo strategiją pašto dėžutei, galite palaukti, kol valdomojo aplanko pagalbinė priemonė apdoros pašto dėžutę, arba galėsite paleisti cmdlet Start-ManagedFolderAssistant, kad paleistumėte valdomojo aplanko asistentą, kad apdorotumėte konkrečią pašto dėžutę.</span><span class="sxs-lookup"><span data-stu-id="c9016-108">If you change a retention tag or apply a different retention policy to a mailbox, you can wait until the Managed Folder Assist processes the mailbox, or you can run the Start-ManagedFolderAssistant cmdlet to start the Managed Folder Assistant to process a specific mailbox.</span></span> <span data-ttu-id="c9016-109">Šio cmdlet vykdymas naudingas tikrinant arba šalinant saugojimo strategijos arba saugojimo žymės parametrų triktis.</span><span class="sxs-lookup"><span data-stu-id="c9016-109">Running this cmdlet is useful for testing or troubleshooting a retention policy or retention tag settings.</span></span> <span data-ttu-id="c9016-110">Jei norite gauti daugiau informacijos, apsilankykite [paleisti valdomojo aplanko asistentas](https://msdn.microsoft.com/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist).</span><span class="sxs-lookup"><span data-stu-id="c9016-110">For more information, visit [Run the Managed Folder Assistant](https://msdn.microsoft.com/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist).</span></span>
    
  - <span data-ttu-id="c9016-111">**Sprendimas:** Vykdykite šią komandą, kad paleistumėte konkrečios pašto dėžutės valdomojo aplanko asistentą:</span><span class="sxs-lookup"><span data-stu-id="c9016-111">**Solution:** Run the following command to start the Managed Folder Assistant for a specific mailbox:</span></span>
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

- <span data-ttu-id="c9016-112">Taip gali atsitikti ir tuo atveju, jei **Saugojimhold** buvo **įjungtas** pašto dėžutės.</span><span class="sxs-lookup"><span data-stu-id="c9016-112">This may also be occur if **RetentionHold** has been **enabled** on the mailbox.</span></span> <span data-ttu-id="c9016-113">Jei pašto dėžutės buvo ant RetentionHold, saugojimo strategijos pašto dėžutės nebus tvarkomi per tą laiką.</span><span class="sxs-lookup"><span data-stu-id="c9016-113">If the mailbox has been placed on a RetentionHold, the retention policy on the mailbox will not be processed during that time.</span></span> <span data-ttu-id="c9016-114">Jei norite gauti daugiau informacijos apie RetentionHold parametrą žr.: [Pašto dėžutės saugojimo sulaikymas](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).</span><span class="sxs-lookup"><span data-stu-id="c9016-114">For more informaton on the RetentionHold setting see: [Mailbox Retention Hold](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).</span></span>
    
    <span data-ttu-id="c9016-115">**Tirpalas:**</span><span class="sxs-lookup"><span data-stu-id="c9016-115">**Solution:**</span></span>
    
  - <span data-ttu-id="c9016-116">Patikrinkite, ar statusu RetentionHold parametrą konkrečios pašto dėžutės [EXO PowerShell:](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps)</span><span class="sxs-lookup"><span data-stu-id="c9016-116">Check the status of the RetentionHold setting on the specific mailbox in [EXO powershell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps):</span></span>
    
  ```
  Get-Mailbox -Identity <name of the mailbox> |fl *retentionHold*
  ```

  - <span data-ttu-id="c9016-117">Vykdykite šią komandą norėdami **išjungti** RetentionHold konkrečioje pašto dėžutėje:</span><span class="sxs-lookup"><span data-stu-id="c9016-117">Run the following command to **disable** RetentionHold on a specific mailbox:</span></span>
    
  ```
  Set-Mailbox -RetentionHoldEnabled $false
  ```

  - <span data-ttu-id="c9016-118">Dabar iš naujo paleiskite valdomojo aplanko asistentą:</span><span class="sxs-lookup"><span data-stu-id="c9016-118">Now, re-run the Managed folder Assistant:</span></span>
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

 <span data-ttu-id="c9016-119">**Pastaba:** Jei pašto dėžutės yra mažesnis nei 10 MB, valdomojo aplanko asistentas nebus automatiškai apdoroti pašto dėžutės.</span><span class="sxs-lookup"><span data-stu-id="c9016-119">**Note:** If a mailbox is smaller than 10 MB, the Managed Folder Assistant will not automatically process the mailbox.</span></span>
 
<span data-ttu-id="c9016-120">Daugiau informacijos apie saugojimo strategijas "Exchange" administravimo centre rasite:</span><span class="sxs-lookup"><span data-stu-id="c9016-120">For more info on retention policies in the Exchange Admin Center, see:</span></span>
- [<span data-ttu-id="c9016-121">Saugojimo žymės ir saugojimo strategijos</span><span class="sxs-lookup"><span data-stu-id="c9016-121">Retention tags and retention policies</span></span>](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/retention-tags-and-policies)
- [<span data-ttu-id="c9016-122">Saugojimo strategijos taikymas pašto dėžutėms</span><span class="sxs-lookup"><span data-stu-id="c9016-122">Apply a retention policy to mailboxes</span></span>](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy)
- [<span data-ttu-id="c9016-123">Saugojimo žymių pridėjimas arba šalinimas</span><span class="sxs-lookup"><span data-stu-id="c9016-123">Add or remove retention tags</span></span>](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/add-or-remove-retention-tags)
- [<span data-ttu-id="c9016-124">Kaip nustatyti pašto dėžutės sulaikymo tipą</span><span class="sxs-lookup"><span data-stu-id="c9016-124">How to identify the type of hold placed on a mailbox</span></span>](https://docs.microsoft.com/microsoft-365/compliance/identify-a-hold-on-an-exchange-online-mailbox)
