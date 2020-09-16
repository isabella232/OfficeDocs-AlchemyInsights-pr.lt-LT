---
title: "\"Yammer\" licencijavimo problemos"
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/14/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5900"
- "9003071"
ms.openlocfilehash: f0a7625c7b77860e5ba0e29f2df47101749aace3
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47657284"
---
# <a name="yammer-licensing-issues"></a><span data-ttu-id="4e297-102">"Yammer" licencijavimo problemos</span><span class="sxs-lookup"><span data-stu-id="4e297-102">Yammer licensing issues</span></span>

<span data-ttu-id="4e297-103">Visi vartotojai turi turėti licenciją, kad galėtų naudoti "Yammer Enterprise" paslaugą, tačiau pagal numatytuosius "Yammer" nereikalauja, kad vartotojai turėtų licenciją, kad galėtų pasiekti paslaugą.</span><span class="sxs-lookup"><span data-stu-id="4e297-103">All users must have a license to use the Yammer Enterprise service, but by default Yammer does not require that users have a license to access the service.</span></span> <span data-ttu-id="4e297-104">Kai administratorius pakeis nustatymą, kad būtų galima blokuoti "Microsoft 365" vartotojus, neturinčius "Yammer" licencijų, vartotojai, kuriems nepriskirta "Yammer Enterprise" licencija, negali pasiekti "Yammer"</span><span class="sxs-lookup"><span data-stu-id="4e297-104">When an administrator changes the setting to block Microsoft 365 users without Yammer licenses, users not assigned a Yammer Enterprise license can't access the Yammer service.</span></span> <span data-ttu-id="4e297-105">Daugiau informacijos ieškokite " [Yammer" vartotojų licencijų valdymas "Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365) "</span><span class="sxs-lookup"><span data-stu-id="4e297-105">For more info, see [Manage Yammer user licenses in Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365)</span></span> 

<span data-ttu-id="4e297-106">Kai licencijos pašalinamos iš vartotojų, "Yammer" plytelė nebebus rodoma, o kitos tarnybos gali naudoti licencijos pašalinimą, kad būtų slepiamos funkcijos.</span><span class="sxs-lookup"><span data-stu-id="4e297-106">When licenses are removed from users, the Yammer tile is no longer displayed, and other services can use license removal to hide features.</span></span> <span data-ttu-id="4e297-107">Kitais atvejais funkcijos vis tiek gali atsirasti, bet reikia vykdyti licencijos priskyrimą.</span><span class="sxs-lookup"><span data-stu-id="4e297-107">In other cases, features can still appear but require licence assignment to operate.</span></span>  

<span data-ttu-id="4e297-108">**Licencija neatnaujinama vartotojui**</span><span class="sxs-lookup"><span data-stu-id="4e297-108">**License is not getting updated for the user**</span></span>  

<span data-ttu-id="4e297-109">Kartais vartotojui priskiriama licencija, tačiau jis vis tiek negali pasiekti "Yammer".</span><span class="sxs-lookup"><span data-stu-id="4e297-109">Occasionally, a user is assigned a license but is still unable to access Yammer.</span></span> <span data-ttu-id="4e297-110">Delsimas yra labiau tikėtinas, kai vykdoma masinės licencijos priskyrimas.</span><span class="sxs-lookup"><span data-stu-id="4e297-110">Delays are more likely to occur when a mass license assignment is in progress.</span></span> <span data-ttu-id="4e297-111">"Yammer" vartotojai gali būti neatnaujinti ta pačia tvarka, kaip licencijos pakeistos "Azure AD", nes sistema veikia asinchroniškai.</span><span class="sxs-lookup"><span data-stu-id="4e297-111">Yammer users might not be updated in the same order as licenses are changed in Azure AD because the system runs asynchronously.</span></span> <span data-ttu-id="4e297-112">Palaukite iki 24 valandų, kol bus atidaroma palaikymo byla, kad būtų galima pranešti apie licencijos sinchronizavimo problemas.</span><span class="sxs-lookup"><span data-stu-id="4e297-112">Wait up to 24 hours before opening a support case to report license sync issues.</span></span>  

<span data-ttu-id="4e297-113">**Masinis licencijų priskyrimas**</span><span class="sxs-lookup"><span data-stu-id="4e297-113">**Bulk licence assignment**</span></span>  

<span data-ttu-id="4e297-114">Licencijas galima priskirti administravimo centre arba "PowerShell" scenarijams.</span><span class="sxs-lookup"><span data-stu-id="4e297-114">Licenses can be assigned through the admin center or PowerShell scripting.</span></span> <span data-ttu-id="4e297-115">Daugiau informacijos ieškokite [licencijų priskyrimas vartotojams](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) ir [licencijų priskyrimas vartotojų abonementams su "Office 365 PowerShell](https://docs.microsoft.com/office365/enterprise/powershell/assign-licenses-to-user-accounts-with-office-365-powershell)".</span><span class="sxs-lookup"><span data-stu-id="4e297-115">For more info, see [Assign licenses to users](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) and [Assign licenses to user accounts with Office 365 PowerShell](https://docs.microsoft.com/office365/enterprise/powershell/assign-licenses-to-user-accounts-with-office-365-powershell).</span></span> 

<span data-ttu-id="4e297-116">"Microsoft" palaikymas neteikia pagalbos kuriant scenarijus, bet galima naudoti dokumentaciją apie "Yammer" licencijos priskyrimas.</span><span class="sxs-lookup"><span data-stu-id="4e297-116">Microsoft Support does not provide assistance with creating scripts, but documentation on Yammer license assignment is available.</span></span> <span data-ttu-id="4e297-117">Daugiau informacijos ieškokite ["Yammer" licencijų valdymas naudojant "Windows PowerShell"](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365#manage-yammer-licenses-by-using-windows-powershell).</span><span class="sxs-lookup"><span data-stu-id="4e297-117">For more info, see [Manage Yammer licenses by using Windows PowerShell](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365#manage-yammer-licenses-by-using-windows-powershell).</span></span>