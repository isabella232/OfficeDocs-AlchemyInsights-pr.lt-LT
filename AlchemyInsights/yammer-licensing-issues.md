---
title: "\"Yammer\" licencijavimo problemos"
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/14/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5900"
- "9003071"
ms.openlocfilehash: 6d9b2126dc1ed90968738ddb2e249dce9857f1db
ms.sourcegitcommit: b677b85395b7244b2bf2b753468b696b4cf27c8d
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 07/16/2020
ms.locfileid: "45148314"
---
# <a name="yammer-licensing-issues"></a><span data-ttu-id="11e03-102">"Yammer" licencijavimo problemos</span><span class="sxs-lookup"><span data-stu-id="11e03-102">Yammer licensing issues</span></span>

<span data-ttu-id="11e03-103">Visi vartotojai turi turėti licenciją naudoti "Yammer Enterprise" paslaugą, tačiau pagal numatytuosius nustatymus "Yammer" nereikalauja, kad vartotojai turėtų licenciją naudotis paslauga.</span><span class="sxs-lookup"><span data-stu-id="11e03-103">All users must have a license to use the Yammer Enterprise service, but by default Yammer does not require that users have a license to access the service.</span></span> <span data-ttu-id="11e03-104">Kai administratorius pakeičia parametrą blokuoti "Microsoft 365" vartotojus be "Yammer" licencijų, vartotojai, kuriems nepriskirta "Yammer Enterprise" licencija, negali pasiekti "Yammer" paslaugos.</span><span class="sxs-lookup"><span data-stu-id="11e03-104">When an administrator changes the setting to block Microsoft 365 users without Yammer licenses, users not assigned a Yammer Enterprise license can't access the Yammer service.</span></span> <span data-ttu-id="11e03-105">Daugiau informacijos rasite ["Yammer" vartotojų licencijų valdymas "Office 365"](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365)</span><span class="sxs-lookup"><span data-stu-id="11e03-105">For more info, see [Manage Yammer user licenses in Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365)</span></span> 

<span data-ttu-id="11e03-106">Kai licencijos pašalinamos iš vartotojų, "Yammer" plytelė neberodomas, o kitos tarnybos gali naudoti licencijos šalinimą funkcijoms slėpti.</span><span class="sxs-lookup"><span data-stu-id="11e03-106">When licenses are removed from users, the Yammer tile is no longer displayed, and other services can use license removal to hide features.</span></span> <span data-ttu-id="11e03-107">Kitais atvejais funkcijos vis tiek gali pasirodyti, tačiau joms reikia suteikti licenciją.</span><span class="sxs-lookup"><span data-stu-id="11e03-107">In other cases, features can still appear but require licence assignment to operate.</span></span>  

<span data-ttu-id="11e03-108">**Licencija neatnaujinama vartotojui**</span><span class="sxs-lookup"><span data-stu-id="11e03-108">**License is not getting updated for the user**</span></span>  

<span data-ttu-id="11e03-109">Kartais vartotojui priskiriama licencija, bet vis tiek nepavyksta pasiekti "Yammer".</span><span class="sxs-lookup"><span data-stu-id="11e03-109">Occasionally, a user is assigned a license but is still unable to access Yammer.</span></span> <span data-ttu-id="11e03-110">Delsa yra labiau tikėtina, kai masinis licencijos priskyrimas vyksta.</span><span class="sxs-lookup"><span data-stu-id="11e03-110">Delays are more likely to occur when a mass license assignment is in progress.</span></span> <span data-ttu-id="11e03-111">"Yammer" vartotojai gali būti neatnaujinti ta pačia tvarka, kaip licencijos pakeičiamos Azure AD, nes sistema veikia asinchroniškai.</span><span class="sxs-lookup"><span data-stu-id="11e03-111">Yammer users might not be updated in the same order as licenses are changed in Azure AD because the system runs asynchronously.</span></span> <span data-ttu-id="11e03-112">Palaukite iki 24 valandų, kol atidarydami palaikymo atvejį praneškite apie licencijos sinchronizavimo problemas.</span><span class="sxs-lookup"><span data-stu-id="11e03-112">Wait up to 24 hours before opening a support case to report license sync issues.</span></span>  

<span data-ttu-id="11e03-113">**Masinis licencijų priskyrimas**</span><span class="sxs-lookup"><span data-stu-id="11e03-113">**Bulk licence assignment**</span></span>  

<span data-ttu-id="11e03-114">Licencijos gali būti priskirtos per administravimo centrą arba "PowerShell" scenarijus.</span><span class="sxs-lookup"><span data-stu-id="11e03-114">Licenses can be assigned through the admin center or PowerShell scripting.</span></span> <span data-ttu-id="11e03-115">Daugiau informacijos rasite [Licencijų priskyrimas vartotojams](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) ir [Licencijų priskyrimas vartotojų abonementams naudojant "Office 365 PowerShell".](https://docs.microsoft.com/office365/enterprise/powershell/assign-licenses-to-user-accounts-with-office-365-powershell)</span><span class="sxs-lookup"><span data-stu-id="11e03-115">For more info, see [Assign licenses to users](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) and [Assign licenses to user accounts with Office 365 PowerShell](https://docs.microsoft.com/office365/enterprise/powershell/assign-licenses-to-user-accounts-with-office-365-powershell).</span></span> 

<span data-ttu-id="11e03-116">"Microsoft" palaikymo tarnyba neteikia pagalbos kuriant scenarijus, bet galima naudoti "Yammer" licencijos priskyrimo dokumentaciją.</span><span class="sxs-lookup"><span data-stu-id="11e03-116">Microsoft Support does not provide assistance with creating scripts, but documentation on Yammer license assignment is available.</span></span> <span data-ttu-id="11e03-117">Daugiau informacijos rasite ["Yammer" licencijų valdymas naudojant "Windows PowerShell".](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365#manage-yammer-licenses-by-using-windows-powershell)</span><span class="sxs-lookup"><span data-stu-id="11e03-117">For more info, see [Manage Yammer licenses by using Windows PowerShell](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365#manage-yammer-licenses-by-using-windows-powershell).</span></span>