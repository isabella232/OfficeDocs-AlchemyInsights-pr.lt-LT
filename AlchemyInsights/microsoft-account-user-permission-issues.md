---
title: Trikčių šalinimo problema – vartotojas kataloge nerastas
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.openlocfilehash: 512494a69ab274af00962cb9777a3479b4200fd7
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47725415"
---
# <a name="troubleshoot-issue---user-not-found-in-directory"></a><span data-ttu-id="24f46-102">Trikčių šalinimo problema – vartotojas kataloge nerastas</span><span class="sxs-lookup"><span data-stu-id="24f46-102">Troubleshoot issue - User not found in directory</span></span>

<span data-ttu-id="24f46-103">Jei vartotojai gauna klaidos pranešimą "vartotojas negali būti rastas" kataloge, bandykite dar kartą, kai problemos tipas yra vartotojo kataloge nėra.</span><span class="sxs-lookup"><span data-stu-id="24f46-103">If users are receiving error message "user can't be found" in the directory, please try again where the Issue Type is User not in directory.</span></span>

<span data-ttu-id="24f46-104">Toliau nurodytus veiksmus galima atlikti, kad išspręstumėte problemą.</span><span class="sxs-lookup"><span data-stu-id="24f46-104">The following steps can be completed to troubleshoot the issue.</span></span>

- <span data-ttu-id="24f46-105">Įsitikinkite, kad abonementas, kuris priėmė kvietimą į laišką, yra ta pati paskyra, kuri yra naudojama prisijungiant.</span><span class="sxs-lookup"><span data-stu-id="24f46-105">Ensure the account that accepted the email invitation is the same account that is being used to sign in later.</span></span> <span data-ttu-id="24f46-106">Įsitikinkite, kad vartotojas naudoja tą pačią paskyrą, kad priimtų kvietimą ir prisijungtų prie svetainės.</span><span class="sxs-lookup"><span data-stu-id="24f46-106">Make sure the user is using the same account to accept the invite and sign into the site.</span></span> 

<span data-ttu-id="24f46-107">Daugiau informacijos ieškokite [kaip valdyti "Microsoft" paskyros pseudonimus, </a> kad galėtumėte valdyti "microsoft" 365 prisijungimą](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases).</span><span class="sxs-lookup"><span data-stu-id="24f46-107">For more info, see [How to manage aliases for your Microsoft account</a> to manage the Microsoft 365 login](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases).</span></span> 

- <span data-ttu-id="24f46-108">Eikite į kiekvieną svetainę (-as), kurioje vartotojas gauna klaidą.</span><span class="sxs-lookup"><span data-stu-id="24f46-108">Browse to each site(s) in which the user is receiving the error.</span></span> 

<span data-ttu-id="24f46-109">Įtraukite "/_layouts/15/People.aspx/membershipgroupid = 0" (per dvigubų kabučių) į svetainės URL pabaigą.</span><span class="sxs-lookup"><span data-stu-id="24f46-109">Add "/_layouts/15/people.aspx/membershipgroupid=0" (within the double-quotes) to the end of the site URL.</span></span> 

<span data-ttu-id="24f46-110">Pavyzdys: https://< "Contoso" >. sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0.</span><span class="sxs-lookup"><span data-stu-id="24f46-110">Example: https://<"contoso">.sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0.</span></span>

- <span data-ttu-id="24f46-111">Sąraše pasirinkite vartotoją.</span><span class="sxs-lookup"><span data-stu-id="24f46-111">Select the user from the list.</span></span>

- <span data-ttu-id="24f46-112">Juostelėje spustelėkite **pašalinti vartotojų teises** .</span><span class="sxs-lookup"><span data-stu-id="24f46-112">Click **Remove User Permissions** from the Ribbon.</span></span> 
-  <span data-ttu-id="24f46-113">Įtraukti vartotoją ir iš naujo persiųsti kvietimą vartotojui.</span><span class="sxs-lookup"><span data-stu-id="24f46-113">Add back the User and Resend the invite to the user.</span></span>

