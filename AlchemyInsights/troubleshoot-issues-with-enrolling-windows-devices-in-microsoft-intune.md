---
title: Šalinti triktis su mokosi Windows įrenginių Microsoft Intune
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
ms.sourcegitcommit: b3e55405af384e868fcd32ea794eb15d1356c3fc
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 08/29/2019
ms.locfileid: "36665840"
---
# <a name="troubleshoot-issues-with-enrolling-windows-devices-in-microsoft-intune"></a><span data-ttu-id="5dbe6-102">Šalinti triktis su mokosi Windows įrenginių Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="5dbe6-102">Troubleshoot issues with enrolling Windows devices in Microsoft Intune</span></span>

<span data-ttu-id="5dbe6-103">Peržiūrėkite toliau išvardytus išteklius, kad išspręstumėte problemą dabar.</span><span class="sxs-lookup"><span data-stu-id="5dbe6-103">Review the resources listed below to resolve your issue now.</span></span>
  
<span data-ttu-id="5dbe6-104">Kai kurie dažnai pasitaikę klaidų pranešimai ir sprendimo veiksmai:</span><span class="sxs-lookup"><span data-stu-id="5dbe6-104">Some common error messages and resolution steps:</span></span>
  
 <span data-ttu-id="5dbe6-105">**Programinė įranga negali būti įdiegta, 0x80cf4017:** Jūsų paskyros sertifikato galiojimo laikas baigėsi.</span><span class="sxs-lookup"><span data-stu-id="5dbe6-105">**The software cannot be installed, 0x80cf4017:** Your account certificate has expired.</span></span> <span data-ttu-id="5dbe6-106">Iš naujo atsisiųsti PC kliento programinės įrangos paketą Intune administratoriaus konsolėje.</span><span class="sxs-lookup"><span data-stu-id="5dbe6-106">Re-download the PC Client software package in the Intune Admin Console.</span></span> <span data-ttu-id="5dbe6-107">Norėdami gauti daugiau informacijos, Peržiūrėkite šį dokumentą.</span><span class="sxs-lookup"><span data-stu-id="5dbe6-107">Review this documentation for more information.</span></span>
  
 <span data-ttu-id="5dbe6-108">**Klaidos kodas 0x801c0003:** Klaida gali įvykti šiais atvejais:</span><span class="sxs-lookup"><span data-stu-id="5dbe6-108">**Error code 0x801c0003:** The error can occur in the following scenarios:</span></span>
  
-  <span data-ttu-id="5dbe6-109">Vartotojas turi daugiau įrenginių įtraukti nei įrenginio limitą.</span><span class="sxs-lookup"><span data-stu-id="5dbe6-109">The user has more devices enrolled than the device limit.</span></span> <span data-ttu-id="5dbe6-110">Peržiūrėkite šiuos dokumentus, kad [pašalintumėte įrenginį](https://docs.microsoft.com/intune/devices-wipe) arba [pakeistumėte įrenginio limitą](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span><span class="sxs-lookup"><span data-stu-id="5dbe6-110">Review these documents to [remove a device](https://docs.microsoft.com/intune/devices-wipe) or [change the device limit](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span></span>

-  <span data-ttu-id="5dbe6-111">"Vartotojai gali prisijungti prie įrenginių Azure AD" nustatyta kaip "nė vienas."</span><span class="sxs-lookup"><span data-stu-id="5dbe6-111">"Users may join devices to Azure AD" is set to "none."</span></span> <span data-ttu-id="5dbe6-112">Nustatykite ją visiems arba pasirinkite vartotojus.</span><span class="sxs-lookup"><span data-stu-id="5dbe6-112">Set it to all or select users.</span></span> <span data-ttu-id="5dbe6-113">Norėdami gauti daugiau informacijos, peržiūrėkite [šį dokumentą](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) .</span><span class="sxs-lookup"><span data-stu-id="5dbe6-113">Review [this documentation](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) for more information.</span></span>

-  <span data-ttu-id="5dbe6-114">Įrenginys jau yra užregistruotas kito vartotojo.</span><span class="sxs-lookup"><span data-stu-id="5dbe6-114">The device is already enrolled by another user.</span></span> <span data-ttu-id="5dbe6-115">Tokiu atveju pašalinkite įrenginį iš "Azure Intune" konsolės arba rankiniu būdu išregistruokite įrenginį prieš bandydami dar kartą.</span><span class="sxs-lookup"><span data-stu-id="5dbe6-115">If that's the case, remove the device from the Azure Intune console or manually unenroll the device before trying again.</span></span>

-  <span data-ttu-id="5dbe6-116">Įrenginys yra "Windows 10 Home".</span><span class="sxs-lookup"><span data-stu-id="5dbe6-116">The device is Windows 10 Home.</span></span> <span data-ttu-id="5dbe6-117">Tik Windows 10 Pro, švietimas ir Enterprise SKU gali prisijungti prie Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="5dbe6-117">Only Windows 10 Pro, Education and Enterprise SKUs can join Azure Active Directory.</span></span>

<span data-ttu-id="5dbe6-118">Papildomi ištekliai, padėsię išspręsti problemą.</span><span class="sxs-lookup"><span data-stu-id="5dbe6-118">Additional resources to help resolve your issue:</span></span>
  
-  <span data-ttu-id="5dbe6-119">Naudokite [Intune trikčių šalinimo portalas](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) diagnozuoti ir išspręsti bendras registracijos triktis.</span><span class="sxs-lookup"><span data-stu-id="5dbe6-119">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="5dbe6-120">Norėdami gauti daugiau informacijos, peržiūrėkite [šį dokumentą](https://docs.microsoft.com/intune/help-desk-operators) .</span><span class="sxs-lookup"><span data-stu-id="5dbe6-120">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span>

-  <span data-ttu-id="5dbe6-121">Peržiūrėkite šiuos dokumentus, kad būtų pateikiamas bendrų klaidų, kurios neleidžia registracijos ir rezoliucijų, sąrašas: [trikčių šalinimo vadovas](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) ir [trikčių diagnostikos dokumentas](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span><span class="sxs-lookup"><span data-stu-id="5dbe6-121">Review these documents for a list of common errors that prevent enrollment and resolutions to each: [Troubleshooting guide](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) and [Troubleshooting doc](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span></span>

<span data-ttu-id="5dbe6-122">[Sužinokite, kaip užregistruoti "Windows" įrenginius "Microsoft Intune](https://docs.microsoft.com/intune/windows-enroll)".</span><span class="sxs-lookup"><span data-stu-id="5dbe6-122">[Learn how to enroll Windows devices in Microsoft Intune](https://docs.microsoft.com/intune/windows-enroll).</span></span>
