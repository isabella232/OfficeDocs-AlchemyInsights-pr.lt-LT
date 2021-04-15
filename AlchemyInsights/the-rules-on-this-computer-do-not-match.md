---
title: 'Klaida: šio kompiuterio taisyklės nesutampa'
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "3518"
- "1800021"
ms.openlocfilehash: c46eb856baafbef9bc3b7fa34a0258ef16923fb8
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 04/15/2021
ms.locfileid: "51782960"
---
# <a name="error-the-rules-on-this-computer-do-not-match"></a><span data-ttu-id="ac012-102">Klaida: šio kompiuterio taisyklės nesutampa</span><span class="sxs-lookup"><span data-stu-id="ac012-102">Error: The rules on this computer do not match</span></span>

<span data-ttu-id="ac012-103">Norėdami pamatyti atnaujintą šios žinomos problemos būseną, žr. Šio kompiuterio [taisyklės neatitinka "Microsoft Exchange" taisyklių](https://support.office.com/article/d032e037-b224-429e-b325-633afde9b5f0)</span><span class="sxs-lookup"><span data-stu-id="ac012-103">To see updated status of this known issue, see [The rules on this computer do not match the rules on Microsoft Exchange](https://support.office.com/article/d032e037-b224-429e-b325-633afde9b5f0)</span></span>

<span data-ttu-id="ac012-104">"Outlook" komanda įdiegė pataisą 12928.10000 komponavimo versija.</span><span class="sxs-lookup"><span data-stu-id="ac012-104">The Outlook Team has implemented a fix in Build 12928.10000.</span></span> <span data-ttu-id="ac012-105">Pataisa jau yra "Insider Fast" ir 2020 m. birželio pabaigoje bus pereis į Mėnesinis kanalas.</span><span class="sxs-lookup"><span data-stu-id="ac012-105">The fix is already at Insider Fast and will go to Monthly Channel in late June 2020.</span></span> <span data-ttu-id="ac012-106">Kai turite fiksuotą komponavimo versiją, paskutinį kartą galite gauti raginimą "Kurias taisykles norite išsaugoti".</span><span class="sxs-lookup"><span data-stu-id="ac012-106">Once you have the fixed build you may get the prompt "Which rules do you want to keep" one last time.</span></span> <span data-ttu-id="ac012-107">Kai būsite paraginti, pasirinkite Serveris, tada grįžkite į "Outlook" ir vėl įgalinkite visas išjungtas taisykles.</span><span class="sxs-lookup"><span data-stu-id="ac012-107">Choose Server when prompted and then go back in Outlook and re-enable any rules that were disabled.</span></span>

<span data-ttu-id="ac012-108">Kol pataisa bus pasiekiama, naudokite šį sprendimo būdą:</span><span class="sxs-lookup"><span data-stu-id="ac012-108">Until the fix is available please use the following workaround:</span></span>

<span data-ttu-id="ac012-109">**Sprendimo būdas:** naujausiose ataskaitose problema kilo tiems, kurie sukūrė kliento taisykles tik "Outlook" kompiuteryje.</span><span class="sxs-lookup"><span data-stu-id="ac012-109">**Workaround**: In recent reports, the issue has occurred for those that have only created client rules in Outlook desktop.</span></span> <span data-ttu-id="ac012-110">Jei ir toliau kyla problema, apsvarstykite galimybę panaikinti taisykles, tada kurti ir redaguoti taisykles tik OWA ("Outlook Web App"), kol problema bus išspręsta.</span><span class="sxs-lookup"><span data-stu-id="ac012-110">If you continue to run into the problem, consider deleting the rules and then create and edit rules only in OWA (Outlook Web App) until the issue is resolved.</span></span>

<span data-ttu-id="ac012-111">Jei negalite panaikinti taisyklių rankiniu būdu, galite paleisti "Outlook" komandą, kai paleidžiate "Outlook" paleisdami Outlook.exe /cleanrules.</span><span class="sxs-lookup"><span data-stu-id="ac012-111">If you cannot delete the rules manually you can run an Outlook command when you start Outlook by running Outlook.exe /cleanrules.</span></span> <span data-ttu-id="ac012-112">Tai panaikins kliento ir serverio taisykles.</span><span class="sxs-lookup"><span data-stu-id="ac012-112">This will delete both the client and server rules.</span></span> <span data-ttu-id="ac012-113">Jis panaikins visas visų "Outlook" profilio paskyrų taisykles.</span><span class="sxs-lookup"><span data-stu-id="ac012-113">It will delete all of the rules for all of the accounts in the Outlook Profile.</span></span> <span data-ttu-id="ac012-114">Ši komanda toliau dokumentuota straipsnyje Komandų eilutės jungikliai.</span><span class="sxs-lookup"><span data-stu-id="ac012-114">This command is further documented in the Command-line switches article.</span></span>

