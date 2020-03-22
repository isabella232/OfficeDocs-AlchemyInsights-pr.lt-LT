---
title: Nepavyksta pasiekti viešųjų aplankų
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "3462"
ms.openlocfilehash: a579b89b68bfb8432adfe64b155803eda2c3b086
ms.sourcegitcommit: a3b42ee05224846327d353b48a8c67dab724f6eb
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 03/21/2020
ms.locfileid: "42891757"
---
# <a name="outlook-cannot-connect-to-public-folders"></a><span data-ttu-id="4bc19-102">Programa Outlook negali prisijungti prie viešųjų aplankų</span><span class="sxs-lookup"><span data-stu-id="4bc19-102">Outlook cannot connect to public folders</span></span>

<span data-ttu-id="4bc19-103">Jei kai kuriems vartotojams viešojo aplanko prieiga neveikia, pabandykite atlikti šiuos veiksmus:</span><span class="sxs-lookup"><span data-stu-id="4bc19-103">If public folder access isn't working for some users, try the following:</span></span>

<span data-ttu-id="4bc19-104">Prisijunkite prie EXO "PowerShell" ir sukonfigūruokite parametrą DefaultPublicFolderMailbox problemos vartotojo abonemente, kad atitiktų parametrą, esantį veikiančiame vartotojo abonemente.</span><span class="sxs-lookup"><span data-stu-id="4bc19-104">Connect to EXO PowerShell and configure the DefaultPublicFolderMailbox parameter on the problem user account to match the parameter on a working user account.</span></span>

<span data-ttu-id="4bc19-105">Pavyzdys:</span><span class="sxs-lookup"><span data-stu-id="4bc19-105">Example:</span></span>

<span data-ttu-id="4bc19-106">Get-Mailbox WorkingUser | ft DefaultPublicFolderMailbox,EffectivePublicFolderMailbox ft DefaultPublicFolderMailbox, EffectivePublicFolderMailbox ft DefaultPublicFolderMailbox, EffectivePublicFolderMailbox ft Default</span><span class="sxs-lookup"><span data-stu-id="4bc19-106">Get-Mailbox WorkingUser | ft DefaultPublicFolderMailbox,EffectivePublicFolderMailbox</span></span>

<span data-ttu-id="4bc19-107">Set-Mailbox ProblemUser -DefaultPublicFolderMailbox \<reikšmė iš ankstesnės komandos></span><span class="sxs-lookup"><span data-stu-id="4bc19-107">Set-Mailbox ProblemUser -DefaultPublicFolderMailbox \<value from previous command></span></span>

<span data-ttu-id="4bc19-108">Palaukite bent vieną valandą, kol pakeitimas įsigalios.</span><span class="sxs-lookup"><span data-stu-id="4bc19-108">Wait at least one hour for the change to take effect.</span></span>

<span data-ttu-id="4bc19-109">Jei problema išlieka, atlikite [šią procedūrą,](https://aka.ms/pfcte) norėdami išspręsti viešųjų aplankų prieigos problemas naudodami "Outlook".</span><span class="sxs-lookup"><span data-stu-id="4bc19-109">If the issue remains, please follow [this procedure](https://aka.ms/pfcte) to troubleshoot public folder access issues using Outlook.</span></span>