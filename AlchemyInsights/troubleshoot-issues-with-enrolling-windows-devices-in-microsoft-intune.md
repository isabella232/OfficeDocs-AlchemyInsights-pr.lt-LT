---
title: "\"Windows\" įrenginių registracijos \"Microsoft Intune\" trikčių šalinimas"
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 20e9bd42-2db0-4dd7-b480-966571494dd9
ms.custom:
- "784"
- "6200002"
ms.openlocfilehash: a456cc8f2336e6b902de0b7873cb233f4b846140
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 04/15/2021
ms.locfileid: "51808979"
---
# <a name="troubleshoot-issues-with-enrolling-windows-devices-in-microsoft-intune"></a><span data-ttu-id="24464-102">"Windows" įrenginių registracijos "Microsoft Intune" trikčių šalinimas</span><span class="sxs-lookup"><span data-stu-id="24464-102">Troubleshoot issues with enrolling Windows devices in Microsoft Intune</span></span>

<span data-ttu-id="24464-103">Peržiūrėkite toliau nurodytus išteklius, kad išspręsite problemą dabar.</span><span class="sxs-lookup"><span data-stu-id="24464-103">Review the resources listed below to resolve your issue now.</span></span>
  
<span data-ttu-id="24464-104">Kai kurie dažnai pasitaikę klaidų pranešimai ir sprendimo veiksmai:</span><span class="sxs-lookup"><span data-stu-id="24464-104">Some common error messages and resolution steps:</span></span>
  
 <span data-ttu-id="24464-105">**Programinės įrangos įdiegti negalima, 0x80cf4017:** Jūsų paskyros sertifikato galiojimo laikas baigėsi.</span><span class="sxs-lookup"><span data-stu-id="24464-105">**The software cannot be installed, 0x80cf4017:** Your account certificate has expired.</span></span> <span data-ttu-id="24464-106">Iš naujo atsisiųskite kompiuterio kliento programinės įrangos paketą "Intune" administravimo konsolėje.</span><span class="sxs-lookup"><span data-stu-id="24464-106">Re-download the PC Client software package in the Intune Admin Console.</span></span> <span data-ttu-id="24464-107">Peržiūrėkite šią dokumentaciją, jei reikia daugiau informacijos.</span><span class="sxs-lookup"><span data-stu-id="24464-107">Review this documentation for more information.</span></span>
  
 <span data-ttu-id="24464-108">**Klaidos kodas 0x801c0003:** Klaida gali įvykti šiais atvejais:</span><span class="sxs-lookup"><span data-stu-id="24464-108">**Error code 0x801c0003:** The error can occur in the following scenarios:</span></span>
  
-  <span data-ttu-id="24464-109">Vartotojas turi daugiau įrenginių, užregistruotų už įrenginio limitą.</span><span class="sxs-lookup"><span data-stu-id="24464-109">The user has more devices enrolled than the device limit.</span></span> <span data-ttu-id="24464-110">Peržiūrėkite šiuos [dokumentus, kad pašalintumėte įrenginį](https://docs.microsoft.com/intune/devices-wipe) [arba pakeistumėte įrenginio limitą.](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions)</span><span class="sxs-lookup"><span data-stu-id="24464-110">Review these documents to [remove a device](https://docs.microsoft.com/intune/devices-wipe) or [change the device limit](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span></span>

-  <span data-ttu-id="24464-111">"Vartotojai gali prisijungti prie įrenginių prie "Azure AD", nustatyta kaip "nėra".</span><span class="sxs-lookup"><span data-stu-id="24464-111">"Users may join devices to Azure AD" is set to "none."</span></span> <span data-ttu-id="24464-112">Nustatykite jį visiems arba pasirinkite vartotojus.</span><span class="sxs-lookup"><span data-stu-id="24464-112">Set it to all or select users.</span></span> <span data-ttu-id="24464-113">Peržiūrėkite [šią dokumentaciją,](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) jei reikia daugiau informacijos.</span><span class="sxs-lookup"><span data-stu-id="24464-113">Review [this documentation](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) for more information.</span></span>

-  <span data-ttu-id="24464-114">Įrenginį jau užregistravo kitas vartotojas.</span><span class="sxs-lookup"><span data-stu-id="24464-114">The device is already enrolled by another user.</span></span> <span data-ttu-id="24464-115">Tokiu atveju pašalinkite įrenginį iš "Azure Intune" konsolės arba rankiniu būdu atjunkite įrenginį prieš bandydami dar kartą.</span><span class="sxs-lookup"><span data-stu-id="24464-115">If that's the case, remove the device from the Azure Intune console or manually unenroll the device before trying again.</span></span>

-  <span data-ttu-id="24464-116">Įrenginys yra "Windows 10 Home".</span><span class="sxs-lookup"><span data-stu-id="24464-116">The device is Windows 10 Home.</span></span> <span data-ttu-id="24464-117">Prie "Azure Active Directory" gali prisijungti tik "Windows 10 Pro", "Education" ir "Enterprise" SKU.</span><span class="sxs-lookup"><span data-stu-id="24464-117">Only Windows 10 Pro, Education and Enterprise SKUs can join Azure Active Directory.</span></span>

<span data-ttu-id="24464-118">Papildomi ištekliai, kurie padės išspręsti problemą:</span><span class="sxs-lookup"><span data-stu-id="24464-118">Additional resources to help resolve your issue:</span></span>
  
-  <span data-ttu-id="24464-119">Naudokite ["Intune" trikčių diagnostikos portalą,](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) kad diagnozuojant ir išspręsdami bendrąsias registracijos triktis.</span><span class="sxs-lookup"><span data-stu-id="24464-119">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="24464-120">Peržiūrėkite [šį dokumentą,](https://docs.microsoft.com/intune/help-desk-operators) jei reikia daugiau informacijos.</span><span class="sxs-lookup"><span data-stu-id="24464-120">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span>

-  <span data-ttu-id="24464-121">Peržiūrėkite šiuos dokumentus, kad būtų pateikiamas sąrašas dažnai pasitaikančių klaidų, kurios neleidžia registruotis ir išspręsti kiekvieno iš jų: Trikčių diagnostikos [vadovas](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) [ir Trikčių diagnostikos dokumentas.](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune)</span><span class="sxs-lookup"><span data-stu-id="24464-121">Review these documents for a list of common errors that prevent enrollment and resolutions to each: [Troubleshooting guide](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) and [Troubleshooting doc](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune).</span></span>

<span data-ttu-id="24464-122">[Sužinokite, kaip registruoti "Windows" įrenginius "Microsoft Intune".](https://docs.microsoft.com/intune/windows-enroll)</span><span class="sxs-lookup"><span data-stu-id="24464-122">[Learn how to enroll Windows devices in Microsoft Intune](https://docs.microsoft.com/intune/windows-enroll).</span></span>
