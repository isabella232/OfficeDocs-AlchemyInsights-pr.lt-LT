---
title: Šalinti triktis-vartotojas nerastas kataloge
ms.author: pebaum
author: Techwriter40
manager: pamgreen
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.openlocfilehash: 59713231da25be441e7c05d788337e66bf17265a
ms.sourcegitcommit: b43f77221f47b50c41197a448a9c26c423ce1ad5
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 11/15/2019
ms.locfileid: "37768809"
---
# <a name="troubleshoot-issue---user-not-found-in-directory"></a><span data-ttu-id="f5820-102">Šalinti triktis-vartotojas nerastas kataloge</span><span class="sxs-lookup"><span data-stu-id="f5820-102">Troubleshoot issue - User not found in directory</span></span>

<span data-ttu-id="f5820-103">Jei vartotojai gauna klaidos pranešimą "vartotojas negali rasti" kataloge, bandykite dar kartą, kai problema tipas yra vartotojas ne kataloge.</span><span class="sxs-lookup"><span data-stu-id="f5820-103">If users are receiving error message "user can't be found" in the directory, please try again where the Issue Type is User not in directory.</span></span>

<span data-ttu-id="f5820-104">Norėdami išspręsti šią problemą, galite atlikti toliau nurodytus veiksmus.</span><span class="sxs-lookup"><span data-stu-id="f5820-104">The following steps can be completed to troubleshoot the issue.</span></span>

- <span data-ttu-id="f5820-105">Įsitikinkite, kad paskyra, priimta el. paštu, yra ta pati paskyra, kuri naudojama norint prisijungti vėliau.</span><span class="sxs-lookup"><span data-stu-id="f5820-105">Ensure the account that accepted the email invitation is the same account that is being used to sign in later.</span></span> <span data-ttu-id="f5820-106">Įsitikinkite, kad naudotojas naudoja tą pačią paskyrą, kad priimtų kvietimą ir prisijungtų prie svetainės.</span><span class="sxs-lookup"><span data-stu-id="f5820-106">Make sure the user is using the same account to accept the invite and sign into the site.</span></span> 

<span data-ttu-id="f5820-107">Daugiau informacijos rasite [kaip valdyti "Microsoft" paskyros</a> pseudonimus, kad galėtumėte tvarkyti "Office 365" prisijungimo duomenis](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases).</span><span class="sxs-lookup"><span data-stu-id="f5820-107">For more info, see [How to manage aliases for your Microsoft account</a> to manage the Office 365 login](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases).</span></span> 

- <span data-ttu-id="f5820-108">Pereikite į kiekvieną svetainę (-as), kurioje vartotojas gauna klaidą.</span><span class="sxs-lookup"><span data-stu-id="f5820-108">Browse to each site(s) in which the user is receiving the error.</span></span> 

<span data-ttu-id="f5820-109">Pridėti "/_layouts/15/People.aspx/membershipgroupid = 0" (per dvigubų kabučių) į svetainės URL pabaigoje.</span><span class="sxs-lookup"><span data-stu-id="f5820-109">Add "/_layouts/15/people.aspx/membershipgroupid=0" (within the double-quotes) to the end of the site URL.</span></span> 

<span data-ttu-id="f5820-110">Pavyzdys: https://< "Contoso" >. sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0.</span><span class="sxs-lookup"><span data-stu-id="f5820-110">Example: https://<"contoso">.sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0.</span></span>

- <span data-ttu-id="f5820-111">Pasirinkite vartotoją iš sąrašo.</span><span class="sxs-lookup"><span data-stu-id="f5820-111">Select the user from the list.</span></span>

- <span data-ttu-id="f5820-112">Juostelėje spustelėkite **pašalinti vartotojo teises** .</span><span class="sxs-lookup"><span data-stu-id="f5820-112">Click **Remove User Permissions** from the Ribbon.</span></span> 
-  <span data-ttu-id="f5820-113">Pridėti atgal vartotojo ir persiųsti pakviesti į vartotoją.</span><span class="sxs-lookup"><span data-stu-id="f5820-113">Add back the User and Resend the invite to the user.</span></span>

