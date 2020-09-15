---
title: "\"Teams\" 4c7 klaida"
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3472"
- "9001211"
ms.openlocfilehash: 08494b461a24eba8999a5edb99c89af7b17db9b3
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47700211"
---
# <a name="4c7-error-in-microsoft-teams"></a><span data-ttu-id="32431-102">4c7 klaida programoje "Microsoft teams"</span><span class="sxs-lookup"><span data-stu-id="32431-102">4c7 error in Microsoft Teams</span></span>

<span data-ttu-id="32431-103">Ši klaida įvyksta dėl to, kad "Microsoft teams" reikia formų autentifikavimo.</span><span class="sxs-lookup"><span data-stu-id="32431-103">This error occurs because Microsoft Teams requires Forms Authentication.</span></span> <span data-ttu-id="32431-104">Kai diegiate "Active Directory" susiejimo tarnybą (AD FS), intraneto formų autentifikavimas neįgalintas pagal numatytuosius.</span><span class="sxs-lookup"><span data-stu-id="32431-104">When you deploy Active Directory Federation Services (AD FS), Forms Authentication is not enabled for the intranet by default.</span></span> <span data-ttu-id="32431-105">Jei nepavyksta "Windows" integruoto autentifikavimo, būsite paraginti prisijungti naudodami formų autentifikavimą.</span><span class="sxs-lookup"><span data-stu-id="32431-105">If Windows Integrated Authentication fails, you are prompted to sign in by using Forms Authentication.</span></span>

<span data-ttu-id="32431-106">Norėdami išspręsti šią problemą, įgalinkite formų autentifikavimą naudodami AD FS "Microsoft" valdymo konsolės (MMC) pridėtinį įrankį kompiuteryje, kuriame yra vietinė "Active Directory" kopija.</span><span class="sxs-lookup"><span data-stu-id="32431-106">To resolve this issue, enable Forms Authentication by using the AD FS Microsoft Management Console (MMC) snap-in on the computer that has the local copy of Active Directory.</span></span> <span data-ttu-id="32431-107">Jei norite tai padaryti, atlikite tokius veiksmus:</span><span class="sxs-lookup"><span data-stu-id="32431-107">To do this, follow these steps:</span></span> 

1. <span data-ttu-id="32431-108">Naršymo srityje raskite **autentifikavimo strategijas**.</span><span class="sxs-lookup"><span data-stu-id="32431-108">In the navigation pane, browse to **Authentication Policies**.</span></span>
2. <span data-ttu-id="32431-109">Dalyje **veiksmai** išsamios informacijos srityje pasirinkite **Redaguoti visuotinį pirminį autentifikavimą**.</span><span class="sxs-lookup"><span data-stu-id="32431-109">Under **Actions** in the details pane, select **Edit Global Primary Authentication**.</span></span>
3. <span data-ttu-id="32431-110">Skirtuke **intranetas** pasirinkite **formų autentifikavimas**.</span><span class="sxs-lookup"><span data-stu-id="32431-110">On the **Intranet** tab, select **Forms Authentication**.</span></span>
4. <span data-ttu-id="32431-111">Pasirinkite **gerai** (arba **taikyti**).</span><span class="sxs-lookup"><span data-stu-id="32431-111">Select **OK** (or **Apply**).</span></span>