---
title: "\"Windows\" įrenginių įtraukimo į \"Microsoft Intune\" trikčių šalinimas"
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 20e9bd42-2db0-4dd7-b480-966571494dd9
ms.custom:
- "784"
- "6200002"
ms.openlocfilehash: 7b298360fe31d3f52ef382e5b8f25ee3588c36c8
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 06/02/2020
ms.locfileid: "36665840"
---
# <a name="troubleshoot-issues-with-enrolling-windows-devices-in-microsoft-intune"></a><span data-ttu-id="71e96-102">"Windows" įrenginių įtraukimo į "Microsoft Intune" trikčių šalinimas</span><span class="sxs-lookup"><span data-stu-id="71e96-102">Troubleshoot issues with enrolling Windows devices in Microsoft Intune</span></span>

<span data-ttu-id="71e96-103">Peržiūrėkite toliau išvardytus išteklius, kad išspręstumėte problemą dabar.</span><span class="sxs-lookup"><span data-stu-id="71e96-103">Review the resources listed below to resolve your issue now.</span></span>
  
<span data-ttu-id="71e96-104">Kai kurie dažniausiai pasitaikantys klaidų pranešimai ir sprendimo veiksmai:</span><span class="sxs-lookup"><span data-stu-id="71e96-104">Some common error messages and resolution steps:</span></span>
  
 <span data-ttu-id="71e96-105">**Programinės įrangos įdiegti negalima, 0x80cf4017:** Baigėsi abonemento sertifikato galiojimo laikas.</span><span class="sxs-lookup"><span data-stu-id="71e96-105">**The software cannot be installed, 0x80cf4017:** Your account certificate has expired.</span></span> <span data-ttu-id="71e96-106">Iš naujo atsisiųskite kompiuterio kliento programinės įrangos paketą "Intune" administravimo konsolėje.</span><span class="sxs-lookup"><span data-stu-id="71e96-106">Re-download the PC Client software package in the Intune Admin Console.</span></span> <span data-ttu-id="71e96-107">Peržiūrėkite šią dokumentaciją, jei norite gauti daugiau informacijos.</span><span class="sxs-lookup"><span data-stu-id="71e96-107">Review this documentation for more information.</span></span>
  
 <span data-ttu-id="71e96-108">**Klaidos kodas 0x801c0003:** Klaida gali įvykti šiais atvejais:</span><span class="sxs-lookup"><span data-stu-id="71e96-108">**Error code 0x801c0003:** The error can occur in the following scenarios:</span></span>
  
-  <span data-ttu-id="71e96-109">Vartotojas turi daugiau įrenginių, įtrauktų nei įrenginio riba.</span><span class="sxs-lookup"><span data-stu-id="71e96-109">The user has more devices enrolled than the device limit.</span></span> <span data-ttu-id="71e96-110">Peržiūrėkite šiuos dokumentus, kad [pašalintumėte įrenginį](https://docs.microsoft.com/intune/devices-wipe) arba [pakeistumėte įrenginio limitą](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span><span class="sxs-lookup"><span data-stu-id="71e96-110">Review these documents to [remove a device](https://docs.microsoft.com/intune/devices-wipe) or [change the device limit](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span></span>

-  <span data-ttu-id="71e96-111">"Vartotojai gali prisijungti prie įrenginių Azure AD" yra nustatyta kaip "nėra."</span><span class="sxs-lookup"><span data-stu-id="71e96-111">"Users may join devices to Azure AD" is set to "none."</span></span> <span data-ttu-id="71e96-112">Nustatykite jį visiems arba pasirinkite vartotojus.</span><span class="sxs-lookup"><span data-stu-id="71e96-112">Set it to all or select users.</span></span> <span data-ttu-id="71e96-113">Peržiūrėkite [šią dokumentaciją,](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) jei norite gauti daugiau informacijos.</span><span class="sxs-lookup"><span data-stu-id="71e96-113">Review [this documentation](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) for more information.</span></span>

-  <span data-ttu-id="71e96-114">Įrenginį jau užregistravo kitas vartotojas.</span><span class="sxs-lookup"><span data-stu-id="71e96-114">The device is already enrolled by another user.</span></span> <span data-ttu-id="71e96-115">Tokiu atveju pašalinkite įrenginį iš "Azure Intune" konsolės arba rankiniu būdu išnaujoužkite įrenginį prieš bandydami dar kartą.</span><span class="sxs-lookup"><span data-stu-id="71e96-115">If that's the case, remove the device from the Azure Intune console or manually unenroll the device before trying again.</span></span>

-  <span data-ttu-id="71e96-116">Įrenginys yra "Windows 10 Home".</span><span class="sxs-lookup"><span data-stu-id="71e96-116">The device is Windows 10 Home.</span></span> <span data-ttu-id="71e96-117">Tik "Windows 10 Pro", "Education" ir "Enterprise" SKU gali prisijungti prie "Azure Active Directory".</span><span class="sxs-lookup"><span data-stu-id="71e96-117">Only Windows 10 Pro, Education and Enterprise SKUs can join Azure Active Directory.</span></span>

<span data-ttu-id="71e96-118">Papildomi ištekliai, padėsiantys išspręsti problemą:</span><span class="sxs-lookup"><span data-stu-id="71e96-118">Additional resources to help resolve your issue:</span></span>
  
-  <span data-ttu-id="71e96-119">Naudokite [Intune trikčių diagnostikos portalas](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) diagnozuoti ir išspręsti bendrąsias registracijos klaidas.</span><span class="sxs-lookup"><span data-stu-id="71e96-119">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="71e96-120">Peržiūrėkite [šį dokumentą,](https://docs.microsoft.com/intune/help-desk-operators) jei norite gauti daugiau informacijos.</span><span class="sxs-lookup"><span data-stu-id="71e96-120">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span>

-  <span data-ttu-id="71e96-121">Peržiūrėkite šiuos dokumentus, kad būtų pateiktas dažniausiai pasitaikančių klaidų, kurios neleidžia registruotis ir šalinti kiekvieno sąskirstys: [trikčių šalinimo vadovas](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) ir [trikčių šalinimo dokumentas](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune), sąrašas.</span><span class="sxs-lookup"><span data-stu-id="71e96-121">Review these documents for a list of common errors that prevent enrollment and resolutions to each: [Troubleshooting guide](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) and [Troubleshooting doc](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span></span>

<span data-ttu-id="71e96-122">[Sužinokite, kaip užregistruoti "Windows" įrenginius "Microsoft Intune".](https://docs.microsoft.com/intune/windows-enroll)</span><span class="sxs-lookup"><span data-stu-id="71e96-122">[Learn how to enroll Windows devices in Microsoft Intune](https://docs.microsoft.com/intune/windows-enroll).</span></span>
