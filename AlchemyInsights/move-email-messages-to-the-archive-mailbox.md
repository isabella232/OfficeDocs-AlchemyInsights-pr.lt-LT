---
title: Perkelti el. laiškus į archyvo pašto dėžutę
ms.author: cmcatee
author: cmcatee-MSFT
manager: mnirkhe
ms.date: 11/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 59cd8630-6196-4680-ad92-1ce0e479f924
ms.openlocfilehash: a631af20e28a531a40f078e290239a372c38ab74
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 02/12/2019
ms.locfileid: "29941722"
---
<span data-ttu-id="9b225-p101">Problemų archyvuoti elementus į archyvo pašto dėžutę. Įsitikinkite, kad turite atlikti šiuos veiksmus:</span><span class="sxs-lookup"><span data-stu-id="9b225-p101">Having problems archiving items to the Archive mailbox. Make sure you have performed the following steps:</span></span>
  
1. <span data-ttu-id="9b225-p102">Patvirtinkite, kad **archyvo pašto dėžutės** įgalintas. Jei ne, atlikite veiksmus [šiame](https://docs.microsoft.com/office365/securitycompliance/enable-archive-mailboxes) straipsnyje, kad archyvo pašto dėžutę.</span><span class="sxs-lookup"><span data-stu-id="9b225-p102">Confirm that an **Archive mailbox** has been enabled. If not, use steps in [this article](https://docs.microsoft.com/office365/securitycompliance/enable-archive-mailboxes) to enable the archive mailbox.</span></span> 
    
2. <span data-ttu-id="9b225-106">Exchange administravimo centro, pasirinkite **Saugojimo ˛ymes** pagal **Reikalavimų laikymosi valdymas**, sukurti **saugojimo žymę** **perkelti į archyvą** veiksmų, kuriame yra norimas **Saugojimo laiką**.</span><span class="sxs-lookup"><span data-stu-id="9b225-106">In the Exchange Admin Center, select **Retention Tags** under **Compliance Management**, create a **Retention tag** with the **Move to Archive** action containing the desired **Retention Age**.</span></span>
    
3. <span data-ttu-id="9b225-107">Exchange administravimo centro, pasirinkite **Saugojimo strategijas**, sukurti **Saugojimo strategija** ir pridėti savo **perkelti į archyvo** saugojimo žymę prie tos politikos.</span><span class="sxs-lookup"><span data-stu-id="9b225-107">In the Exchange Admin Center, select **Retention Policies**, create a **Retention Policy** and add your **Move to Archive** retention tag to that policy.</span></span> 
    
4. <span data-ttu-id="9b225-p103">[Priskirti saugojimo strategijos](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) konkretaus vartotojo pašto dėžutėje. Ta pačia sutartimi taikysite į **pirminį** ir **archyvo** pašto dėžutę.</span><span class="sxs-lookup"><span data-stu-id="9b225-p103">[Assign the Retention Policy](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) to the specific user's mailbox. The same policy will be applied to both the **Primary** and the **Archive** mailbox.</span></span> 
    
<span data-ttu-id="9b225-p104">Vartotojo pašto dėžutės dabar yra archyvavimo strategija galite perkelti elementus į archyvo pašto dėžutę. Reikia priversti valdomos aplanko asistentas (URM) vykdyti ir taikyti naujus parametrus vartotojo pašto dėžutėje. Vykdykite šią komandą kol [prijungtas prie EXO "PowerShell"](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) pradėti tam tikros pašto dėžutės valdomojo aplanko asistentas:</span><span class="sxs-lookup"><span data-stu-id="9b225-p104">The user's mailbox should now have an Archive policy to move items to the Archive mailbox. It may be necessary to force the Managed Folder Assistant (MFA) to run and apply the new settings to the user's mailbox. Run the following command while [connected to EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) to start the Managed Folder Assistant for a specific mailbox:</span></span> 
  
```
Start-ManagedFolderAssistant -Identity <name of the mailbox>
```

<span data-ttu-id="9b225-113">Norite gauti daugiau informacijos apie archyvavimo strategijos nustatymas, žiūrėkite [nustatyti archyvavimo ir naikinimo politiką pašto dėžučių](https://docs.microsoft.com/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).</span><span class="sxs-lookup"><span data-stu-id="9b225-113">Want more information on setting up an archive policy, see [Set up an archive and deletion policy for mailboxes](https://docs.microsoft.com/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).</span></span>
  

