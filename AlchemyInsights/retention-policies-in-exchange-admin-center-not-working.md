---
title: "\"Exchange\" administravimo centro neveikia saugojimo strategijos"
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
- "308"
- "3100007"
ms.assetid: a48fd5fd-4af7-4d5f-b617-b0f9334ccaa7
ms.openlocfilehash: 1fee2361b2dd6e0989d430a17aebb13bd5948578
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47740518"
---
# <a name="retention-policies-in-exchange-admin-center"></a><span data-ttu-id="9358c-102">Saugojimo strategijos "Exchange" administravimo centre</span><span class="sxs-lookup"><span data-stu-id="9358c-102">Retention Policies in Exchange Admin Center</span></span>

<span data-ttu-id="9358c-103">Jei norite, kad būtų atlikti automatizuoti toliau nurodytų parametrų tikrinimai, pasirinkite mygtuką atgal <--šio puslapio viršuje, tada įveskite vartotojo, kuris turi problemų su saugojimo strategijomis, el. pašto adresą.</span><span class="sxs-lookup"><span data-stu-id="9358c-103">If you want us to run automated checks for the settings mentioned below, select the back button <-- at the top of this page, and then enter the email address of the user who has problems with retention policies.</span></span>

 <span data-ttu-id="9358c-104">**Problema:** Naujai sukurtos arba atnaujintos saugojimo strategijos "Exchange" administravimo centre netaikomos pašto dėžutėms arba elementai neperkeliami į archyvo pašto dėžutę arba panaikinta.</span><span class="sxs-lookup"><span data-stu-id="9358c-104">**Issue:** Newly created or updated retention policies in the Exchange Admin Center are not applying to mailboxes or items are not moved to the archive mailbox or deleted.</span></span> 
  
 <span data-ttu-id="9358c-105">**Pagrindinės priežastys:**</span><span class="sxs-lookup"><span data-stu-id="9358c-105">**Root Causes:**</span></span>
  
- <span data-ttu-id="9358c-106">Taip gali būti dėl to, kad **valdomojo aplanko asistentas** neapdorojo vartotojo pašto dėžutės.</span><span class="sxs-lookup"><span data-stu-id="9358c-106">This may be because the **Managed Folder Assistant** has not processed the user's mailbox.</span></span> <span data-ttu-id="9358c-107">Valdomojo aplanko asistentas kiekvieną nuotolinių išteklių saugyklomis pagrįstos organizacijos pašto dėžutę bando apdoroti kas septynias dienas.</span><span class="sxs-lookup"><span data-stu-id="9358c-107">The Managed Folder Assistant tries to process every mailbox in your cloud-based organization once every seven days.</span></span> <span data-ttu-id="9358c-108">Jei keičiate saugojimo žymę arba taikote kitokią saugojimo strategiją pašto dėžutei, galite palaukti, kol valdomojo aplanko pagalba apdoros pašto dėžutę, arba galite paleisti "Start-ManagedFolderAssistant" cmdlet, kad paleistumėte valdomojo aplanko asistentą ir apdorotų konkrečią pašto dėžutę.</span><span class="sxs-lookup"><span data-stu-id="9358c-108">If you change a retention tag or apply a different retention policy to a mailbox, you can wait until the Managed Folder Assist processes the mailbox, or you can run the Start-ManagedFolderAssistant cmdlet to start the Managed Folder Assistant to process a specific mailbox.</span></span> <span data-ttu-id="9358c-109">Paleidus šią "cmdlet" galima išbandyti arba pašalinti saugojimo strategijos arba išsaugojimo žymių parametrus.</span><span class="sxs-lookup"><span data-stu-id="9358c-109">Running this cmdlet is useful for testing or troubleshooting a retention policy or retention tag settings.</span></span> <span data-ttu-id="9358c-110">Norėdami gauti daugiau informacijos, apsilankykite [valdomojo aplanko pagalbinės priemonės paleidimas](https://msdn.microsoft.com/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist).</span><span class="sxs-lookup"><span data-stu-id="9358c-110">For more information, visit [Run the Managed Folder Assistant](https://msdn.microsoft.com/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist).</span></span>
    
  - <span data-ttu-id="9358c-111">**Sprendimas:** Vykdykite šią komandą, kad paleistumėte konkrečios pašto dėžutės valdomojo aplanko asistentą:</span><span class="sxs-lookup"><span data-stu-id="9358c-111">**Solution:** Run the following command to start the Managed Folder Assistant for a specific mailbox:</span></span>
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

