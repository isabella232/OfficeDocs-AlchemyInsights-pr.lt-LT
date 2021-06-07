---
title: Aktyvinti „Office“ nepavyko
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "2000023"
- "3509"
ms.openlocfilehash: 81941d84127a096c3bd588dafc61b492ab6d6458
ms.sourcegitcommit: 1eee2412dfb8b1f10a3aa28dd1086a0c589cdba0
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 06/07/2021
ms.locfileid: "52798688"
---
# <a name="unable-to-activate-office"></a><span data-ttu-id="35988-102">Aktyvinti „Office“ nepavyko</span><span class="sxs-lookup"><span data-stu-id="35988-102">Unable to activate Office</span></span>

<span data-ttu-id="35988-103">**Pastaba:** jei naudojate senesnę "Windows versiją (pvz., "Windows 7"), įsitikinkite, kad TLS 1.2 įgalinta kaip numatytoji.</span><span class="sxs-lookup"><span data-stu-id="35988-103">**Note**: If you are using an older version of Windows (For example, Windows 7), ensure that TLS 1.2 is enabled as the default.</span></span> <span data-ttu-id="35988-104">Daugiau informacijos žr. Naujinimas, kad [įgalintumėte TLS 1.1 ir TLS 1.2 kaip numatytuosius saugos protokolus "WinHTTP" Windows.](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392)</span><span class="sxs-lookup"><span data-stu-id="35988-104">For more information, see [Update to enable TLS 1.1 and TLS 1.2 as default secure protocols in WinHTTP in Windows](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392).</span></span>

- <span data-ttu-id="35988-105">Patikrinkite, ar jūsų prenumeratos galiojimas nėra pasibaigęs.</span><span class="sxs-lookup"><span data-stu-id="35988-105">Check if your subscription status has expired.</span></span>
- <span data-ttu-id="35988-106">Įsitikinkite, kad turite prenumeratą, leidžiančią naudoti kliento licencijas, pvz., „Office 365 Business“ arba „Business Premium“, ir [įsitikinkite, kad vartotojui yra priskirta licencija](/microsoft-365/admin/manage/assign-licenses-to-users).</span><span class="sxs-lookup"><span data-stu-id="35988-106">Ensure you have a subscription that allows client licenses, such as Office 365 Business or Business Premium, and [ensure the user has a license assigned](/microsoft-365/admin/manage/assign-licenses-to-users).</span></span>
- <span data-ttu-id="35988-107">Įsitikinkite, kad vartotojas prie „Office“ yra prisijungęs su paskyra, kuriai priskirta licencija.</span><span class="sxs-lookup"><span data-stu-id="35988-107">Ensure the user is signing into Office with the same account that has the license assigned.</span></span>
- <span data-ttu-id="35988-108">Peržiūrėkite [„Office 365“ tarnybų sveikatos puslapį](/office365/enterprise/view-service-health), kad sužinotumėte, ar yra žinomų tarnybos problemų.</span><span class="sxs-lookup"><span data-stu-id="35988-108">Check the [Office 365 Service Health page](/office365/enterprise/view-service-health) to see if there are any known problems with the service.</span></span>
- <span data-ttu-id="35988-109">Patikrinkite užkardos, antivirusinės programos ir tarpinio serverio parametrus, kad užtikrintumėte, jog jie neblokuoja „Microsoft 365“ programų prieigos prie interneto.</span><span class="sxs-lookup"><span data-stu-id="35988-109">Check your firewall, antivirus software and proxy settings to confirm that they are not blocking Microsoft 365 apps access to the internet.</span></span> <span data-ttu-id="35988-110">Žr. [„Office 365“ URL ir IP adresų diapazonai](/office365/enterprise/urls-and-ip-address-ranges "„Office 365“ URL ir IP adresų diapazonai").</span><span class="sxs-lookup"><span data-stu-id="35988-110">Please see [Office 365 URLs and IP address ranges](/office365/enterprise/urls-and-ip-address-ranges "Office 365 URLs and IP address ranges").</span></span>

