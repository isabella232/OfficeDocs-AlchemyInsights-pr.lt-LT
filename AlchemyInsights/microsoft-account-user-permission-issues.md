---
title: Šalinti triktis problema - vartotojas nerastas katalogas
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.openlocfilehash: 537b27d06acd17cbb3fe99bcb89e153099e92bb4
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 08/22/2019
ms.locfileid: "36544871"
---
# <a name="troubleshoot-issue---user-not-found-in-directory"></a><span data-ttu-id="ac286-102">Šalinti triktis problema - vartotojas nerastas katalogas</span><span class="sxs-lookup"><span data-stu-id="ac286-102">Troubleshoot issue - User not found in directory</span></span>

<span data-ttu-id="ac286-103">Jei vartotojai gaunate klaidos pranešimą "negali rasti vartotojo" kataloge.</span><span class="sxs-lookup"><span data-stu-id="ac286-103">If users are receiving error message "user can't be found" in the directory.</span></span> <span data-ttu-id="ac286-104">Prašome pabandyti dar kartą kai problemos tipas nėra vartotojo kataloge.</span><span class="sxs-lookup"><span data-stu-id="ac286-104">Please try again where the Issue Type is User not in directory.</span></span>

<span data-ttu-id="ac286-105">Šiuos veiksmus galima užbaigti Šalinkite triktis.</span><span class="sxs-lookup"><span data-stu-id="ac286-105">The following steps can be completed to troubleshoot the issue.</span></span>

- <span data-ttu-id="ac286-106">Užtikrinti, sąskaitą, kuri priima el. pašto kvietimą tą patį abonementą, kuris yra naudojamas prisijungti vėliau.</span><span class="sxs-lookup"><span data-stu-id="ac286-106">Ensure the account that accepted the email invitation is the same account that is being used to sign in later.</span></span> <span data-ttu-id="ac286-107">Įsitikinkite, kad vartotojas naudoja tą pačią sąskaitą priimti kvietimą ir prisijunkite prie svetainės.</span><span class="sxs-lookup"><span data-stu-id="ac286-107">Make sure the user is using the same account to accept the invite and sign into the site.</span></span> 

<span data-ttu-id="ac286-108">Daugiau informacijos rasite [kaip tvarkyti "Microsoft" paskyros pseudonimų</a> valdyti "Office 365" prisijungimo](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases).</span><span class="sxs-lookup"><span data-stu-id="ac286-108">For more info, see [How to manage aliases for your Microsoft account</a> to manage the Office 365 login](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases).</span></span> 

- <span data-ttu-id="ac286-109">Pereikite prie kiekvienos omis, kurioje vartotojas gauna klaidos.</span><span class="sxs-lookup"><span data-stu-id="ac286-109">Browse to each site(s) in which the user is receiving the error.</span></span> 

<span data-ttu-id="ac286-110">Įtraukite "/ _layouts/15/people.aspx/membershipgroupid=0" (per dvigubų kabučių) į svetainės URL pabaigą.</span><span class="sxs-lookup"><span data-stu-id="ac286-110">Add "/_layouts/15/people.aspx/membershipgroupid=0" (within the double-quotes) to the end of the site URL.</span></span> 

<span data-ttu-id="ac286-111">Pavyzdys: https://_lT _"contoso">.sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0.</span><span class="sxs-lookup"><span data-stu-id="ac286-111">Example: https://<"contoso">.sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0.</span></span>

- <span data-ttu-id="ac286-112">Pasirinkite vartotoją iš sąrašo.</span><span class="sxs-lookup"><span data-stu-id="ac286-112">Select the user from the list.</span></span>

- <span data-ttu-id="ac286-113">Spustelėkite **Šalinti vartotojo teises** iš juostelės.</span><span class="sxs-lookup"><span data-stu-id="ac286-113">Click **Remove User Permissions** from the Ribbon.</span></span> 
-  <span data-ttu-id="ac286-114">Pridėti atgal vartotoją ir persiųsti kvietimą vartotojui.</span><span class="sxs-lookup"><span data-stu-id="ac286-114">Add back the User and Resend the invite to the user.</span></span>

