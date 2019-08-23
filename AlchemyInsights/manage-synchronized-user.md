---
title: Valdyti sinchronizuoto vartotojo
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000609"
- "2444"
ms.openlocfilehash: a943c59d67c512e6326856dacd0053db121f6aa3
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 08/22/2019
ms.locfileid: "36542005"
---
# <a name="unable-to-set-primary-email-address-or-change-user-attributes"></a><span data-ttu-id="c9519-102">Neįmanoma nustatyti pagrindinį el. pašto adresą arba pakeisti vartotojo atributus</span><span class="sxs-lookup"><span data-stu-id="c9519-102">Unable to set primary email address or change user attributes</span></span>

<span data-ttu-id="c9519-103">Jei katalogų sinchronizavimo yra įjungta jūsų aplinkoje, kai vartotojas ar objekto atributų negalima keisti naudojant "Microsoft" 365 administravimo centro.</span><span class="sxs-lookup"><span data-stu-id="c9519-103">If directory synchronization is enabled for your environment, some user or object attributes cannot be changed using the Microsoft 365 admin center.</span></span>

<span data-ttu-id="c9519-104">Visiškai valdyti sinchronizuota vartotojams ir jų atributus, naudokite savo vietos Aktyvaus katalogo vartotojus ir grupes valdymo pultą (adsiedit.msc).</span><span class="sxs-lookup"><span data-stu-id="c9519-104">To fully manage synchronized users and all their attributes, use your local active directory users and groups management console (adsiedit.msc).</span></span>  

<span data-ttu-id="c9519-105">Taip pat galite keisti atskirų vartotojų arba atributai sinchronizuota vartotojams naudojant "PowerShell", kaip parodyta šių pavyzdžių:</span><span class="sxs-lookup"><span data-stu-id="c9519-105">Alternatively, you can change individual users or attributes for synchronized users using powershell such as shown in these common examples:</span></span> 
- <span data-ttu-id="c9519-106">Rinkinys-MsolUser - UserPrincipalName user@yourdomain.onmicrosoft.com - AlternateEmailAddresses user2@yourvanitydomain.onmicrosoft.com</span><span class="sxs-lookup"><span data-stu-id="c9519-106">Set-MsolUser -UserPrincipalName user@yourdomain.onmicrosoft.com -AlternateEmailAddresses user2@yourvanitydomain.onmicrosoft.com</span></span>
- <span data-ttu-id="c9519-107">Rinkinys-MsolUser - UserPrincipalName "user@yourdomain.onmicrosoft.com" - DisplayName "Bandomojo vartotojo" - pavardė "Vartotojas"-pavadinimas "Manager"-skyrius "HR"</span><span class="sxs-lookup"><span data-stu-id="c9519-107">Set-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com" -DisplayName "Test User" -LastName "User" -Title "Manager" -Department "HR"</span></span>
- <span data-ttu-id="c9519-108">Pašalinti-MsolUser - UserPrincipalName "user@yourdomain.onmicrosoft.com</span><span class="sxs-lookup"><span data-stu-id="c9519-108">Remove-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com</span></span>