---
title: "\"OneDrive 0x8004de40 klaidos taisymas"
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: 0edb3e19b5dea240c9f2846dc503e65d92113cb7
ms.sourcegitcommit: 477cce131dc4a3c212ab18a8763a50b2f3bb20b1
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 04/09/2021
ms.locfileid: "51649756"
---
# <a name="fix-0x8004de40-error-in-onedrive"></a><span data-ttu-id="62f08-102">"OneDrive 0x8004de40 klaidos taisymas</span><span class="sxs-lookup"><span data-stu-id="62f08-102">Fix 0x8004de40 error in OneDrive</span></span>

<span data-ttu-id="62f08-103">Jei naudojate "Windows 7" ir gaunate šią klaidą, naujinimas, kad [įgalintumėte TLS 1.1 ir TLS 1.2 kaip numatytuosius saugos protokolus "WinHTTP" sistemoje "Windows".](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392)</span><span class="sxs-lookup"><span data-stu-id="62f08-103">If you're running Windows 7 and receive this error, [Update to enable TLS 1.1 and TLS 1.2 as default secure protocols in WinHTTP in Windows](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392).</span></span>

<span data-ttu-id="62f08-104">Jei naudojate "Windows 10" ir gaunate klaidos 0x8004de40 "OneDrive":</span><span class="sxs-lookup"><span data-stu-id="62f08-104">If you're running Windows 10, and you receive an 0x8004de40 error with OneDrive:</span></span>

- <span data-ttu-id="62f08-105">Perkraukite paveiktą kompiuterį, kai esate prisijungę prie "Acitve Directory" domeno.</span><span class="sxs-lookup"><span data-stu-id="62f08-105">Reboot the affected computer while connected to your Acitve Directory domain.</span></span>
- <span data-ttu-id="62f08-106">Jei paleidimas iš naujo problemos neišspręs, atjunkite ir vėl prijunkite įrenginį iš "Azure AD".</span><span class="sxs-lookup"><span data-stu-id="62f08-106">If a reboot doesn't fix the issue, unjoin and rejoin your device from Azure AD.</span></span> 

<span data-ttu-id="62f08-107">**Pastaba:** atlikdami šiuos veiksmus turėtumėte būti įmonės tinkle.</span><span class="sxs-lookup"><span data-stu-id="62f08-107">**Note**: You should be on your corporate network while performing these steps.</span></span> <span data-ttu-id="62f08-108">Neatlikite šių veiksmų, kai nesate prisijungę prie įmonės infrastruktūros (pvz., keliaudami).</span><span class="sxs-lookup"><span data-stu-id="62f08-108">Don't perform these steps when you aren't connected to your corporate infrastructure (for example, while traveling).</span></span> 

1. <span data-ttu-id="62f08-109">Atidarykite didesnių teisių komandinę eilutę **pasirinkdami Pradžia**, dešiniuoju pelės mygtuku spustelėkite **Komandinė** eilutė , tada pasirinkite **Vykdyti administratoriaus teisėmis**.</span><span class="sxs-lookup"><span data-stu-id="62f08-109">Open an elevated command prompt by selecting **Start**, right-click **Command Prompt**, and then select **Run as administrator**.</span></span>

1. <span data-ttu-id="62f08-110">Įveskite *dsregcmd /leave ir* paspauskite **"Enter".**</span><span class="sxs-lookup"><span data-stu-id="62f08-110">Type *dsregcmd /leave* and press **Enter**.</span></span>

1. <span data-ttu-id="62f08-111">Baigę įveskite *dsregcmd /join ir* paspauskite **"Enter".**</span><span class="sxs-lookup"><span data-stu-id="62f08-111">When complete, type *dsregcmd /join* and press **Enter**.</span></span>

1. <span data-ttu-id="62f08-112">Baigę uždarykite komandinę eilutę.</span><span class="sxs-lookup"><span data-stu-id="62f08-112">When complete, close the command prompt.</span></span>

1. <span data-ttu-id="62f08-113">Iš naujo paleiskite kompiuterį ir prisijunkite prie "OneDrive".</span><span class="sxs-lookup"><span data-stu-id="62f08-113">Reboot the computer, and log into OneDrive.</span></span>