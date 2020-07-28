---
title: Automatinių "Office Apps" naujinimų valdymas
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/24/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1743"
- "9000140"
ms.openlocfilehash: 5c56c3adcc9a06db43d4df6f367657cb8ff0c8c8
ms.sourcegitcommit: b10cea11b4975354b91193327b58aa4740d34833
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 07/28/2020
ms.locfileid: "45439336"
---
# <a name="control-automatic-updates-for-office-apps"></a><span data-ttu-id="e351f-102">Automatinių "Office Apps" naujinimų valdymas</span><span class="sxs-lookup"><span data-stu-id="e351f-102">Control automatic updates for Office Apps</span></span>

<span data-ttu-id="e351f-103">Pagal numatytuosius nustatymus "Office Apps" naujinimai atsisiunčiami automatiškai ir taikomi fone be jokio vartotojo įsikišimo.</span><span class="sxs-lookup"><span data-stu-id="e351f-103">By default, updates for Office Apps are downloaded automatically and applied in the background without any user intervention.</span></span> <span data-ttu-id="e351f-104">Tačiau administratoriai gali valdyti, kaip naujinimai taikomi naudojant "Office Update" parametrus.</span><span class="sxs-lookup"><span data-stu-id="e351f-104">However, administrators can control how updates are applied by using Office Update settings.</span></span> <span data-ttu-id="e351f-105">Naujinimo parametrai leidžia administratoriams įgalinti arba išjungti automatinius naujinimus, rodyti arba slėpti mygtuką **Naujinti dabar** "Office", nustatyti naujinimo terminus ir kt.</span><span class="sxs-lookup"><span data-stu-id="e351f-105">Update settings allow administrators to enable or disable automatic updates, show or hide the **Update Now** button in Office, set update deadlines, and more.</span></span> <span data-ttu-id="e351f-106">Išsamesnės informacijos ieškokite:</span><span class="sxs-lookup"><span data-stu-id="e351f-106">For detailed information, see:</span></span>

- [<span data-ttu-id="e351f-107">"Office" naujinimo parametrų konfigūravimas</span><span class="sxs-lookup"><span data-stu-id="e351f-107">Configure update settings for Office</span></span>](https://docs.microsoft.com/deployoffice/configure-update-settings-for-office-365-proplus)  
- [<span data-ttu-id="e351f-108">Automatinis "Office" naujinimas neįgalintas</span><span class="sxs-lookup"><span data-stu-id="e351f-108">Automatic updating for Office is not enabled</span></span>](https://support.microsoft.com/help/2753538/automatic-updating-for-office-2013-and-office-2016-click-to-run-is-not)  
- [<span data-ttu-id="e351f-109">Nustatyti, kaip "Office" atnaujinamas jį įdiegus</span><span class="sxs-lookup"><span data-stu-id="e351f-109">Define how Office is updated after it's installed</span></span>](https://docs.microsoft.com/deployoffice/configuration-options-for-the-office-2016-deployment-tool#updates-element)

<span data-ttu-id="e351f-110">Norėdami peržiūrėti esamus naujinimus parametrus, taikomus kliento kompiuteryje, atlikite šiuos veiksmus:</span><span class="sxs-lookup"><span data-stu-id="e351f-110">To review the existing updates settings applied to a client machine, follow these steps:</span></span>

1. <span data-ttu-id="e351f-111">Atidarykite registro rengyklę, eikite į **Pradėti**  >  **vykdyti**  >  **regedit**.</span><span class="sxs-lookup"><span data-stu-id="e351f-111">Open the Registry Editor by going to **Start** > **Run** > **regedit**.</span></span>
2. <span data-ttu-id="e351f-112">Pereikite į šią vietą ir peržiūrėkite "Office Update" parametrus:</span><span class="sxs-lookup"><span data-stu-id="e351f-112">Switch to the following location and review the Office Update settings:</span></span>  
    <span data-ttu-id="e351f-113">A.</span><span class="sxs-lookup"><span data-stu-id="e351f-113">a.</span></span> <span data-ttu-id="e351f-114">HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Office</span><span class="sxs-lookup"><span data-stu-id="e351f-114">HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Office</span></span>\  
    <span data-ttu-id="e351f-115">B.</span><span class="sxs-lookup"><span data-stu-id="e351f-115">b.</span></span> <span data-ttu-id="e351f-116">Spustelėkite ĮVykdyti\Konfigūracija</span><span class="sxs-lookup"><span data-stu-id="e351f-116">ClickToRun\Configuration</span></span>

<span data-ttu-id="e351f-117">**Pastaba**  Jei OfficeMgmtCOM raktas nustatytas, **"Office Account**Office" naujinimuose gali būti rodomas pranešimas "Naujinimai valdo sistemos  >  **Account**  >  **administratorius".**</span><span class="sxs-lookup"><span data-stu-id="e351f-117">**Note**  If the OfficeMgmtCOM key is set, you might see the "Updates are managed by your system administrator" message in **Office** > **Account** > **Office Updates**.</span></span> <span data-ttu-id="e351f-118">Jei norite gauti daugiau informacijos, [peržiūrėkite tvarkyti naujinimus į Microsoft 365 apps su Microsoft Endpoint Configuration Manager](https://docs.microsoft.com/deployoffice/manage-updates-to-office-365-proplus-with-system-center-configuration-manager#method-1-use-office-deployment-tool-to-enable-office-365-clients-to-receive-updates-from-configuration-manager).</span><span class="sxs-lookup"><span data-stu-id="e351f-118">For more info, see [Manage updates to Microsoft 365 Apps with Microsoft Endpoint Configuration Manager](https://docs.microsoft.com/deployoffice/manage-updates-to-office-365-proplus-with-system-center-configuration-manager#method-1-use-office-deployment-tool-to-enable-office-365-clients-to-receive-updates-from-configuration-manager).</span></span>  