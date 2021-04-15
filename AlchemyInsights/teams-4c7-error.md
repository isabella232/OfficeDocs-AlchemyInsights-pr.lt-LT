---
title: "\"Teams 4c7\" klaida"
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3472"
- "9001211"
ms.openlocfilehash: 51f2aa936e803b63bcbdf73b89959cd3a1757751
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 04/15/2021
ms.locfileid: "51786677"
---
# <a name="4c7-error-in-microsoft-teams"></a><span data-ttu-id="3691f-102">4c7 klaida "Microsoft Teams"</span><span class="sxs-lookup"><span data-stu-id="3691f-102">4c7 error in Microsoft Teams</span></span>

<span data-ttu-id="3691f-103">Ši klaida įvyksta todėl, kad "Microsoft Teams" reikalauja formų autentifikavimo.</span><span class="sxs-lookup"><span data-stu-id="3691f-103">This error occurs because Microsoft Teams requires Forms Authentication.</span></span> <span data-ttu-id="3691f-104">Kai diegiate "Active Directory" susiejimo tarnybas (AD FS), formų autentifikavimas intranete pagal numatytuosius parametrus neįgalintas.</span><span class="sxs-lookup"><span data-stu-id="3691f-104">When you deploy Active Directory Federation Services (AD FS), Forms Authentication is not enabled for the intranet by default.</span></span> <span data-ttu-id="3691f-105">Jei "Windows" integruotasis autentifikavimas nepavyksta, būsite paraginti prisijungti naudodami formų autentifikavimą.</span><span class="sxs-lookup"><span data-stu-id="3691f-105">If Windows Integrated Authentication fails, you are prompted to sign in by using Forms Authentication.</span></span>

<span data-ttu-id="3691f-106">Norėdami išspręsti šią problemą, įgalinkite formų autentifikavimą naudodami AD FS "Microsoft" valdymo konsolės (MMC) pridėtinį įrankį kompiuteryje, kuriame yra vietinė "Active Directory" kopija.</span><span class="sxs-lookup"><span data-stu-id="3691f-106">To resolve this issue, enable Forms Authentication by using the AD FS Microsoft Management Console (MMC) snap-in on the computer that has the local copy of Active Directory.</span></span> <span data-ttu-id="3691f-107">Jei norite tai padaryti, atlikite tokius veiksmus:</span><span class="sxs-lookup"><span data-stu-id="3691f-107">To do this, follow these steps:</span></span> 

1. <span data-ttu-id="3691f-108">Naršymo srityje raskite **Autentifikavimo strategijos**.</span><span class="sxs-lookup"><span data-stu-id="3691f-108">In the navigation pane, browse to **Authentication Policies**.</span></span>
2. <span data-ttu-id="3691f-109">Išsamios **informacijos** srityje dalyje Veiksmai pasirinkite Redaguoti **visuotinį pirminį autentifikavimą**.</span><span class="sxs-lookup"><span data-stu-id="3691f-109">Under **Actions** in the details pane, select **Edit Global Primary Authentication**.</span></span>
3. <span data-ttu-id="3691f-110">Skirtuke **Intranetas** pasirinkite Formų **autentifikavimas**.</span><span class="sxs-lookup"><span data-stu-id="3691f-110">On the **Intranet** tab, select **Forms Authentication**.</span></span>
4. <span data-ttu-id="3691f-111">Pasirinkite **Gerai** (arba **Taikyti**).</span><span class="sxs-lookup"><span data-stu-id="3691f-111">Select **OK** (or **Apply**).</span></span>