<span data-ttu-id="35988-111">**Patarimas** „Windows“ kompiuteriuose galime diagnozuoti ir automatiškai už jus išspręsti kelias bendrąsias „Office“ prisijungimo problemas.</span><span class="sxs-lookup"><span data-stu-id="35988-111">**Tip** On Windows machines, we can diagnose and automatically fix several common Office sign-in issues for you.</span></span> <span data-ttu-id="35988-112">Atsisiųskite ir paleiskite **[„Microsoft“ palaikymo ir atkūrimo pagalbinę priemonę](https://aka.ms/SaRA-OfficeSignInScenario)**, kad būtų galima naudoti mūsų automatinį įrankį.</span><span class="sxs-lookup"><span data-stu-id="35988-112">Download and run the  **[Microsoft Support and Recovery Assistant](https://aka.ms/SaRA-OfficeSignInScenario)** to use our automated tool.</span></span>

<span data-ttu-id="35988-113">Atlikite šiuos problemų sprendimo veiksmus:</span><span class="sxs-lookup"><span data-stu-id="35988-113">Use the following troubleshooting actions:</span></span>

- <span data-ttu-id="35988-114">Atidarykite „Office“ taikomąją programą ir [atsijunkite](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) nuo bet kokių esamų vartotojų paskyrų.</span><span class="sxs-lookup"><span data-stu-id="35988-114">Open an Office app, and [sign out](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) of any existing user accounts.</span></span> <span data-ttu-id="35988-115">[Pašalinkite](/microsoft-365/admin/manage/remove-licenses-from-users) ir [iš naujo priskirkite](/microsoft-365/admin/manage/assign-licenses-to-users) „Office“ licenciją, tada [prisijunkite prie „Office“](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) naudodami paveiktą vartotojo paskyrą.</span><span class="sxs-lookup"><span data-stu-id="35988-115">[Remove](/microsoft-365/admin/manage/remove-licenses-from-users) and [re-assign](/microsoft-365/admin/manage/assign-licenses-to-users) Office license, and then [sign into Office](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) using the affected user account.</span></span>
- <span data-ttu-id="35988-116">Paleiskite [Aktyvinimo trikčių diagnostikos priemonę](https://aka.ms/SARA-OfficeActivation-Alchemy)</span><span class="sxs-lookup"><span data-stu-id="35988-116">Run the [Activation Troubleshooter](https://aka.ms/SARA-OfficeActivation-Alchemy)</span></span>
- [<span data-ttu-id="35988-117">Nustatykite „Office“ aktyvinimo būseną iš naujo</span><span class="sxs-lookup"><span data-stu-id="35988-117">Reset Office activation state</span></span>](/office365/troubleshoot/activation/reset-office-365-proplus-activation-state "Nustatykite „Office“ aktyvinimo būseną iš naujo")
- [<span data-ttu-id="35988-118">Atlikti „Office“ atkūrimą internete</span><span class="sxs-lookup"><span data-stu-id="35988-118">Perform an Online Repair of Office</span></span>](https://support.office.com/Article/7821d4b6-7c1d-4205-aa0e-a6b40c5bb88b?wt.mc_id=Alchemy_ClientDIA)

<span data-ttu-id="35988-119">Jei reikia papildomų problemų sprendimo patarimų, žr.:</span><span class="sxs-lookup"><span data-stu-id="35988-119">For additional troubleshooting solutions, see:</span></span>  

- [<span data-ttu-id="35988-120">Nelicencijuoto produkto ir aktyvinimo klaidos „Office“</span><span class="sxs-lookup"><span data-stu-id="35988-120">Unlicensed Product and activation errors in Office</span></span>](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380?wt.mc_id=Alchemy_ClientDIA)
- [<span data-ttu-id="35988-121">„Atsiprašome, negalime prisijungti prie jūsų paskyros. Bandykite dar kartą vėliau“ klaida, pasirodanti jums aktyvinus „Office“</span><span class="sxs-lookup"><span data-stu-id="35988-121">"Sorry, we can't connect to your account. Please try again later" error when you activate Office</span></span>](/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365)