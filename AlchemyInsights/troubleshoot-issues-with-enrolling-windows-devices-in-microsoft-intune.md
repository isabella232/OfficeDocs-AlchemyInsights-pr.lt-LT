---
title: Trikčių šalinimas naudojant "Microsoft Intune" "Windows" įrenginius
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 20e9bd42-2db0-4dd7-b480-966571494dd9
ms.custom:
- "784"
- "6200002"
ms.openlocfilehash: 88105671ef6dc34553a265937bf1fb3463353963
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 03/10/2021
ms.locfileid: "50708898"
---
# <a name="troubleshoot-issues-with-enrolling-windows-devices-in-microsoft-intune"></a><span data-ttu-id="8dc92-102">Trikčių šalinimas naudojant "Microsoft Intune" "Windows" įrenginius</span><span class="sxs-lookup"><span data-stu-id="8dc92-102">Troubleshoot issues with enrolling Windows devices in Microsoft Intune</span></span>

<span data-ttu-id="8dc92-103">Peržiūrėkite toliau išvardytus išteklius ir Išspręskite problemą dabar.</span><span class="sxs-lookup"><span data-stu-id="8dc92-103">Review the resources listed below to resolve your issue now.</span></span>
  
<span data-ttu-id="8dc92-104">Kai kurie dažniausi klaidų laiškai ir sprendimo būdai:</span><span class="sxs-lookup"><span data-stu-id="8dc92-104">Some common error messages and resolution steps:</span></span>
  
 <span data-ttu-id="8dc92-105">**Programinės įrangos negalima įdiegti, 0x80cf4017:** Jūsų abonemento sertifikato galiojimas baigėsi.</span><span class="sxs-lookup"><span data-stu-id="8dc92-105">**The software cannot be installed, 0x80cf4017:** Your account certificate has expired.</span></span> <span data-ttu-id="8dc92-106">Iš naujo Atsisiųskite kompiuterio kliento programinės įrangos paketą "Intune" administravimo konsolėje.</span><span class="sxs-lookup"><span data-stu-id="8dc92-106">Re-download the PC Client software package in the Intune Admin Console.</span></span> <span data-ttu-id="8dc92-107">Daugiau informacijos ieškokite šiame dokumentacijoje.</span><span class="sxs-lookup"><span data-stu-id="8dc92-107">Review this documentation for more information.</span></span>
  
 <span data-ttu-id="8dc92-108">**Klaidos kodas 0x801c0003:** Klaida gali įvykti šiais atvejais:</span><span class="sxs-lookup"><span data-stu-id="8dc92-108">**Error code 0x801c0003:** The error can occur in the following scenarios:</span></span>
  
-  <span data-ttu-id="8dc92-109">Vartotojas turi daugiau įrenginių, kuriuos užregistravote kaip įrenginio limitą.</span><span class="sxs-lookup"><span data-stu-id="8dc92-109">The user has more devices enrolled than the device limit.</span></span> <span data-ttu-id="8dc92-110">Peržiūrėkite šiuos dokumentus, kad [pašalintumėte įrenginį](https://docs.microsoft.com/intune/devices-wipe) arba [pakeistumėte įrenginio limitą](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span><span class="sxs-lookup"><span data-stu-id="8dc92-110">Review these documents to [remove a device](https://docs.microsoft.com/intune/devices-wipe) or [change the device limit](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span></span>

-  <span data-ttu-id="8dc92-111">"Vartotojai gali prisijungti prie įrenginių į" Azure AD "nustatyta į" nėra ".</span><span class="sxs-lookup"><span data-stu-id="8dc92-111">"Users may join devices to Azure AD" is set to "none."</span></span> <span data-ttu-id="8dc92-112">Nustatykite visiems arba pasirinkite vartotojus.</span><span class="sxs-lookup"><span data-stu-id="8dc92-112">Set it to all or select users.</span></span> <span data-ttu-id="8dc92-113">Daugiau informacijos ieškokite [šiame dokumentacijoje](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) .</span><span class="sxs-lookup"><span data-stu-id="8dc92-113">Review [this documentation](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) for more information.</span></span>

-  <span data-ttu-id="8dc92-114">Įrenginį jau užregistravote kitas vartotojas.</span><span class="sxs-lookup"><span data-stu-id="8dc92-114">The device is already enrolled by another user.</span></span> <span data-ttu-id="8dc92-115">Jei taip, pašalinkite įrenginį iš "Azure Intune" konsolės arba rankiniu būdu išregistruokite įrenginį prieš bandydami dar kartą.</span><span class="sxs-lookup"><span data-stu-id="8dc92-115">If that's the case, remove the device from the Azure Intune console or manually unenroll the device before trying again.</span></span>

-  <span data-ttu-id="8dc92-116">Įrenginys yra "Windows 10 Home".</span><span class="sxs-lookup"><span data-stu-id="8dc92-116">The device is Windows 10 Home.</span></span> <span data-ttu-id="8dc92-117">Tik "Windows 10 Pro", "Education" ir "Enterprise SKU" gali prisijungti prie "Azure Active Directory".</span><span class="sxs-lookup"><span data-stu-id="8dc92-117">Only Windows 10 Pro, Education and Enterprise SKUs can join Azure Active Directory.</span></span>

<span data-ttu-id="8dc92-118">Papildomi ištekliai, padėsiantys išspręsti problemą:</span><span class="sxs-lookup"><span data-stu-id="8dc92-118">Additional resources to help resolve your issue:</span></span>
  
-  <span data-ttu-id="8dc92-119">Naudokite " [Intune" trikčių diagnostikos portalą](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) , kad išspręstumėte ir išspręstumėte įprastas registracijos triktis.</span><span class="sxs-lookup"><span data-stu-id="8dc92-119">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="8dc92-120">Peržiūrėkite [šį dokumentą](https://docs.microsoft.com/intune/help-desk-operators) , kad sužinotumėte daugiau.</span><span class="sxs-lookup"><span data-stu-id="8dc92-120">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span>

-  <span data-ttu-id="8dc92-121">Peržiūrėkite šiuos dokumentus, jei norite peržiūrėti dažnai pasitaikančių klaidų sąrašą, neleidžiančias įtraukti įtraukimo ir rezoliucijas: [trikčių šalinimo vadovas](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) ir [diagnostikos dokumentas](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune).</span><span class="sxs-lookup"><span data-stu-id="8dc92-121">Review these documents for a list of common errors that prevent enrollment and resolutions to each: [Troubleshooting guide](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) and [Troubleshooting doc](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune).</span></span>

<span data-ttu-id="8dc92-122">[Sužinokite, kaip užregistruoti "Windows" įrenginius "Microsoft Intune"](https://docs.microsoft.com/intune/windows-enroll).</span><span class="sxs-lookup"><span data-stu-id="8dc92-122">[Learn how to enroll Windows devices in Microsoft Intune](https://docs.microsoft.com/intune/windows-enroll).</span></span>
