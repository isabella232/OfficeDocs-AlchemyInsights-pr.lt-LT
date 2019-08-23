---
title: Saugojimo strategijos, Exchange administravimo centro neveikia
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 11/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "308"
- "3100007"
ms.assetid: a48fd5fd-4af7-4d5f-b617-b0f9334ccaa7
ms.openlocfilehash: 5d7b62546397c13b37540e8797b31123b2880280
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 08/22/2019
ms.locfileid: "36551351"
---
# <a name="retention-policies-in-exchange-admin-center"></a><span data-ttu-id="03efb-102">Saugojimo strategijos, Exchange administravimo centro</span><span class="sxs-lookup"><span data-stu-id="03efb-102">Retention Policies in Exchange Admin Center</span></span>

 <span data-ttu-id="03efb-103">**Klausimas:** Naujai sukurta ar atnaujinta saugojimo strategijos, Exchange administravimo centro netaiko į pašto dėžutes arba nėra perkeliami į archyvo pašto dėžutę arba pašalinus elementus.</span><span class="sxs-lookup"><span data-stu-id="03efb-103">**Issue:** Newly created or updated retention policies in the Exchange Admin Center are not applying to mailboxes or items are not moved to the archive mailbox or deleted.</span></span> 
  
 <span data-ttu-id="03efb-104">**Priežastis:**</span><span class="sxs-lookup"><span data-stu-id="03efb-104">**Root Causes:**</span></span>
  
- <span data-ttu-id="03efb-105">Tai gali būti todėl, kad **Valdomojo aplanko asistentas** ne perdirbo vartotojo pašto dėžutėje.</span><span class="sxs-lookup"><span data-stu-id="03efb-105">This may be because the **Managed Folder Assistant** has not processed the user's mailbox.</span></span> <span data-ttu-id="03efb-106">Valdomojo aplanko asistentas bando tvarkyti kiekvieną pašto dėžutės į nuotolinių išteklių saugyklomis pagrįstos organizacijos kas septynias dienas.</span><span class="sxs-lookup"><span data-stu-id="03efb-106">The Managed Folder Assistant tries to process every mailbox in your cloud-based organization once every seven days.</span></span> <span data-ttu-id="03efb-107">Jei pakeitėte saugojimo žymę arba taikyti kitą saugojimo strategiją pašto dėžutei, galite palaukti, kol valdomas aplankas padeda apdoroja pašto dėžutę, arba galite paleisti Start-ManagedFolderAssistant cmdlet ir paleisti valdomojo aplanko asistentas apdoroti tam tikrą pašto dėžutės.</span><span class="sxs-lookup"><span data-stu-id="03efb-107">If you change a retention tag or apply a different retention policy to a mailbox, you can wait until the Managed Folder Assist processes the mailbox, or you can run the Start-ManagedFolderAssistant cmdlet to start the Managed Folder Assistant to process a specific mailbox.</span></span> <span data-ttu-id="03efb-108">Vykdyti į cmdlet yra naudinga bandyti ar trikčių šalinimo saugojimo strategijos ar saugojimo ˛ymės parametrus.</span><span class="sxs-lookup"><span data-stu-id="03efb-108">Running this cmdlet is useful for testing or troubleshooting a retention policy or retention tag settings.</span></span> <span data-ttu-id="03efb-109">Norėdami gauti daugiau informacijos, apsilankykite [paleisti valdomojo aplanko asistentas](https://msdn.microsoft.com/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist).</span><span class="sxs-lookup"><span data-stu-id="03efb-109">For more information, visit [Run the Managed Folder Assistant](https://msdn.microsoft.com/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist).</span></span>
    
  - <span data-ttu-id="03efb-110">**Sprendimas:** Vykdykite šią komandą pradėti tam tikros pašto dėžutės valdomojo aplanko asistentas:</span><span class="sxs-lookup"><span data-stu-id="03efb-110">**Solution:** Run the following command to start the Managed Folder Assistant for a specific mailbox:</span></span>
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

