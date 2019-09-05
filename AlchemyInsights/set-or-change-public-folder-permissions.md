---
title: Viešųjų aplankų teisių nustatymas arba keitimas
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 8/27/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: cffdf9bf-34ce-40f6-a69e-d02f17d9caef
ms.openlocfilehash: 1015c2203406e15d6b418c387b6632a182d6d2ff
ms.sourcegitcommit: a256e8680379c006287ae30996763051c4d9ff85
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 09/04/2019
ms.locfileid: "36734677"
---
# <a name="permissions-and-public-folders"></a><span data-ttu-id="3215a-102">Teisės ir viešieji aplankai</span><span class="sxs-lookup"><span data-stu-id="3215a-102">Permissions and Public Folders</span></span>

<span data-ttu-id="3215a-103">Galite pakeisti teises į viešąjį aplanką naudodami "Outlook", Exchange administravimo centro (EAC) arba "PowerShell":</span><span class="sxs-lookup"><span data-stu-id="3215a-103">You can change the permissions on your Public Folders using Outlook, the Exchange admin center (EAC), or PowerShell:</span></span>
  
- <span data-ttu-id="3215a-104">Norėdami gauti "Outlook" instrukcijų, [spustelėkite čia](https://support.office.com/article/Set-or-change-permissions-for-a-public-folder-b2e0440c-7873-48ec-9ff2-b1a20b723005.aspx).</span><span class="sxs-lookup"><span data-stu-id="3215a-104">For Outlook instructions, [click here](https://support.office.com/article/Set-or-change-permissions-for-a-public-folder-b2e0440c-7873-48ec-9ff2-b1a20b723005.aspx).</span></span>
    
- <span data-ttu-id="3215a-105">EAC, ieškokite [šiame straipsnyje](https://technet.microsoft.com/library/jj651147%28v=exchg.150%29.aspx.aspx#Anchor_1) nurodymų.</span><span class="sxs-lookup"><span data-stu-id="3215a-105">For EAC, refer to [this article](https://technet.microsoft.com/library/jj651147%28v=exchg.150%29.aspx.aspx#Anchor_1) for instructions.</span></span> 
    
- <span data-ttu-id="3215a-106">"PowerShell", skaitykite [šį straipsnį](https://technet.microsoft.com/library/bb124743%28v=exchg.160%29.aspx.aspx) instrukcijų, kaip naudoti pridėti PublicFolderClientPermission commandlet.</span><span class="sxs-lookup"><span data-stu-id="3215a-106">For Powershell, refer to [this article](https://technet.microsoft.com/library/bb124743%28v=exchg.160%29.aspx.aspx) for instructions on using the Add-PublicFolderClientPermission commandlet.</span></span> <span data-ttu-id="3215a-107">Jei jums reikia nurodymų, kaip prisijungti prie Exchange PowerShell, spustelėkite [čia](https://technet.microsoft.com/library/jj984289%28v=exchg.160%29.aspx.aspx).</span><span class="sxs-lookup"><span data-stu-id="3215a-107">If you need instructions to connect to Exchange Powershell, click [here](https://technet.microsoft.com/library/jj984289%28v=exchg.160%29.aspx.aspx).</span></span>
    
<span data-ttu-id="3215a-108">Jei **Išoriniai vartotojai negali siųsti el. laiškų į pašto viešąjį aplanką**, gali būti, kad viešajame aplanke trūksta teisių, reikalingų išoriniam el. pašto pristatymui.</span><span class="sxs-lookup"><span data-stu-id="3215a-108">If **external users can't send emails to a mail-enabled Public Folder**, the reason might be that the public folder is missing permissions required for external email delivery.</span></span> <span data-ttu-id="3215a-109">Galite išspręsti šią problemą naudodami "Outlook" instrukcijos [čia](https://technet.microsoft.com/library/aa997560%28v=exchg.150%29.aspx.aspx#Anchor_1), arba "PowerShell" instrukcijas [čia](https://support.microsoft.com/help/2984402/-5.7.1-smtp-550-5.7.1-resolver.rst.authrequired-nondelivery-report-when-external-users-try-to-send-mail-to-mail-enabled-public-folders-in-office-365.aspx).</span><span class="sxs-lookup"><span data-stu-id="3215a-109">You can fix this using the Outlook instructions [here](https://technet.microsoft.com/library/aa997560%28v=exchg.150%29.aspx.aspx#Anchor_1), or the PowerShell instructions [here](https://support.microsoft.com/help/2984402/-5.7.1-smtp-550-5.7.1-resolver.rst.authrequired-nondelivery-report-when-external-users-try-to-send-mail-to-mail-enabled-public-folders-in-office-365.aspx).</span></span>
  

