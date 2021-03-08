---
title: Nustatykite ClientAccessServerEnabled į TRUE
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/24/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000078"
- "7342"
ms.openlocfilehash: 2adf35662797e9e9e354ddd0c513f5ce2463d07c
ms.sourcegitcommit: c202c0df2d141e63f4f7eb13a56efbfc2f57348f
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 03/05/2021
ms.locfileid: "50525968"
---
# <a name="set-clientaccessserverenabled-to-true"></a><span data-ttu-id="c119d-102">Nustatykite ClientAccessServerEnabled į TRUE</span><span class="sxs-lookup"><span data-stu-id="c119d-102">Set ClientAccessServerEnabled to True</span></span>

<span data-ttu-id="c119d-103">Jei negalite atidaryti užšifruotos el. laiško, o ne matyti **rpmsg** priedą, atlikite šiuos veiksmus:</span><span class="sxs-lookup"><span data-stu-id="c119d-103">If you can't open an encrypted email message and instead see an **rpmsg** attachment, perform the following steps:</span></span>

1. <span data-ttu-id="c119d-104">Prisijungimas prie "Exchange Online" "PowerShell".</span><span class="sxs-lookup"><span data-stu-id="c119d-104">Connect to Exchange Online PowerShell.</span></span>

> [!NOTE]
> <span data-ttu-id="c119d-105">Norėdami prisijungti prie "Exchange Online PowerShell", turite prisijungti naudodami visuotinio administratoriaus arba "Exchange" administratoriaus paskyrą.</span><span class="sxs-lookup"><span data-stu-id="c119d-105">To connect to Exchange Online PowerShell, you must sign in using a global admin or Exchange admin account.</span></span>

   <span data-ttu-id="c119d-106">a.</span><span class="sxs-lookup"><span data-stu-id="c119d-106">a.</span></span> <span data-ttu-id="c119d-107">Atidarykite "Windows PowerShell", tada vykdykite šią komandą: `$UserCredential = Get-Credential`</span><span class="sxs-lookup"><span data-stu-id="c119d-107">Open Windows PowerShell, and then run the following command: `$UserCredential = Get-Credential`</span></span>
<span data-ttu-id="c119d-108">b.</span><span class="sxs-lookup"><span data-stu-id="c119d-108">b.</span></span> <span data-ttu-id="c119d-109">Dialogo lange **"Windows PowerShell" kredencialų užklausa** įveskite savo darbo arba mokymo įstaigos paskyrą ir slaptažodį, c.</span><span class="sxs-lookup"><span data-stu-id="c119d-109">In the **Windows PowerShell Credential Request** dialog box, enter your work or school account and password, c.</span></span> <span data-ttu-id="c119d-110">Spustelėkite **Gerai**.</span><span class="sxs-lookup"><span data-stu-id="c119d-110">Click **OK**.</span></span> 

2. <span data-ttu-id="c119d-111">Vykdykite šią komandą, kad sukurtumėte naują seansą:</span><span class="sxs-lookup"><span data-stu-id="c119d-111">Run the following command to create a new session:</span></span>

    `$Session = New-PSSession -ConfigurationName Microsoft.Exchange -ConnectionUri https://outlook.office365.com/powershell-liveid/ -Credential $UserCredential -Authentication Basic -AllowRedirection`

    <span data-ttu-id="c119d-112">a.</span><span class="sxs-lookup"><span data-stu-id="c119d-112">a.</span></span> <span data-ttu-id="c119d-113">Vykdykite toliau nurodytą komandą.</span><span class="sxs-lookup"><span data-stu-id="c119d-113">Run the following command:</span></span>
    
    `Import-PSSession $Session -DisableNameChecking`

3. <span data-ttu-id="c119d-114">`Get-IRMConfiguration`Komanda vykdyti.</span><span class="sxs-lookup"><span data-stu-id="c119d-114">Run `Get-IRMConfiguration` command.</span></span>

4. <span data-ttu-id="c119d-115">Pažymėkite parametrą **Clientaccessserverenabled** .</span><span class="sxs-lookup"><span data-stu-id="c119d-115">Check the **ClientAccessServerEnabled** setting.</span></span> 

    <span data-ttu-id="c119d-116">a.</span><span class="sxs-lookup"><span data-stu-id="c119d-116">a.</span></span> <span data-ttu-id="c119d-117">Jei parametras **Clientaccessserverenabled** nustatytas kaip **klaidingas**, vykdykite šią "cmdlet": `Set-IRMConfiguration -ClientAccessServerEnabled $True`</span><span class="sxs-lookup"><span data-stu-id="c119d-117">If **ClientAccessServerEnabled** setting is set to **False**, run the following cmdlet: `Set-IRMConfiguration -ClientAccessServerEnabled $True`</span></span>

> [!TIP]
> <span data-ttu-id="c119d-118">Visada uždarykite "PowerShell" seansą naudodami šią komandą: `Remove-PSSession $Session`</span><span class="sxs-lookup"><span data-stu-id="c119d-118">Always close your powershell session with the following command: `Remove-PSSession $Session`</span></span>

<span data-ttu-id="c119d-119">Daugiau informacijos ieškokite " [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell)".</span><span class="sxs-lookup"><span data-stu-id="c119d-119">For more information, see [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell).</span></span>

