---
title: Replikų rinkinys
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004400"
- "9004395"
- "8265"
- "9276"
ms.openlocfilehash: 3834696ff59b7e96e90a5b660a489003dfa9729c
ms.sourcegitcommit: 581c696ec108184adae9d4bc8f47cb9247131de8
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 03/10/2021
ms.locfileid: "50714251"
---
# <a name="replica-set"></a><span data-ttu-id="bcac1-102">Replikų rinkinys</span><span class="sxs-lookup"><span data-stu-id="bcac1-102">Replica set</span></span>

<span data-ttu-id="bcac1-103">"AADDS" taip pat vadinama valdomu domenu.</span><span class="sxs-lookup"><span data-stu-id="bcac1-103">AADDS is also called as the managed domain.</span></span> <span data-ttu-id="bcac1-104">Tai iš tikrųjų yra du domeno valdikliai, kurie vykdomi ir prižiūrimi backend.</span><span class="sxs-lookup"><span data-stu-id="bcac1-104">It is actually two domain controllers that are run and maintained by the backend.</span></span> <span data-ttu-id="bcac1-105">Du DC apima vieną pagrindinį DC ir vieną replikavimo DC.</span><span class="sxs-lookup"><span data-stu-id="bcac1-105">The two DCs include one main DC and one replication DC.</span></span> <span data-ttu-id="bcac1-106">Atsarginės kopijos, esančios AADDS (valdomas domenas), yra automatinis procesas, kurį tvarko "Azure" platforma.</span><span class="sxs-lookup"><span data-stu-id="bcac1-106">Backups in AADDS (managed domain) are an automated process managed by the Azure platform.</span></span> <span data-ttu-id="bcac1-107">Kilus problemai su valdomu domenu, "Azure" palaikymas gali padėti atkurti atsarginę kopiją.</span><span class="sxs-lookup"><span data-stu-id="bcac1-107">In the event of an issue with your managed domain, Azure support can assist you in restoring from backup.</span></span>

<span data-ttu-id="bcac1-108">Sukuriate kiekvieną replikų rinkinį virtualiame tinkle.</span><span class="sxs-lookup"><span data-stu-id="bcac1-108">You create each replica set in a virtual network.</span></span> <span data-ttu-id="bcac1-109">Kiekvienas virtualusis tinklas turi būti valdomas visiems kitiems virtualiam tinklui, kuriame yra valdomo domeno replikų rinkinys.</span><span class="sxs-lookup"><span data-stu-id="bcac1-109">Each virtual network must be peered to every other virtual network that hosts a managed domain's replica set.</span></span> <span data-ttu-id="bcac1-110">Ši konfigūracija sukuria tinklinio tinklo topologiją, kuri palaiko katalogų replikavimą.</span><span class="sxs-lookup"><span data-stu-id="bcac1-110">This configuration creates a mesh network topology that supports directory replication.</span></span> <span data-ttu-id="bcac1-111">Virtualiame tinkle gali būti palaikomi keli replikų rinkiniai, jei kiekvienas replikų rinkinys yra kitame virtualiame potinklyje.</span><span class="sxs-lookup"><span data-stu-id="bcac1-111">A virtual network can support multiple replica sets, provided that each replica set is in a different virtual subnet.</span></span>

<span data-ttu-id="bcac1-112">Daugiau informacijos apie replikų rinkinį ieškokite [koncepcijų replikų rinkiniai](https://docs.microsoft.com/azure/active-directory-domain-services/concepts-replica-sets).</span><span class="sxs-lookup"><span data-stu-id="bcac1-112">For more details on Replica set, see [Concepts Replica sets](https://docs.microsoft.com/azure/active-directory-domain-services/concepts-replica-sets).</span></span>
