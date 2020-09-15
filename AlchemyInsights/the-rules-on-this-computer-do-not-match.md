---
title: 'Klaida: šiame kompiuteryje taisyklės nesutampa'
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "3518"
- "1800021"
ms.openlocfilehash: c2feb6da651d8b3eb7af6a057335b28d26f9e7f6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47690971"
---
# <a name="error-the-rules-on-this-computer-do-not-match"></a><span data-ttu-id="c61ee-102">Klaida: šiame kompiuteryje taisyklės nesutampa</span><span class="sxs-lookup"><span data-stu-id="c61ee-102">Error: The rules on this computer do not match</span></span>

<span data-ttu-id="c61ee-103">Norėdami pamatyti atnaujintą šios žinomos problemos būseną, skaitykite šiame [kompiuteryje taisyklės nesutampa su "Microsoft Exchange" taisyklėmis](https://support.office.com/article/d032e037-b224-429e-b325-633afde9b5f0)</span><span class="sxs-lookup"><span data-stu-id="c61ee-103">To see updated status of this known issue, see [The rules on this computer do not match the rules on Microsoft Exchange](https://support.office.com/article/d032e037-b224-429e-b325-633afde9b5f0)</span></span>

<span data-ttu-id="c61ee-104">"Outlook" komanda įdiegė 12928,10000 komponavimo versiją.</span><span class="sxs-lookup"><span data-stu-id="c61ee-104">The Outlook Team has implemented a fix in Build 12928.10000.</span></span> <span data-ttu-id="c61ee-105">Pataisyti jau yra "Insider" Sparčioji versija ir pereiti į mėnesinius kanalo 2020 birželio pabaigoje.</span><span class="sxs-lookup"><span data-stu-id="c61ee-105">The fix is already at Insider Fast and will go to Monthly Channel in late June 2020.</span></span> <span data-ttu-id="c61ee-106">Kai jau turite fiksuotą komponavimo versiją, galite gauti raginimą "kurias taisykles norite palikti" paskutinį kartą.</span><span class="sxs-lookup"><span data-stu-id="c61ee-106">Once you have the fixed build you may get the prompt "Which rules do you want to keep" one last time.</span></span> <span data-ttu-id="c61ee-107">Kai būsite paraginti, pasirinkite serveris, tada grįžkite į "Outlook" ir vėl įjunkite visas išjungtas taisykles.</span><span class="sxs-lookup"><span data-stu-id="c61ee-107">Choose Server when prompted and then go back in Outlook and re-enable any rules that were disabled.</span></span>

<span data-ttu-id="c61ee-108">Kol pataisymas bus pasiekiamas, naudokite šį sprendimo būdą:</span><span class="sxs-lookup"><span data-stu-id="c61ee-108">Until the fix is available please use the following workaround:</span></span>

<span data-ttu-id="c61ee-109">**Sprendimo būdas**: naujausioje ataskaitoje atsirado problema dėl tų, kurios sukūrė tik kliento taisykles "Outlook" darbalaukyje.</span><span class="sxs-lookup"><span data-stu-id="c61ee-109">**Workaround**: In recent reports, the issue has occurred for those that have only created client rules in Outlook desktop.</span></span> <span data-ttu-id="c61ee-110">Jei ir toliau susiduriate su problema, apsvarstykite galimybę panaikinti taisykles ir kurti bei redaguoti taisykles tik OWA ("Outlook Web App"), kol problema bus išspręsta.</span><span class="sxs-lookup"><span data-stu-id="c61ee-110">If you continue to run into the problem, consider deleting the rules and then create and edit rules only in OWA (Outlook Web App) until the issue is resolved.</span></span>

<span data-ttu-id="c61ee-111">Jei negalite panaikinti taisyklių rankiniu būdu, galite paleisti "Outlook" komandą paleidę "Outlook" paleisdami Outlook.exe/Cleanrules.</span><span class="sxs-lookup"><span data-stu-id="c61ee-111">If you cannot delete the rules manually you can run an Outlook command when you start Outlook by running Outlook.exe /cleanrules.</span></span> <span data-ttu-id="c61ee-112">Taip panaikinsite ir kliento, ir serverio taisykles.</span><span class="sxs-lookup"><span data-stu-id="c61ee-112">This will delete both the client and server rules.</span></span> <span data-ttu-id="c61ee-113">Bus panaikintos visos visos "Outlook" profilyje esančios paskyros taisyklės.</span><span class="sxs-lookup"><span data-stu-id="c61ee-113">It will delete all of the rules for all of the accounts in the Outlook Profile.</span></span> <span data-ttu-id="c61ee-114">Ši komanda yra toliau dokumentuota komandų eilutės jungiklių straipsnyje.</span><span class="sxs-lookup"><span data-stu-id="c61ee-114">This command is further documented in the Command-line switches article.</span></span>