- <span data-ttu-id="03efb-111">Taip, gali nutikti, jei **RetentionHold** buvo **įjungtas** į pašto dėžutę.</span><span class="sxs-lookup"><span data-stu-id="03efb-111">This may also be occur if **RetentionHold** has been **enabled** on the mailbox.</span></span> <span data-ttu-id="03efb-112">Jei pašto dėžutės buvo skiriamas į RetentionHold, saugojimo strategijos pašto dėžutės bus apdorotos per tą laiką.</span><span class="sxs-lookup"><span data-stu-id="03efb-112">If the mailbox has been placed on a RetentionHold, the retention policy on the mailbox will not be processed during that time.</span></span> <span data-ttu-id="03efb-113">Dėl daugiau pateikiamoje RetentionHold parametrą žr: [Pašto dėžutės saugojimo palaikykite](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).</span><span class="sxs-lookup"><span data-stu-id="03efb-113">For more informaton on the RetentionHold setting see: [Mailbox Retention Hold](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).</span></span>
    
    <span data-ttu-id="03efb-114">**Sprendimas:**</span><span class="sxs-lookup"><span data-stu-id="03efb-114">**Solution:**</span></span>
    
  - <span data-ttu-id="03efb-115">Patikrinkite, ar RetentionHold nustatyti konkrečias [EXO "PowerShell"](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps)pašto dėžutės:</span><span class="sxs-lookup"><span data-stu-id="03efb-115">Check the status of the RetentionHold setting on the specific mailbox in [EXO powershell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps):</span></span>
    
  ```
  Get-Mailbox -Identity <name of the mailbox> |fl *retentionHold*
  ```

  - <span data-ttu-id="03efb-116">Vykdyti šią komandą, Norėdami **išjungti** RetentionHold tam tikros pašto dėžutės:</span><span class="sxs-lookup"><span data-stu-id="03efb-116">Run the following command to **disable** RetentionHold on a specific mailbox:</span></span>
    
  ```
  Set-Mailbox -RetentionHoldEnabled $false
  ```

  - <span data-ttu-id="03efb-117">Dabar, naujo paleisti valdomos aplanko asistentas:</span><span class="sxs-lookup"><span data-stu-id="03efb-117">Now, re-run the Managed folder Assistant:</span></span>
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

 <span data-ttu-id="03efb-118">**Pastaba:** Jei pašto dėžutės yra mažesnis nei 10 MB, valdomojo aplanko asistentas nebus automatiškai apdorojami, pašto dėžutės.</span><span class="sxs-lookup"><span data-stu-id="03efb-118">**Note:** If a mailbox is smaller than 10 MB, the Managed Folder Assistant will not automatically process the mailbox.</span></span>
 
<span data-ttu-id="03efb-119">Daugiau informacijos apie saugojimo strategijos, Exchange administravimo centro, žr.:</span><span class="sxs-lookup"><span data-stu-id="03efb-119">For more info on retention policies in the Exchange Admin Center, see:</span></span>
- [<span data-ttu-id="03efb-120">Saugojimo ˛ymes ir saugojimo strategijos</span><span class="sxs-lookup"><span data-stu-id="03efb-120">Retention tags and retention policies</span></span>](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/retention-tags-and-policies)
- [<span data-ttu-id="03efb-121">Taikyti saugojimo strategijos į pašto dėžutes</span><span class="sxs-lookup"><span data-stu-id="03efb-121">Apply a retention policy to mailboxes</span></span>](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy)
- [<span data-ttu-id="03efb-122">Pridėti arba pašalinti saugojimo žymes</span><span class="sxs-lookup"><span data-stu-id="03efb-122">Add or remove retention tags</span></span>](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/add-or-remove-retention-tags)
- [<span data-ttu-id="03efb-123">Kaip nustatyti tos rūšies palaikykite ant pašto dėžutės</span><span class="sxs-lookup"><span data-stu-id="03efb-123">How to identify the type of hold placed on a mailbox</span></span>](https://docs.microsoft.com/office365/securitycompliance/identify-a-hold-on-an-exchange-online-mailbox)
