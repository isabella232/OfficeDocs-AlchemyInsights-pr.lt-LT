---
title: "\"Microsoft Defender ATP Scan\" išimčių konfigūravimas"
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
ms.openlocfilehash: 912e77b9b1a149fef373f2d0814fb2f0671a48c6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 09/14/2020
ms.locfileid: "50713899"
---
# <a name="configuring-exclusions-for-microsoft-defender-atp-scan"></a><span data-ttu-id="806b7-102">"Microsoft Defender ATP Scan" išimčių konfigūravimas</span><span class="sxs-lookup"><span data-stu-id="806b7-102">Configuring exclusions for Microsoft Defender ATP scan</span></span>

<span data-ttu-id="806b7-103">Paprastai galite neįtraukti tam tikrų failų plėtinių ir aplankų vietų iš "Microsoft Defender ATP" nuskaitymo.</span><span class="sxs-lookup"><span data-stu-id="806b7-103">In general, you can exclude certain file extensions and folder locations from Microsoft Defender ATP scans.</span></span> <span data-ttu-id="806b7-104">Taip pat galite sukonfigūruoti tam tikrų procesų atidarytiems failams skirtas išimtis.</span><span class="sxs-lookup"><span data-stu-id="806b7-104">You can also configure exclusions for files opened by certain processes.</span></span> <span data-ttu-id="806b7-105">Daugiau informacijos ieškokite, [Konfigūruokite ir patvirtinkite išimtis pagal failų plėtinį ir aplanko vietą](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-antivirus/configure-extension-file-exclusions-microsoft-defender-antivirus) bei [Konfigūruokite pagal procesus atidarytų failų išimtis](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-antivirus/configure-process-opened-file-exclusions-microsoft-defender-antivirus) .</span><span class="sxs-lookup"><span data-stu-id="806b7-105">For more info, see, [Configure and validate exclusions based on file extension and folder location](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-antivirus/configure-extension-file-exclusions-microsoft-defender-antivirus) and [Configure exclusions for files opened by processes](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-antivirus/configure-process-opened-file-exclusions-microsoft-defender-antivirus) .</span></span>

<span data-ttu-id="806b7-106">Norėdami sukonfigūruoti  **"Windows Server" 2016 ir "2019**", peržiūrėkite " [Microsoft Defender" antivirusinės programos išskyrimų konfigūravimas "Windows Server"](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-antivirus/configure-server-exclusions-microsoft-defender-antivirus).</span><span class="sxs-lookup"><span data-stu-id="806b7-106">To configure exclusions for  **Windows Server 2016 and 2019**, see [Configure Microsoft Defender Antivirus exclusions on Windows Server](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-antivirus/configure-server-exclusions-microsoft-defender-antivirus).</span></span>

<span data-ttu-id="806b7-107">**Mac**</span><span class="sxs-lookup"><span data-stu-id="806b7-107">**Mac**</span></span>

<span data-ttu-id="806b7-108">Išsamios informacijos apie palaikomus atmetimo tipus ir "Mac" išimčių sąrašo konfigūravimą ieškokite [palaikomų atmetimo tipų](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#supported-exclusion-types) ir [kaip konfigūruoti išimčių sąrašą](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#how-to-configure-the-list-of-exclusions).</span><span class="sxs-lookup"><span data-stu-id="806b7-108">For details on supported exclusion types and configuring a list of exclusions for Mac, see [Supported exclusion types](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#supported-exclusion-types) and [How to configure the list of exclusions](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#how-to-configure-the-list-of-exclusions).</span></span>

<span data-ttu-id="806b7-109">**Pastaba** Taip pat galite patvirtinti išimčių sąrašus naudodami "EICAR" bandomąjį failą.</span><span class="sxs-lookup"><span data-stu-id="806b7-109">**Note** You can also validate exclusions lists using the EICAR test file.</span></span> <span data-ttu-id="806b7-110">Daugiau informacijos ieškokite [išimčių sąrašai su "EICAR" tikrinimo failu](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#validate-exclusions-lists-with-the-eicar-test-file).</span><span class="sxs-lookup"><span data-stu-id="806b7-110">For more info, see [Validate exclusions lists with the EICAR test file](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#validate-exclusions-lists-with-the-eicar-test-file).</span></span> 

<span data-ttu-id="806b7-111">**Linux**</span><span class="sxs-lookup"><span data-stu-id="806b7-111">**Linux**</span></span>

<span data-ttu-id="806b7-112">Išsamios informacijos apie palaikomus atmetimo tipus ir konfigūruojant "Linux" išimčių sąrašą rasite [palaikomų išimčių tipus](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions#supported-exclusion-types) ir [Konfigūruokite bei patvirtinkite išimtis "Microsoft Defender ATP for Linux"](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions).</span><span class="sxs-lookup"><span data-stu-id="806b7-112">For details on supported exclusion types and configuring a list of exclusions for Linux, see [Supported exclusion types](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions#supported-exclusion-types) and [Configure and validate exclusions for Microsoft Defender ATP for Linux](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions).</span></span>

<span data-ttu-id="806b7-113">**Pastaba** Taip pat galite patvirtinti išimčių sąrašus naudodami "EICAR" bandomąjį failą.</span><span class="sxs-lookup"><span data-stu-id="806b7-113">**Note** You can also validate exclusions lists using the EICAR test file.</span></span> <span data-ttu-id="806b7-114">Daugiau informacijos ieškokite [išimčių sąrašai su "EICAR" tikrinimo failu](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions#validate-exclusions-lists-with-the-eicar-test-file).</span><span class="sxs-lookup"><span data-stu-id="806b7-114">For more info, see [Validate exclusions lists with the EICAR test file](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions#validate-exclusions-lists-with-the-eicar-test-file).</span></span> 