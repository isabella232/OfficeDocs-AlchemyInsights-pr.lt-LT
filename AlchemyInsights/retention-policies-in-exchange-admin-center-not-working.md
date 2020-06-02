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
ms.openlocfilehash: 3040365b9d686bcbcce60977ee9bdbbaffc70b24
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 06/02/2020
ms.locfileid: "44502615"
---
# <a name="retention-policies-in-exchange-admin-center"></a><span data-ttu-id="c6c39-102">Saugojimo strategijos "Exchange" administravimo centre</span><span class="sxs-lookup"><span data-stu-id="c6c39-102">Retention Policies in Exchange Admin Center</span></span>

 <span data-ttu-id="c6c39-103">**Problema:** Naujai sukurtos arba atnaujintos saugojimo strategijos "Exchange" administravimo centre netaikomos pašto dėžutėms arba elementai neperkeliami į archyvo pašto dėžutę arba panaikinami.</span><span class="sxs-lookup"><span data-stu-id="c6c39-103">**Issue:** Newly created or updated retention policies in the Exchange Admin Center are not applying to mailboxes or items are not moved to the archive mailbox or deleted.</span></span> 
  
 <span data-ttu-id="c6c39-104">**Priežastis:**</span><span class="sxs-lookup"><span data-stu-id="c6c39-104">**Root Causes:**</span></span>
  
- <span data-ttu-id="c6c39-105">Taip gali būti dėl to, kad **valdomojo aplanko asistentas** neapdorojo vartotojo pašto dėžutės.</span><span class="sxs-lookup"><span data-stu-id="c6c39-105">This may be because the **Managed Folder Assistant** has not processed the user's mailbox.</span></span> <span data-ttu-id="c6c39-106">Valdomojo aplanko asistentas bando apdoroti kiekvieną nuotolinių išteklių saugyklomis pagrįstoje organizacijoje pašto dėžutę kartą per septynias dienas.</span><span class="sxs-lookup"><span data-stu-id="c6c39-106">The Managed Folder Assistant tries to process every mailbox in your cloud-based organization once every seven days.</span></span> <span data-ttu-id="c6c39-107">Jei pakeisite saugojimo žymę arba pašto dėžutei taikote kitą saugojimo strategiją, galite palaukti, kol valdomos aplanko pagalbinė priemonė apdoros pašto dėžutę, arba galite paleisti cmdlet Start-ManagedFolderAssistant, kad paleistumėte valdomojo aplanko asistentą, kad apdorotumėte konkrečią pašto dėžutę.</span><span class="sxs-lookup"><span data-stu-id="c6c39-107">If you change a retention tag or apply a different retention policy to a mailbox, you can wait until the Managed Folder Assist processes the mailbox, or you can run the Start-ManagedFolderAssistant cmdlet to start the Managed Folder Assistant to process a specific mailbox.</span></span> <span data-ttu-id="c6c39-108">Šios cmdlet vykdymas naudingas tikrinant arba šalinant saugojimo strategiją arba saugojimo žymės parametrus.</span><span class="sxs-lookup"><span data-stu-id="c6c39-108">Running this cmdlet is useful for testing or troubleshooting a retention policy or retention tag settings.</span></span> <span data-ttu-id="c6c39-109">Jei norite gauti daugiau informacijos, apsilankykite [paleisti valdomojo aplanko asistentas](https://msdn.microsoft.com/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist).</span><span class="sxs-lookup"><span data-stu-id="c6c39-109">For more information, visit [Run the Managed Folder Assistant](https://msdn.microsoft.com/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist).</span></span>
    
  - <span data-ttu-id="c6c39-110">**Sprendimas:** Vykdykite šią komandą, kad paleistumėte konkrečios pašto dėžutės valdomojo aplanko asistentą:</span><span class="sxs-lookup"><span data-stu-id="c6c39-110">**Solution:** Run the following command to start the Managed Folder Assistant for a specific mailbox:</span></span>
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

