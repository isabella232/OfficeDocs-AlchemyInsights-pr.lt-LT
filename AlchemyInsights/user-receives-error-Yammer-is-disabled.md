---
title: Vartotojas gauna klaidos AADSTS7000112 "Yammer" yra išjungtas
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/16/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6010"
- "9003111"
ms.openlocfilehash: c92b09ee9a9ca06f85906e7fce601582a7e83244
ms.sourcegitcommit: c078058ee0b77ee1f1496feb2f3a5773e3e3b30d
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 07/16/2020
ms.locfileid: "45198054"
---
# <a name="user-receives-error-aadsts7000112-yammer-is-disabled"></a><span data-ttu-id="7722f-102">Vartotojas gauna klaidos AADSTS7000112 "Yammer" yra išjungtas</span><span class="sxs-lookup"><span data-stu-id="7722f-102">User receives error AADSTS7000112 Yammer is disabled</span></span>

<span data-ttu-id="7722f-103">Jei gaunate klaidos pranešimą "AADSTS7000112: programa"00000005-0000-0ff1-ce00-00000000000"("Yammer") yra išjungta", problema yra su tarnybos pagrindinė per Azure AD.</span><span class="sxs-lookup"><span data-stu-id="7722f-103">If you receive the error "AADSTS7000112: Application '00000005-0000-0ff1-ce00-000000000000'(Yammer) is disabled", a problem exists with the service principal within Azure AD.</span></span> <span data-ttu-id="7722f-104">Administratorius galėjo išjungti pagrindinę tarnybą, kad užblokuotų prieigą prie "Yammer".</span><span class="sxs-lookup"><span data-stu-id="7722f-104">An administrator might have disabled the service principal to block access to Yammer.</span></span>

<span data-ttu-id="7722f-105">Tarnybos pagrindinės sistemos išjungimas nerekomenduojamas ir gali sukelti papildomų problemų.</span><span class="sxs-lookup"><span data-stu-id="7722f-105">Disabling the service principal is not recommended and can cause additional issues.</span></span> <span data-ttu-id="7722f-106">Daugiau informacijos apie palaikomą vartotojo prieigos prie "Yammer" blokavimo metodą rasite ["Yammer" prieigos išjungimas "Microsoft 365" vartotojams](https://docs.microsoft.com/yammer/manage-yammer-users/turn-off-user-access).</span><span class="sxs-lookup"><span data-stu-id="7722f-106">For more info about the supported approach to block user access to Yammer, see [Turn off Yammer access for Microsoft 365 users](https://docs.microsoft.com/yammer/manage-yammer-users/turn-off-user-access).</span></span>  

<span data-ttu-id="7722f-107">Norėdami išspręsti šią problemą Azure portalas ir atkurti vartotojo prieigą prie "Yammer":</span><span class="sxs-lookup"><span data-stu-id="7722f-107">To correct this issue in the Azure Portal and restore user access to Yammer:</span></span>

1.  <span data-ttu-id="7722f-108">Atidarykite "Azure Active Directory" puslapį ir kairiojoje naršymo srityje dalyje **Tvarkyti** pasirinkite **Įmonės taikomosios programos.**</span><span class="sxs-lookup"><span data-stu-id="7722f-108">Open the Azure Active Directory page, and select **Enterprise applications** under **Manage** in the left navigation pane.</span></span>
3.  <span data-ttu-id="7722f-109">Ieškos lauke įveskite **"Office 365" "Yammer"** ir pasirinkite programos pavadinimą, kad atidarytumėte parametrus.</span><span class="sxs-lookup"><span data-stu-id="7722f-109">Type **Office 365 Yammer** in the search box, and select the application name to open settings.</span></span>
4.  <span data-ttu-id="7722f-110">Kairiojoje naršymo srityje dalyje **Tvarkyti** pasirinkite **Ypatybės.**</span><span class="sxs-lookup"><span data-stu-id="7722f-110">Select **Properties** under **Manage** in the left navigation pane.</span></span>
5.  <span data-ttu-id="7722f-111">Nustatykite **reikšmę Įgalinta vartotojams prisijungti?** **Yes** **Save**</span><span class="sxs-lookup"><span data-stu-id="7722f-111">Set the value of **Enabled for users to sign-in?** to **Yes**, and then select **Save**.</span></span>
6.  <span data-ttu-id="7722f-112">Vėl prisijunkite prie "Yammer".</span><span class="sxs-lookup"><span data-stu-id="7722f-112">Sign in to Yammer again.</span></span> <span data-ttu-id="7722f-113">Gali reikėti išvalyti slapukus.</span><span class="sxs-lookup"><span data-stu-id="7722f-113">You might need to clear cookies.</span></span>

<span data-ttu-id="7722f-114">Arba paleiskite "PowerShell" komandas, kad nustatytumėte reikšmę.</span><span class="sxs-lookup"><span data-stu-id="7722f-114">Alternatively, run PowerShell commands to set the value.</span></span> <span data-ttu-id="7722f-115">Jei reikia daugiau informacijos, [peržiūrėkite klaidos pranešimą "Atsiprašome, bet kyla problemų prisijungiant prie jūsų", kai "Office 365" spustelite "Yammer" plytelę](https://docs.microsoft.com/yammer/troubleshoot-problems/error-when-click-the-yammer-tile-in-office-365).</span><span class="sxs-lookup"><span data-stu-id="7722f-115">For more info, see ["Sorry, but we're having trouble signing you in" error when you click the Yammer tile in Office 365](https://docs.microsoft.com/yammer/troubleshoot-problems/error-when-click-the-yammer-tile-in-office-365).</span></span> 