- <span data-ttu-id="9358c-112">Taip pat gali nutikti, jei pašto dėžutėje **įgalintas** **RetentionHold** .</span><span class="sxs-lookup"><span data-stu-id="9358c-112">This may also be occur if **RetentionHold** has been **enabled** on the mailbox.</span></span> <span data-ttu-id="9358c-113">Jei pašto dėžutė yra įtraukta į Retentionsulaikymą, pašto dėžutės saugojimo strategija tuo metu nebus apdorota.</span><span class="sxs-lookup"><span data-stu-id="9358c-113">If the mailbox has been placed on a RetentionHold, the retention policy on the mailbox will not be processed during that time.</span></span> <span data-ttu-id="9358c-114">Daugiau informacijos apie RetentionHold parametrą matyti: [pašto dėžutės saugojimo sulaikymas](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).</span><span class="sxs-lookup"><span data-stu-id="9358c-114">For more informaton on the RetentionHold setting see: [Mailbox Retention Hold](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).</span></span>
    
    <span data-ttu-id="9358c-115">**Tirpalo**</span><span class="sxs-lookup"><span data-stu-id="9358c-115">**Solution:**</span></span>
    
  - <span data-ttu-id="9358c-116">Pažymėkite " [EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps)" konkrečios pašto dėžutės parametro RetentionHold būseną:</span><span class="sxs-lookup"><span data-stu-id="9358c-116">Check the status of the RetentionHold setting on the specific mailbox in [EXO powershell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps):</span></span>
    
  ```
  Get-Mailbox -Identity <name of the mailbox> |fl *retentionHold*
  ```

  - <span data-ttu-id="9358c-117">Vykdykite šią komandą, kad **išjungtumėte** RetentionHold konkrečioje pašto dėžutėje:</span><span class="sxs-lookup"><span data-stu-id="9358c-117">Run the following command to **disable** RetentionHold on a specific mailbox:</span></span>
    
  ```
  Set-Mailbox -RetentionHoldEnabled $false
  ```

  - <span data-ttu-id="9358c-118">Dabar iš naujo paleiskite valdomojo aplanko asistentą:</span><span class="sxs-lookup"><span data-stu-id="9358c-118">Now, re-run the Managed folder Assistant:</span></span>
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

 <span data-ttu-id="9358c-119">**Pastaba:** Jei pašto dėžutė yra mažesnė nei 10 MB, valdomojo aplanko asistentas automatiškai neapdoros pašto dėžutės.</span><span class="sxs-lookup"><span data-stu-id="9358c-119">**Note:** If a mailbox is smaller than 10 MB, the Managed Folder Assistant will not automatically process the mailbox.</span></span>
 
<span data-ttu-id="9358c-120">Daugiau informacijos apie saugojimo strategijas "Exchange" administravimo centre rasite:</span><span class="sxs-lookup"><span data-stu-id="9358c-120">For more info on retention policies in the Exchange Admin Center, see:</span></span>
- [<span data-ttu-id="9358c-121">Saugojimo žymės ir saugojimo strategijos</span><span class="sxs-lookup"><span data-stu-id="9358c-121">Retention tags and retention policies</span></span>](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/retention-tags-and-policies)
- [<span data-ttu-id="9358c-122">Saugojimo strategijos taikymas pašto dėžutėms</span><span class="sxs-lookup"><span data-stu-id="9358c-122">Apply a retention policy to mailboxes</span></span>](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy)
- [<span data-ttu-id="9358c-123">Saugojimo žymių įtraukimas arba šalinimas</span><span class="sxs-lookup"><span data-stu-id="9358c-123">Add or remove retention tags</span></span>](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/add-or-remove-retention-tags)
- [<span data-ttu-id="9358c-124">Kaip nustatyti pašto dėžutėje esančio sulaikymo tipą</span><span class="sxs-lookup"><span data-stu-id="9358c-124">How to identify the type of hold placed on a mailbox</span></span>](https://docs.microsoft.com/microsoft-365/compliance/identify-a-hold-on-an-exchange-online-mailbox)
