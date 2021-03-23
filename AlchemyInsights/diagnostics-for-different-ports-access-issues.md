---
title: Įvairių prievadų prieigos trikčių diagnostika
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9035"
- "9005220"
ms.openlocfilehash: 3673067cad7ac55f3820422dc2ec09942c393149
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 03/19/2021
ms.locfileid: "51035779"
---
# <a name="diagnostics-for-different-ports-access-issues"></a><span data-ttu-id="70e70-102">Įvairių prievadų prieigos trikčių diagnostika</span><span class="sxs-lookup"><span data-stu-id="70e70-102">Diagnostics for different ports access issues</span></span>

<span data-ttu-id="70e70-103">Norėdami išspręsti skirtingas prievadų prieigos problemas, atlikite šiuos veiksmus:</span><span class="sxs-lookup"><span data-stu-id="70e70-103">To resolve the different port access issues, perform the following steps:</span></span>

1. <span data-ttu-id="70e70-104">Stop/dealrasti virtualios mašinos (VM) iš portalo, iš naujo paleiskite VM ir bandykite dar kartą.</span><span class="sxs-lookup"><span data-stu-id="70e70-104">Stop/deallocate the virtual machine (VM) from the portal, restart the VM, and test again.</span></span> 
2. <span data-ttu-id="70e70-105">Patikrinkite VM tinklo parametrus, kad nustatytumėte, ar turite tinklo saugos grupes (NSGs) blokuoja srautą.</span><span class="sxs-lookup"><span data-stu-id="70e70-105">Check your VM's network settings to determine if you have Network Security Groups (NSGs) blocking traffic.</span></span> <span data-ttu-id="70e70-106">Taip pat galite naudoti [tinklo watcher IP srauto tikrinimo įrankį](https://docs.microsoft.com/azure/network-watcher/network-watcher-ip-flow-verify-overview?WT.mc_id=Portal-Microsoft_Azure_Support) , kad patikrintumėte, ar yra nsgs blokavimas srauto, User-Defined maršrutų (udrs) nukreipia srautą atgal į vietinę ("Numatytasis maršrutas ' 0.0.0.0/0) arba tinklo Appliance.</span><span class="sxs-lookup"><span data-stu-id="70e70-106">You can also use [Network Watcher's IP flow verify tool](https://docs.microsoft.com/azure/network-watcher/network-watcher-ip-flow-verify-overview?WT.mc_id=Portal-Microsoft_Azure_Support) to check for NSGs blocking traffic, User-Defined Routes (UDRs) rerouting your traffic back to on-premises ('Default Route' 0.0.0.0/0), or to a network appliance.</span></span>
<span data-ttu-id="70e70-107">Jei vis dar kyla problemų bandant atlikti anksčiau nurodytus veiksmus, pateikite VM pavadinimą ir TCP prievadą, kurį mėginate siųsti paštu tolesniam diagnozavimui.</span><span class="sxs-lookup"><span data-stu-id="70e70-107">If you still experience issues after trying the steps above, please provide the VM name and the TCP port you are attempting to send mail on for further diagnosis.</span></span>

<span data-ttu-id="70e70-108">**Rekomenduojami dokumentai**</span><span class="sxs-lookup"><span data-stu-id="70e70-108">**Recommended Documents**</span></span>

[<span data-ttu-id="70e70-109">Siuntimo elektroninio pašto siuntimo per 25 prievadą apribojimai ir rekomendacijos</span><span class="sxs-lookup"><span data-stu-id="70e70-109">Limitations and recommendations for sending outbound email over port 25</span></span>](https://docs.microsoft.com/azure/virtual-network/troubleshoot-outbound-smtp-connectivity)