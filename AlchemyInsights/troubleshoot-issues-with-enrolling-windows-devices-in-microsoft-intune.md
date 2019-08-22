---
title: Šalinkite triktis naudodami werbowania į Microsoft Intune "Windows" įrenginiai
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 10/24/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 20e9bd42-2db0-4dd7-b480-966571494dd9
ms.custom:
- "784"
- "6200002"
ms.openlocfilehash: be66135b80f32f78266ef2b6a7b3f5b30e24d5fc
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 08/22/2019
ms.locfileid: "36559669"
---
# <a name="troubleshoot-issues-with-enrolling-windows-devices-in-microsoft-intune"></a><span data-ttu-id="fee97-102">Šalinkite triktis naudodami werbowania į Microsoft Intune "Windows" įrenginiai</span><span class="sxs-lookup"><span data-stu-id="fee97-102">Troubleshoot issues with enrolling Windows devices in Microsoft Intune</span></span>

<span data-ttu-id="fee97-103">Peržiūrėkite žemiau siekiama išspręsti jūsų problemą dabar ištekliai.</span><span class="sxs-lookup"><span data-stu-id="fee97-103">Review the resources listed below to resolve your issue now.</span></span>
  
<span data-ttu-id="fee97-104">Kai kurių įprastinių klaidos prane imų ir sprendimo veiksmai:</span><span class="sxs-lookup"><span data-stu-id="fee97-104">Some common error messages and resolution steps:</span></span>
  
 <span data-ttu-id="fee97-105">**Negali būti įdiegta programinė įranga, 0x80cf4017:** Jūsų paskyros sertifikatas nebegalioja.</span><span class="sxs-lookup"><span data-stu-id="fee97-105">**The software cannot be installed, 0x80cf4017:** Your account certificate has expired.</span></span> <span data-ttu-id="fee97-106">Iš naujo atsisiųsti PC kliento programinės įrangos paketą Intune administratoriaus konsolėje.</span><span class="sxs-lookup"><span data-stu-id="fee97-106">Re-download the PC Client software package in the Intune Admin Console.</span></span> <span data-ttu-id="fee97-107">Peržiūrėti šiuos dokumentus daugiau informacijos.</span><span class="sxs-lookup"><span data-stu-id="fee97-107">Review this documentation for more information.</span></span>
  
 <span data-ttu-id="fee97-108">**Klaidos kodas 0x801c0003:** Klaida gali atsirasti šie scenarijai:</span><span class="sxs-lookup"><span data-stu-id="fee97-108">**Error code 0x801c0003:** The error can occur in the following scenarios:</span></span>
  
1. <span data-ttu-id="fee97-109">Vartotojas turi daugiau įrenginius, užregistruotus nei įrenginio.</span><span class="sxs-lookup"><span data-stu-id="fee97-109">The user has more devices enrolled than the device limit.</span></span> <span data-ttu-id="fee97-110">Peržiūrėkite šiuos dokumentus [pašalinti įrenginį](https://docs.microsoft.com/intune/devices-wipe) arba [pakeisti įrenginio](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span><span class="sxs-lookup"><span data-stu-id="fee97-110">Review these documents to [remove a device](https://docs.microsoft.com/intune/devices-wipe) or [change the device limit](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span></span>

2. <span data-ttu-id="fee97-111">"Vartotojai gali prisijungti prie įrenginių Azure AD" nustatykite "none".</span><span class="sxs-lookup"><span data-stu-id="fee97-111">"Users may join devices to Azure AD" is set to "none".</span></span> <span data-ttu-id="fee97-112">Nustatyti visiems arba pasirinkite vartotojai.</span><span class="sxs-lookup"><span data-stu-id="fee97-112">Set it to all or select users.</span></span> <span data-ttu-id="fee97-113">Peržiūrėkite [šiuos dokumentus](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) daugiau informacijos.</span><span class="sxs-lookup"><span data-stu-id="fee97-113">Review [this documentation](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) for more information.</span></span>

3. <span data-ttu-id="fee97-114">Prietaisas jau mokosi kitas vartotojas.</span><span class="sxs-lookup"><span data-stu-id="fee97-114">The device is already enrolled by another user.</span></span> <span data-ttu-id="fee97-115">Jei tai byla, pašalinti įrenginį iš Azure Intune konsolės arba rankiniu būdu unenroll įrenginį, prieš bandydami dar kartą.</span><span class="sxs-lookup"><span data-stu-id="fee97-115">If that's the case, remove the device from the Azure Intune console or manually unenroll the device before trying again.</span></span>

4. <span data-ttu-id="fee97-116">Prietaisas veikia Windows 10 namuose.</span><span class="sxs-lookup"><span data-stu-id="fee97-116">The device is Windows 10 Home.</span></span> <span data-ttu-id="fee97-117">Tik "Windows 10 Pro", švietimo ir Enterprise SKU prisijungti prie Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="fee97-117">Only Windows 10 Pro, Education and Enterprise SKUs can join Azure Active Directory.</span></span>

<span data-ttu-id="fee97-118">Papildomų išteklių, kurie padės išspręsti jūsų problemą:</span><span class="sxs-lookup"><span data-stu-id="fee97-118">Additional resources to help resolve your issue:</span></span>
  
1. <span data-ttu-id="fee97-119">Naudoti [Intune trikčių šalinimo portalas](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) diagnozuoti ir išspręsti bendras registracijos nesėkmių.</span><span class="sxs-lookup"><span data-stu-id="fee97-119">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="fee97-120">Peržiūrėti daugiau informacijos [šiame dokumente](https://docs.microsoft.com/intune/help-desk-operators) .</span><span class="sxs-lookup"><span data-stu-id="fee97-120">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span>

2. <span data-ttu-id="fee97-121">Peržiūrėkite šiuos dokumentus bendrosios klaidos, kurios neleis registracijos ir rezoliucijas į kiekvieną sąrašą: [trikčių diagnostikos vadovas](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) ir [trikčių diagnostika doc](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span><span class="sxs-lookup"><span data-stu-id="fee97-121">Review these documents for a list of common errors that prevent enrollment and resolutions to each: [Troubleshooting guide](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) and [Troubleshooting doc](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span></span>

<span data-ttu-id="fee97-122">[Sužinokite, kaip įtraukti į Microsoft Intune "Windows" įrenginiuose](https://docs.microsoft.com/intune/windows-enroll).</span><span class="sxs-lookup"><span data-stu-id="fee97-122">[Learn how to enroll Windows devices in Microsoft Intune](https://docs.microsoft.com/intune/windows-enroll).</span></span>
