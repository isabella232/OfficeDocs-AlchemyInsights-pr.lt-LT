---
title: Teams,skirtas "Mac"
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/10/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6173"
- "6166"
- "9003233"
- "9002573"
ms.openlocfilehash: 45df4381688335f10f6699d8b5ff1aaafd6f7257
ms.sourcegitcommit: 730efbac8eec016b2b4f83f1b0e01e077f28c444
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 05/20/2021
ms.locfileid: "52582078"
---
# <a name="teams-add-in-for-mac"></a><span data-ttu-id="95d02-102">Teams,skirtas "Mac"</span><span class="sxs-lookup"><span data-stu-id="95d02-102">Teams add-in for Mac</span></span>

<span data-ttu-id="95d02-103">Norėdami pašalinti trūkstamą "Teams", skirtą "Mac", operacinės sistemos vartotojams, atlikite šiuos veiksmus:</span><span class="sxs-lookup"><span data-stu-id="95d02-103">To troubleshoot a missing Teams add-in for Mac operating system users, follow these steps:</span></span>

<span data-ttu-id="95d02-104">**1 veiksmas:** Jei turite hibridinę Exchange vietinį (2016 CU3 arba naujesnę), naudokite "Test-HMA.ps1" įrankį, kad patvirtintumėte, jog hibridinis modernusis autentifikavimas tinkamai sukonfigūruotas.</span><span class="sxs-lookup"><span data-stu-id="95d02-104">**Step 1:** If you have Hybrid Exchange On-Premises (2016 CU3 or later required), use the Test-HMA.ps1 tool to confirm that Hybrid Modern Authentication is correctly configured.</span></span> <span data-ttu-id="95d02-105">Daugiau informacijos žr. [Hibridinio modernaus autentifikavimo sąrankos patvirtinimas "Outlook OS" ir "Android".](https://aka.ms/TestHMAEAS)</span><span class="sxs-lookup"><span data-stu-id="95d02-105">For more info, see [Validating Hybrid Modern Authentication setup for Outlook for iOS and Android](https://aka.ms/TestHMAEAS).</span></span>  

<span data-ttu-id="95d02-106">**Pastaba** Naudokite UPN adreso formatą (pvz., [username@contoso.com](mailto:username@contoso.com)), o ne domeną\vartotojo vardą.</span><span class="sxs-lookup"><span data-stu-id="95d02-106">**Note** Use the UPN address format (for example, [username@contoso.com](mailto:username@contoso.com)), not domain\username.</span></span> <span data-ttu-id="95d02-107">Tai atlikite net vartotojams, naudojantiems Exchange Online pašto dėžutes.</span><span class="sxs-lookup"><span data-stu-id="95d02-107">Do this even for users with Exchange Online mailboxes.</span></span>

<span data-ttu-id="95d02-108">**2 veiksmas:** Nueikite į Įrankių **paskyros**  >  ... "Outlook for Mac" ir raskite ir pasirinkite paskyrą.</span><span class="sxs-lookup"><span data-stu-id="95d02-108">**Step 2:** Have the user go to **Tools** > **Accounts**... in Outlook for Mac, and find and select the account.</span></span> <span data-ttu-id="95d02-109">Patvirtinkite, kad nurodytas vartotojo vardas yra UPN formatu (pvz., [username@contoso.com](mailto:username@contoso.com)).</span><span class="sxs-lookup"><span data-stu-id="95d02-109">Confirm the username listed is in UPN format (for example, [username@contoso.com](mailto:username@contoso.com)).</span></span>

<span data-ttu-id="95d02-110">**3 veiksmas:** Patvirtinkite, kad vartotojas yra licencijuotas Microsoft Teams vartotojas.</span><span class="sxs-lookup"><span data-stu-id="95d02-110">**Step 3:** Confirm the user is a licensed Microsoft Teams user.</span></span> <span data-ttu-id="95d02-111">Vartotojas turi naudoti "Office 365 Mac" prenumeratą, 16.24 arba naujesnę produkto versiją.</span><span class="sxs-lookup"><span data-stu-id="95d02-111">The user must be using the Office 365 for Mac subscription, product version 16.24 or later.</span></span>