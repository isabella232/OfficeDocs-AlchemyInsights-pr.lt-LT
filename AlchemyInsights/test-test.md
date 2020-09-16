---
title: "\"SharePoint Online\" terminų saugyklos sąlygos"
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1243"
- "5200021"
ms.openlocfilehash: 06711c289365c0fcdf71cf9cccf3cfc53511495a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47750459"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a><span data-ttu-id="ab716-102">"BitLocker" šifravimo su "Intune" įgalinimas</span><span class="sxs-lookup"><span data-stu-id="ab716-102">Enabling Bitlocker Encryption with Intune</span></span>

<span data-ttu-id="ab716-103">"Intune Endpoint Protection" strategiją galima naudoti norint sukonfigūruoti "Windows" įrenginių Boitlocker šifravimo parametrus, kaip aprašyta: Windows10 (ir vėlesni) parametrai, skirti apsaugoti įrenginius naudojant Intune</span><span class="sxs-lookup"><span data-stu-id="ab716-103">Intune Endpoint Protection Policy can be used to configure Boitlocker encryption settings for Windows devices as described in : Windows10 (and later) settings to protect devices using Intune</span></span>

<span data-ttu-id="ab716-104">Turėtumėte žinoti, kad daugelis naujesnių įrenginių, kuriuose veikia "Windows 10", palaiko automatinį "BitLocker" šifravimą, kuris paleidžiamas nenaudojant MDM strategijos.</span><span class="sxs-lookup"><span data-stu-id="ab716-104">You should be aware that many newer devices running Windows 10 support automatic bitlocker encryption which is triggered without the application of MDM policy.</span></span> <span data-ttu-id="ab716-105">Tai gali turėti įtakos strategijos taikymui, jei nenumatytieji parametrai yra sukonfigūruoti.</span><span class="sxs-lookup"><span data-stu-id="ab716-105">This may impact application of policy if non default settings are configured.</span></span> <span data-ttu-id="ab716-106">Išsamiau žr DUK.</span><span class="sxs-lookup"><span data-stu-id="ab716-106">See FAQ for more detail.</span></span>


<span data-ttu-id="ab716-107">DUK   k: kokių "Windows" palaikymo įrenginių šifravimo leidimų naudojant Endpoint Protection strategiją?</span><span class="sxs-lookup"><span data-stu-id="ab716-107">FAQ  Q: Which editions of Windows support device encryption using the Endpoint Protection Policy?</span></span>
<span data-ttu-id="ab716-108"> A: "Intune Endpoint Protection" strategijos parametrai vykdomi naudojant "BitLocker" CSP.</span><span class="sxs-lookup"><span data-stu-id="ab716-108"> A: The settings in Intune Endpoint Protection Policy  are implemented using the Bitlocker CSP.</span></span><span data-ttu-id="ab716-109">Ne visi leidimai ir "Windows" komponavimo versijos nepalaiko "BitLocker" CSP. 
     </span><span class="sxs-lookup"><span data-stu-id="ab716-109">  Not all editions nor builds of Windows support the Bitlocker CSP. 
     </span></span> <span data-ttu-id="ab716-110">Šiuo metu "Windows" leidimuose: Enterprise; Švietimo, mobilioji, mobilioji įmonė ir specialistas (1809 komponavimo versijoje) yra palaikomos.</span><span class="sxs-lookup"><span data-stu-id="ab716-110">At this time Windows Editions: Enterprise; Education, Mobile, Mobile Enterprise and Professional (from build 1809 onwards) are supported.</span></span>




<span data-ttu-id="ab716-111">K: Jei įrenginys jau užšifruotas naudojant "BitLocker", kai šifravimo metodui ir šifro atsparumui OS numatytuosius parametrus (XTS-AES-128) bus taikoma strategija su skirtingais parametrais, automatiškai suaktyvins disko, kuriame yra nauji parametrai, šifravimą?</span><span class="sxs-lookup"><span data-stu-id="ab716-111">Q: If a device is already encrypted with Bitlocker using the OS default settings for encryption method and cipher strength (XTS-AES-128)  will applying a policy with different settings automatically trigger re-encryption of the drive with the new settings?</span></span>

<span data-ttu-id="ab716-112">A.: Ne.</span><span class="sxs-lookup"><span data-stu-id="ab716-112">A: No.</span></span> <span data-ttu-id="ab716-113">Norint taikyti naujus šifro parametrus, pirmiausia reikia iššifruoti loginį diską.</span><span class="sxs-lookup"><span data-stu-id="ab716-113">In order to apply the new cipher settings the drive must first be decrypted.</span></span>

<span data-ttu-id="ab716-114">Pastaba "Autopilot" registruotam įrenginiams Automatinis šifravimas, įvykęs OOBE metu, nėra paleidžiamas, kol bus įvertinta "Intune" strategija, kuri leidžia naudoti strategijos parametrus vietoj OS numatytųjų reikšmių</span><span class="sxs-lookup"><span data-stu-id="ab716-114">Note For devices being enrolled with Autopilot the automatic encryption that would occur during OOBE is not triggered until Intune policy is evaluated which allows the policy based settings to be used in place of the OS defaults</span></span>




<span data-ttu-id="ab716-115">K jei įrenginys užšifruotas kaip "Intune" strategijos taikymas, jis bus iššifruotas pašalinus šią strategiją?</span><span class="sxs-lookup"><span data-stu-id="ab716-115">Q If a device is encrypted as a result of the  application of Intune policy will it be decrypted when that policy is removed?</span></span>

<span data-ttu-id="ab716-116">A: šifravimo susijusios strategijos pašalinimas nesukelia loginių diskų iššifravimo.</span><span class="sxs-lookup"><span data-stu-id="ab716-116">A: Removal of encryption related policy does NOT result in decryption of the drives which were configured.</span></span>




<span data-ttu-id="ab716-117">K: Kodėl Intune atitikties strategija rodo, kad mano įrenginys neturi "BitLocker" įjungtas, bet jis yra?</span><span class="sxs-lookup"><span data-stu-id="ab716-117">Q: Why does intune Compliance policy show that my device does not have "Bitlocker Enabled" but it is?</span></span>

<span data-ttu-id="ab716-118">A: "BitLocker" įgalintas parametras Intune atitikties strategijoje naudoja "Windows" įrenginio sveikatos patvirtinimo (DHA) klientą.</span><span class="sxs-lookup"><span data-stu-id="ab716-118">A: The "Bitlocker enabled" setting in intune compliance policy utilizes the Windows Device Health Attestation  (DHA) client.</span></span> <span data-ttu-id="ab716-119">Šis klientas tik matuoja įrenginio būseną įkrovimo metu.</span><span class="sxs-lookup"><span data-stu-id="ab716-119">This client only measures device state at boot time.</span></span> <span data-ttu-id="ab716-120">Taigi, jei įrenginys nebuvo paleistas, nes "BitLocker" šifravimas buvo užbaigtas, DHA kliento tarnyba nepateiks "BitLocker" kaip aktyvaus.</span><span class="sxs-lookup"><span data-stu-id="ab716-120">So if a device has not been rebooted since bitlocker encryption was completed the DHA client service will not report bitlocker as being active.</span></span>