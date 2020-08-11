---
title: "\"Teams\" papildinys, skirtas \"Mac\""
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/10/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6173"
- "9003233"
ms.openlocfilehash: 74bd424f71a59b80a91b960b815363668bee7036
ms.sourcegitcommit: 1361b2b37fd0201502a1a3547084961de284a3fc
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 08/11/2020
ms.locfileid: "46629715"
---
# <a name="teams-add-in-for-mac"></a><span data-ttu-id="62206-102">"Teams" papildinys, skirtas "Mac"</span><span class="sxs-lookup"><span data-stu-id="62206-102">Teams add-in for Mac</span></span>

<span data-ttu-id="62206-103">Norėdami pašalinti trūkstamas "Microsoft teams" priedo, skirto "Mac" operacinei sistemai, veiksmus, atlikite šiuos veiksmus:</span><span class="sxs-lookup"><span data-stu-id="62206-103">To troubleshoot a missing Teams add-in for Mac operating system users, follow these steps:</span></span>

<span data-ttu-id="62206-104">**1 veiksmas:** Jei turite hibridinio "Exchange" (2016 CU3 arba naujesnę versiją), naudokite Test-HMA.ps1 įrankį, kad patvirtintumėte, jog hibridinio modernaus autentifikavimo konfigūracija tinkamai sukonfigūruota.</span><span class="sxs-lookup"><span data-stu-id="62206-104">**Step 1:** If you have Hybrid Exchange On-Premises (2016 CU3 or later required), use the Test-HMA.ps1 tool to confirm that Hybrid Modern Authentication is correctly configured.</span></span> <span data-ttu-id="62206-105">Daugiau informacijos ieškokite ["Outlook", skirtos "iOS" ir "Android", hibridinio modernaus autentifikavimo sąrankos](https://aka.ms/AA980zq)patvirtinimas.</span><span class="sxs-lookup"><span data-stu-id="62206-105">For more info, see [Validating Hybrid Modern Authentication setup for Outlook for iOS and Android](https://aka.ms/AA980zq).</span></span>  

<span data-ttu-id="62206-106">**Pastaba** Naudokite UPN adreso formatą (pvz., [username@contoso.com](mailto:username@contoso.com)), o ne domenas\vartotojovardas.</span><span class="sxs-lookup"><span data-stu-id="62206-106">**Note** Use the UPN address format (for example, [username@contoso.com](mailto:username@contoso.com)), not domain\username.</span></span> <span data-ttu-id="62206-107">Atlikite tai net su vartotojais, kurie turi "Exchange Online" pašto dėžutes.</span><span class="sxs-lookup"><span data-stu-id="62206-107">Do this even for users with Exchange Online mailboxes.</span></span>

<span data-ttu-id="62206-108">**2 veiksmas:** Ar vartotojas turi eiti į **įrankių**  >  **paskyras**... programoje "Outlook", skirtos "Mac", ir raskite bei pasirinkite paskyrą.</span><span class="sxs-lookup"><span data-stu-id="62206-108">**Step 2:** Have the user go to **Tools** > **Accounts**... in Outlook for Mac, and find and select the account.</span></span> <span data-ttu-id="62206-109">Patvirtinkite vartotojo vardą, nurodytą UPN formatu (pvz., [username@contoso.com](mailto:username@contoso.com)).</span><span class="sxs-lookup"><span data-stu-id="62206-109">Confirm the username listed is in UPN format (for example, [username@contoso.com](mailto:username@contoso.com)).</span></span>

<span data-ttu-id="62206-110">**3 veiksmas:** Patvirtinkite, kad vartotojas yra licencijuotas "Microsoft teams" vartotojas.</span><span class="sxs-lookup"><span data-stu-id="62206-110">**Step 3:** Confirm the user is a licensed Microsoft Teams user.</span></span> <span data-ttu-id="62206-111">Vartotojas turi naudoti "Office 365 for Mac" prenumeratą, produkto versiją 16,24 arba naujesnę.</span><span class="sxs-lookup"><span data-stu-id="62206-111">The user must be using the Office 365 for Mac subscription, product version 16.24 or later.</span></span>