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
ms.openlocfilehash: 81b9dafe8e27e5f73fe232c51ff56fed3fec29b4
ms.sourcegitcommit: a65d196d00adb70045af5caca9828fe44b951f61
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 09/04/2019
ms.locfileid: "36754200"
---
# <a name="troubleshoot-issue---user-not-found-in-directory"></a><span data-ttu-id="0b15d-102">Šalinti triktis-vartotojas nerastas kataloge</span><span class="sxs-lookup"><span data-stu-id="0b15d-102">Troubleshoot issue - User not found in directory</span></span>

<span data-ttu-id="0b15d-103">Jei vartotojai gauna klaidos pranešimą "vartotojas nerastas" kataloge.</span><span class="sxs-lookup"><span data-stu-id="0b15d-103">If users are receiving error message "user can't be found" in the directory.</span></span> <span data-ttu-id="0b15d-104">Bandykite dar kartą, kai problemos tipas yra vartotojo ne kataloge.</span><span class="sxs-lookup"><span data-stu-id="0b15d-104">Please try again where the Issue Type is User not in directory.</span></span>

<span data-ttu-id="0b15d-105">Norėdami išspręsti šią problemą, galite atlikti toliau nurodytus veiksmus.</span><span class="sxs-lookup"><span data-stu-id="0b15d-105">The following steps can be completed to troubleshoot the issue.</span></span>

- <span data-ttu-id="0b15d-106">Įsitikinkite, kad paskyra, priimta el. paštu, yra ta pati paskyra, kuri naudojama norint prisijungti vėliau.</span><span class="sxs-lookup"><span data-stu-id="0b15d-106">Ensure the account that accepted the email invitation is the same account that is being used to sign in later.</span></span> <span data-ttu-id="0b15d-107">Įsitikinkite, kad naudotojas naudoja tą pačią paskyrą, kad priimtų kvietimą ir prisijungtų prie svetainės.</span><span class="sxs-lookup"><span data-stu-id="0b15d-107">Make sure the user is using the same account to accept the invite and sign into the site.</span></span> 

<span data-ttu-id="0b15d-108">Daugiau informacijos rasite [kaip valdyti "Microsoft" paskyros</a> pseudonimus, kad galėtumėte tvarkyti "Office 365" prisijungimo duomenis](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases).</span><span class="sxs-lookup"><span data-stu-id="0b15d-108">For more info, see [How to manage aliases for your Microsoft account</a> to manage the Office 365 login](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases).</span></span> 

- <span data-ttu-id="0b15d-109">Pereikite į kiekvieną svetainę (-as), kurioje vartotojas gauna klaidą.</span><span class="sxs-lookup"><span data-stu-id="0b15d-109">Browse to each site(s) in which the user is receiving the error.</span></span> 

<span data-ttu-id="0b15d-110">Pridėti "/_layouts/15/People.aspx/membershipgroupid = 0" (per dvigubų kabučių) į svetainės URL pabaigoje.</span><span class="sxs-lookup"><span data-stu-id="0b15d-110">Add "/_layouts/15/people.aspx/membershipgroupid=0" (within the double-quotes) to the end of the site URL.</span></span> 

<span data-ttu-id="0b15d-111">Pavyzdys: https://< "contoso">. SharePoint. com/_ Layouts/15/People. aspx/membershipGroupId = 0.</span><span class="sxs-lookup"><span data-stu-id="0b15d-111">Example: https://<"contoso">.sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0.</span></span>

- <span data-ttu-id="0b15d-112">Pasirinkite vartotoją iš sąrašo.</span><span class="sxs-lookup"><span data-stu-id="0b15d-112">Select the user from the list.</span></span>

- <span data-ttu-id="0b15d-113">Juostelėje spustelėkite **pašalinti vartotojo teises** .</span><span class="sxs-lookup"><span data-stu-id="0b15d-113">Click **Remove User Permissions** from the Ribbon.</span></span> 
-  <span data-ttu-id="0b15d-114">Pridėti atgal vartotojo ir persiųsti pakviesti į vartotoją.</span><span class="sxs-lookup"><span data-stu-id="0b15d-114">Add back the User and Resend the invite to the user.</span></span>

