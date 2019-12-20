---
title: "\"Teams\" 4c7 klaida"
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3472"
- "9001211"
ms.openlocfilehash: 0945a341c6456ee4178c0485f3bfb9232fa78a11
ms.sourcegitcommit: 802537a54ef8bde1bdd758ee9a60b6c19d37d6e1
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 12/19/2019
ms.locfileid: "40796248"
---
# <a name="4c7-error-in-microsoft-teams"></a><span data-ttu-id="8a40e-102">4c7 klaida "Microsoft teams"</span><span class="sxs-lookup"><span data-stu-id="8a40e-102">4c7 error in Microsoft Teams</span></span>

<span data-ttu-id="8a40e-103">Ši klaida įvyksta, nes "Microsoft teams" reikalingas formų autentifikavimas.</span><span class="sxs-lookup"><span data-stu-id="8a40e-103">This error occurs because Microsoft Teams requires Forms Authentication.</span></span> <span data-ttu-id="8a40e-104">Kai diegiate Active Directory susiejimo tarnyba (AD FS), formų autentifikavimas neįgalintas intraneto pagal numatytuosius parametrus.</span><span class="sxs-lookup"><span data-stu-id="8a40e-104">When you deploy Active Directory Federation Services (AD FS), Forms Authentication is not enabled for the intranet by default.</span></span> <span data-ttu-id="8a40e-105">Jei "Windows" integruotasis autentifikavimas nepavyksta, būsite paraginti prisijungti naudodami formų autentifikavimas.</span><span class="sxs-lookup"><span data-stu-id="8a40e-105">If Windows Integrated Authentication fails, you are prompted to sign in by using Forms Authentication.</span></span>

<span data-ttu-id="8a40e-106">Norėdami išspręsti šią problemą, įgalinkite formų autentifikavimas naudojant AD FS Microsoft valdymo konsolės (MMC) pridėtiniame įrankyje kompiuteryje, kuriame yra vietos kopiją Active Directory.</span><span class="sxs-lookup"><span data-stu-id="8a40e-106">To resolve this issue, enable Forms Authentication by using the AD FS Microsoft Management Console (MMC) snap-in on the computer that has the local copy of Active Directory.</span></span> <span data-ttu-id="8a40e-107">Jei norite tai padaryti, atlikite tokius veiksmus:</span><span class="sxs-lookup"><span data-stu-id="8a40e-107">To do this, follow these steps:</span></span> 

1. <span data-ttu-id="8a40e-108">Naršymo srityje suraskite **autentifikavimo strategijos**.</span><span class="sxs-lookup"><span data-stu-id="8a40e-108">In the navigation pane, browse to **Authentication Policies**.</span></span>
2. <span data-ttu-id="8a40e-109">Dalyje **veiksmai** išsamios informacijos srityje pasirinkite **Redaguoti visuotinį pirminį autentifikavimą**.</span><span class="sxs-lookup"><span data-stu-id="8a40e-109">Under **Actions** in the details pane, select **Edit Global Primary Authentication**.</span></span>
3. <span data-ttu-id="8a40e-110">Skirtuke **intranetas** pasirinkite **formų autentifikavimas**.</span><span class="sxs-lookup"><span data-stu-id="8a40e-110">On the **Intranet** tab, select **Forms Authentication**.</span></span>
4. <span data-ttu-id="8a40e-111">Pasirinkite **gerai** (arba **taikyti**).</span><span class="sxs-lookup"><span data-stu-id="8a40e-111">Select **OK** (or **Apply**).</span></span>