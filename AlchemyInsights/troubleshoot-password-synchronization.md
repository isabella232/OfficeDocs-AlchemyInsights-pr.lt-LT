---
title: Slaptažodžių sinchronizavimo trikčių diagnostika
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "579"
- "1300006"
ms.assetid: 1cba32c4-37ce-4ec1-9e58-8d3440b53d57
ms.openlocfilehash: 54b5a033b7cbb99520425b31800364ed4a99a4e6
ms.sourcegitcommit: 1d01b8b48eef2d5d10c375dcf802cd36e9d6bf61
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 07/23/2020
ms.locfileid: "45387885"
---
# <a name="troubleshoot-password-synchronization"></a><span data-ttu-id="e49e5-102">Slaptažodžių sinchronizavimo trikčių diagnostika</span><span class="sxs-lookup"><span data-stu-id="e49e5-102">Troubleshoot password synchronization</span></span>

<span data-ttu-id="e49e5-103">Norėdami pašalinti slaptažodžių sinchronizavimo problemas, pradėkite naudoti šią AAD prisijungimo trikčių šalinimo užduotį, kad nustatytumėte, kodėl slaptažodžiai nesinchronizuojami.</span><span class="sxs-lookup"><span data-stu-id="e49e5-103">To troubleshoot password synchronization issues, start by using this AAD Connect troubleshooting task to determine why passwords are not syncing.</span></span> <span data-ttu-id="e49e5-104">Norėdami pradėti, eikite į [Tvarkyti tiesioginį sinchronizavimą](https://admin.microsoft.com/AdminPortal/Home#/dirsyncmanagement).</span><span class="sxs-lookup"><span data-stu-id="e49e5-104">To begin, go to [Manage direct sync](https://admin.microsoft.com/AdminPortal/Home#/dirsyncmanagement).</span></span>  

1. <span data-ttu-id="e49e5-105">Atidarykite naują "Windows PowerShell" seansą savo "Azure AD Connect" serveryje ir pasirinkite parinktį **Paleisti administratoriaus teisėmis.**</span><span class="sxs-lookup"><span data-stu-id="e49e5-105">Open a new Windows PowerShell session on your Azure AD Connect server, and select the **Run as Administrator** option.</span></span>

2. <span data-ttu-id="e49e5-106">Paleiskite Set-ExecutionPolicy RemoteSigned arba Set-ExecutionPolicy Unrestricted.</span><span class="sxs-lookup"><span data-stu-id="e49e5-106">Run Set-ExecutionPolicy RemoteSigned or Set-ExecutionPolicy Unrestricted.</span></span>

3. <span data-ttu-id="e49e5-107">Paleiskite Azure AD Connect vedlį.</span><span class="sxs-lookup"><span data-stu-id="e49e5-107">Start the Azure AD Connect wizard.</span></span>

4. <span data-ttu-id="e49e5-108">Eikite į puslapį Papildomos užduotys > **Šalinti**  >  **triktis toliau**.</span><span class="sxs-lookup"><span data-stu-id="e49e5-108">Go to the Additional Tasks page > **Troubleshoot** > **Next**.</span></span>

5. <span data-ttu-id="e49e5-109">Pasirinkite **Paleisti,** kad atidarytumėte "PowerShell" trikčių diagnostikos meniu.</span><span class="sxs-lookup"><span data-stu-id="e49e5-109">Select **Launch** to open the PowerShell troubleshooting menu.</span></span>

6. <span data-ttu-id="e49e5-110">Pasirinkite **Slaptažodžių sinchronizavimo trikčių diagnostika**.</span><span class="sxs-lookup"><span data-stu-id="e49e5-110">Select **Troubleshoot Password Synchronization**.</span></span>

    <span data-ttu-id="e49e5-111">Problema yra paprastai, kad slaptažodis nėra sinchronizuojami tam tikrą vartotojo abonementą.</span><span class="sxs-lookup"><span data-stu-id="e49e5-111">The issue is usually that a password is not synchronized for a specific user account.</span></span>

    <span data-ttu-id="e49e5-112">**Pastabos** Slaptažodžio sinchronizavimas nepavyksta, jei paskutinis sėkmingas slaptažodžio sinchronizavimas buvo prieš kurį laiką.</span><span class="sxs-lookup"><span data-stu-id="e49e5-112">**Notes** Password synchronization fails if the last successful password sync was some time ago.</span></span>

<span data-ttu-id="e49e5-113">Daugiau pagalbos dėl slaptažodžių sinchronizavimo trikčių diagnostika, [peržiūrėkite slaptažodžio maišos sinchronizavimo su "Azure AD Connect" sinchronizavimo trikčių diagnostika](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization).</span><span class="sxs-lookup"><span data-stu-id="e49e5-113">For more help troubleshooting password synchronization, see [Troubleshoot password hash synchronization with Azure AD Connect sync](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization).</span></span>