- <span data-ttu-id="c6c39-111">Tai taip pat gali įvykti, jei **RetentionHold** buvo **įjungtas** pašto dėžutės.</span><span class="sxs-lookup"><span data-stu-id="c6c39-111">This may also be occur if **RetentionHold** has been **enabled** on the mailbox.</span></span> <span data-ttu-id="c6c39-112">Jei pašto dėžutės buvo įrašytas į RetentionHold, saugojimo strategija pašto dėžutės nebus tvarkomi per tą laiką.</span><span class="sxs-lookup"><span data-stu-id="c6c39-112">If the mailbox has been placed on a RetentionHold, the retention policy on the mailbox will not be processed during that time.</span></span> <span data-ttu-id="c6c39-113">Daugiau informaton dėl RetentionHold parametrą žr.: [Pašto dėžutės saugojimo sulaikymo](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).</span><span class="sxs-lookup"><span data-stu-id="c6c39-113">For more informaton on the RetentionHold setting see: [Mailbox Retention Hold](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).</span></span>
    
    <span data-ttu-id="c6c39-114">**Tirpalas:**</span><span class="sxs-lookup"><span data-stu-id="c6c39-114">**Solution:**</span></span>
    
  - <span data-ttu-id="c6c39-115">Patikrinkite, ar retentionHold parametro būseną konkrečios pašto dėžutės [EXO powershell:](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps)</span><span class="sxs-lookup"><span data-stu-id="c6c39-115">Check the status of the RetentionHold setting on the specific mailbox in [EXO powershell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps):</span></span>
    
  ```
  Get-Mailbox -Identity <name of the mailbox> |fl *retentionHold*
  ```

  - <span data-ttu-id="c6c39-116">Vykdykite šią komandą **norėdami išjungti** RetentionHold konkrečioje pašto dėžutėje:</span><span class="sxs-lookup"><span data-stu-id="c6c39-116">Run the following command to **disable** RetentionHold on a specific mailbox:</span></span>
    
  ```
  Set-Mailbox -RetentionHoldEnabled $false
  ```

  - <span data-ttu-id="c6c39-117">Dabar iš naujo paleiskite valdomojo aplanko asistentas:</span><span class="sxs-lookup"><span data-stu-id="c6c39-117">Now, re-run the Managed folder Assistant:</span></span>
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

 <span data-ttu-id="c6c39-118">**Pastaba:** Jei pašto dėžutės yra mažesnis nei 10 MB, valdomojo aplanko asistentas nebus automatiškai apdoroti pašto dėžutės.</span><span class="sxs-lookup"><span data-stu-id="c6c39-118">**Note:** If a mailbox is smaller than 10 MB, the Managed Folder Assistant will not automatically process the mailbox.</span></span>
 
<span data-ttu-id="c6c39-119">Daugiau informacijos apie saugojimo strategijas "Exchange" administravimo centre rasite:</span><span class="sxs-lookup"><span data-stu-id="c6c39-119">For more info on retention policies in the Exchange Admin Center, see:</span></span>
- [<span data-ttu-id="c6c39-120">Saugojimo žymės ir saugojimo strategijos</span><span class="sxs-lookup"><span data-stu-id="c6c39-120">Retention tags and retention policies</span></span>](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/retention-tags-and-policies)
- [<span data-ttu-id="c6c39-121">Saugojimo strategijos taikymas pašto dėžutėms</span><span class="sxs-lookup"><span data-stu-id="c6c39-121">Apply a retention policy to mailboxes</span></span>](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy)
- [<span data-ttu-id="c6c39-122">Saugojimo žymių pridėjimas arba šalinimas</span><span class="sxs-lookup"><span data-stu-id="c6c39-122">Add or remove retention tags</span></span>](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/add-or-remove-retention-tags)
- [<span data-ttu-id="c6c39-123">Kaip nustatyti sulaikymo, padėto pašto dėžutėje, tipą</span><span class="sxs-lookup"><span data-stu-id="c6c39-123">How to identify the type of hold placed on a mailbox</span></span>](https://docs.microsoft.com/microsoft-365/compliance/identify-a-hold-on-an-exchange-online-mailbox)
