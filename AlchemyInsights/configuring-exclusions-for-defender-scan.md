---
title: Išimčių konfigūravimas "Microsoft" sargybos ATP nuskaitymas
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/16/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6027"
- "9001464"
ms.openlocfilehash: 5eb18f4133aca93c1506f4975c8d0567bede8d57
ms.sourcegitcommit: f4866e94918c7b591ad0cd3b58169d340bcc7f00
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 05/19/2021
ms.locfileid: "52543693"
---
# <a name="configuring-exclusions-for-microsoft-defender-atp-scan"></a><span data-ttu-id="eb023-102">Išimčių konfigūravimas "Microsoft" sargybos ATP nuskaitymas</span><span class="sxs-lookup"><span data-stu-id="eb023-102">Configuring exclusions for Microsoft Defender ATP scan</span></span>

<span data-ttu-id="eb023-103">Paprastai galite neįtraukti tam tikrų failų plėtinių ir aplankų vietų į "Microsoft" sargybos ATP nuskaitymą.</span><span class="sxs-lookup"><span data-stu-id="eb023-103">In general, you can exclude certain file extensions and folder locations from Microsoft Defender ATP scans.</span></span> <span data-ttu-id="eb023-104">Taip pat galite konfigūruoti tam tikrų procesų atidarytų failų išimtis.</span><span class="sxs-lookup"><span data-stu-id="eb023-104">You can also configure exclusions for files opened by certain processes.</span></span> <span data-ttu-id="eb023-105">Daugiau informacijos žr. Išimčių [konfigūravimas ir tikrintas](/windows/security/threat-protection/microsoft-defender-antivirus/configure-extension-file-exclusions-microsoft-defender-antivirus) atsižvelgiant į failų plėtinį ir aplanko vietą bei Procesų [atidarytų failų išimčių konfigūravimas.](/windows/security/threat-protection/microsoft-defender-antivirus/configure-process-opened-file-exclusions-microsoft-defender-antivirus)</span><span class="sxs-lookup"><span data-stu-id="eb023-105">For more info, see, [Configure and validate exclusions based on file extension and folder location](/windows/security/threat-protection/microsoft-defender-antivirus/configure-extension-file-exclusions-microsoft-defender-antivirus) and [Configure exclusions for files opened by processes](/windows/security/threat-protection/microsoft-defender-antivirus/configure-process-opened-file-exclusions-microsoft-defender-antivirus) .</span></span>

<span data-ttu-id="eb023-106">Norėdami konfigūruoti **"Windows Server 2016" ir "Server 2019"** išimtis , žr. [""Microsoft" sargybos antivirusinė programa Server" Windows išimčių konfigūravimas](/windows/security/threat-protection/microsoft-defender-antivirus/configure-server-exclusions-microsoft-defender-antivirus).</span><span class="sxs-lookup"><span data-stu-id="eb023-106">To configure exclusions for  **Windows Server 2016 and 2019**, see [Configure Microsoft Defender Antivirus exclusions on Windows Server](/windows/security/threat-protection/microsoft-defender-antivirus/configure-server-exclusions-microsoft-defender-antivirus).</span></span>

<span data-ttu-id="eb023-107">**"Mac"**</span><span class="sxs-lookup"><span data-stu-id="eb023-107">**Mac**</span></span>

<span data-ttu-id="eb023-108">Daugiau informacijos apie palaikomus išimčių tipus ir "Mac" išimčių sąrašo konfigūravimą žr. Palaikomi išimčių tipai ir Kaip [konfigūruoti išimčių sąrašą](/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#how-to-configure-the-list-of-exclusions). [](/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#supported-exclusion-types)</span><span class="sxs-lookup"><span data-stu-id="eb023-108">For details on supported exclusion types and configuring a list of exclusions for Mac, see [Supported exclusion types](/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#supported-exclusion-types) and [How to configure the list of exclusions](/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#how-to-configure-the-list-of-exclusions).</span></span>

<span data-ttu-id="eb023-109">**Pastaba** Taip pat galite patikrinti išimčių sąrašus naudodami BANDOMĄJĮ FAILĄ EICAR.</span><span class="sxs-lookup"><span data-stu-id="eb023-109">**Note** You can also validate exclusions lists using the EICAR test file.</span></span> <span data-ttu-id="eb023-110">Daugiau informacijos žr. [Išimčių sąrašų tikrinimas naudojant EICAR bandomąjį failą](/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#validate-exclusions-lists-with-the-eicar-test-file).</span><span class="sxs-lookup"><span data-stu-id="eb023-110">For more info, see [Validate exclusions lists with the EICAR test file](/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#validate-exclusions-lists-with-the-eicar-test-file).</span></span> 

<span data-ttu-id="eb023-111">**"Linux"**</span><span class="sxs-lookup"><span data-stu-id="eb023-111">**Linux**</span></span>

<span data-ttu-id="eb023-112">Daugiau informacijos apie palaikomus išimčių tipus ir "Linux" išimčių sąrašo konfigūravimą žr. Palaikomi išimčių tipai ir ["Linux" skirtų ""Microsoft" sargybos ATP" išimčių konfigūravimas ir "Microsoft" sargybos ATP.](/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions) [](/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions#supported-exclusion-types)</span><span class="sxs-lookup"><span data-stu-id="eb023-112">For details on supported exclusion types and configuring a list of exclusions for Linux, see [Supported exclusion types](/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions#supported-exclusion-types) and [Configure and validate exclusions for Microsoft Defender ATP for Linux](/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions).</span></span>

<span data-ttu-id="eb023-113">**Pastaba** Taip pat galite patikrinti išimčių sąrašus naudodami BANDOMĄJĮ FAILĄ EICAR.</span><span class="sxs-lookup"><span data-stu-id="eb023-113">**Note** You can also validate exclusions lists using the EICAR test file.</span></span> <span data-ttu-id="eb023-114">Daugiau informacijos žr. [Išimčių sąrašų tikrinimas naudojant EICAR bandomąjį failą](/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions#validate-exclusions-lists-with-the-eicar-test-file).</span><span class="sxs-lookup"><span data-stu-id="eb023-114">For more info, see [Validate exclusions lists with the EICAR test file](/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions#validate-exclusions-lists-with-the-eicar-test-file).</span></span> 