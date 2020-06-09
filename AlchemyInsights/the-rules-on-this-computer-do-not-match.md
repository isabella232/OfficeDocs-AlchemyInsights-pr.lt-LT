---
title: 'Klaida: šio kompiuterio taisyklės nesutampa'
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "3518"
- "1800021"
ms.openlocfilehash: ecc1e5ec741cc90c58698991c3a3135f87c39938
ms.sourcegitcommit: 9816ac4d0fef20558383a491e0e76b79c56323f5
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 06/09/2020
ms.locfileid: "44618021"
---
# <a name="error-the-rules-on-this-computer-do-not-match"></a><span data-ttu-id="566cc-102">Klaida: šio kompiuterio taisyklės nesutampa</span><span class="sxs-lookup"><span data-stu-id="566cc-102">Error: The rules on this computer do not match</span></span>

<span data-ttu-id="566cc-103">Norėdami pamatyti atnaujintą būseną šią žinomą problemą, [ieškokite šio kompiuterio taisyklės neatitinka Microsoft Exchange taisykles](https://support.office.com/article/d032e037-b224-429e-b325-633afde9b5f0)</span><span class="sxs-lookup"><span data-stu-id="566cc-103">To see updated status of this known issue, see [The rules on this computer do not match the rules on Microsoft Exchange](https://support.office.com/article/d032e037-b224-429e-b325-633afde9b5f0)</span></span>

<span data-ttu-id="566cc-104">"Outlook" komanda įdiegė nustatyti sukurti 12928.10000.</span><span class="sxs-lookup"><span data-stu-id="566cc-104">The Outlook Team has implemented a fix in Build 12928.10000.</span></span> <span data-ttu-id="566cc-105">Nustatyti jau Viešai ne "Insider Fast" ir bus eiti į mėnesio kanalą birželio pabaigoje 2020.</span><span class="sxs-lookup"><span data-stu-id="566cc-105">The fix is already at Insider Fast and will go to Monthly Channel in late June 2020.</span></span> <span data-ttu-id="566cc-106">Kai jūs turite fiksuotą statyti galite gauti eilutę "Kokios taisyklės norite išlaikyti" paskutinį kartą.</span><span class="sxs-lookup"><span data-stu-id="566cc-106">Once you have the fixed build you may get the prompt "Which rules do you want to keep" one last time.</span></span> <span data-ttu-id="566cc-107">Pasirinkite serverio, kai būsite paraginti ir tada grįžti į "Outlook" ir iš naujo įgalinti visas taisykles, kurios buvo išjungtos.</span><span class="sxs-lookup"><span data-stu-id="566cc-107">Choose Server when prompted and then go back in Outlook and re-enable any rules that were disabled.</span></span>

<span data-ttu-id="566cc-108">Kol taisyti yra, naudokite šiuos problemos sprendimo veiksmus:</span><span class="sxs-lookup"><span data-stu-id="566cc-108">Until the fix is available please use the following workaround:</span></span>

<span data-ttu-id="566cc-109">**Sprendimo būdas**: Naujausiose ataskaitose problema kilo tiems, kurie "Outlook" darbalaukyje sukūrė tik kliento taisykles.</span><span class="sxs-lookup"><span data-stu-id="566cc-109">**Workaround**: In recent reports, the issue has occurred for those that have only created client rules in Outlook desktop.</span></span> <span data-ttu-id="566cc-110">Jei ir toliau kyla problema, apsvarstykite galimybę panaikinti taisykles ir tada kurti ir redaguoti taisykles tik OWA (Outlook Web App), kol problema bus išspręsta.</span><span class="sxs-lookup"><span data-stu-id="566cc-110">If you continue to run into the problem, consider deleting the rules and then create and edit rules only in OWA (Outlook Web App) until the issue is resolved.</span></span>

<span data-ttu-id="566cc-111">Jei negalite panaikinti taisykles rankiniu būdu galite paleisti "Outlook" komandą paleidus programą Outlook paleisdami Outlook.exe /cleanrules.</span><span class="sxs-lookup"><span data-stu-id="566cc-111">If you cannot delete the rules manually you can run an Outlook command when you start Outlook by running Outlook.exe /cleanrules.</span></span> <span data-ttu-id="566cc-112">Tai panaikins kliento ir serverio taisykles.</span><span class="sxs-lookup"><span data-stu-id="566cc-112">This will delete both the client and server rules.</span></span> <span data-ttu-id="566cc-113">Tai ištrins visas taisykles visoms "Outlook" profilio paskyroms.</span><span class="sxs-lookup"><span data-stu-id="566cc-113">It will delete all of the rules for all of the accounts in the Outlook Profile.</span></span> <span data-ttu-id="566cc-114">Ši komanda toliau aprašyta straipsnyje Komandinės eilutės raktai.</span><span class="sxs-lookup"><span data-stu-id="566cc-114">This command is further documented in the Command-line switches  article.</span></span>