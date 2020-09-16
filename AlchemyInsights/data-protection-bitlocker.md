---
title: "\"DataProtection\" – \"BitLocker\""
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1802"
- "9000220"
ms.openlocfilehash: ab28162fcdf0a37060be3bdf15a78aceca7a48b1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47731247"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a><span data-ttu-id="a78ba-102">"BitLocker" šifravimo su "Intune" įgalinimas</span><span class="sxs-lookup"><span data-stu-id="a78ba-102">Enabling Bitlocker encryption with Intune</span></span>

 <span data-ttu-id="a78ba-103">"Intune Endpoint Protection" strategiją galima naudoti konfigūruojant "BitLocker" šifravimo parametrus "Windows" įrenginiuose.</span><span class="sxs-lookup"><span data-stu-id="a78ba-103">Intune Endpoint Protection Policy can be used to configure Bitlocker encryption settings for Windows devices.</span></span> <span data-ttu-id="a78ba-104">Daugiau informacijos rasite ["Windows 10" (ir vėlesnės versijos) parametruose, kad apsaugotumėte įrenginius naudodami Intune](https://docs.microsoft.com/intune/endpoint-protection-windows-10#windows-encryption).</span><span class="sxs-lookup"><span data-stu-id="a78ba-104">For more information, see [Windows 10 (and later) settings to protect devices using Intune](https://docs.microsoft.com/intune/endpoint-protection-windows-10#windows-encryption).</span></span>
 
<span data-ttu-id="a78ba-105">Turėtumėte žinoti, kad daugelis naujesnių įrenginių, kuriuose veikia "Windows 10", palaiko automatinį "BitLocker" šifravimą, kuris paleidžiamas nenaudojant MDM strategijos.</span><span class="sxs-lookup"><span data-stu-id="a78ba-105">You should be aware that many newer devices running Windows 10 support automatic Bitlocker encryption, which is triggered without the application of MDM policy.</span></span> <span data-ttu-id="a78ba-106">Tai gali turėti įtakos strategijos taikymui, jei nenumatytieji parametrai yra sukonfigūruoti.</span><span class="sxs-lookup"><span data-stu-id="a78ba-106">This may impact application of policy if non-default settings are configured.</span></span> <span data-ttu-id="a78ba-107">Daugiau informacijos rasite toliau pateiktuose DUK.</span><span class="sxs-lookup"><span data-stu-id="a78ba-107">See the following FAQ for more detail.</span></span>
 
<span data-ttu-id="a78ba-108">Informacijos apie "BitLocker" problemų diagnostiką ieškokite ["BitLocker" strategijų trikčių diagnostika "Microsoft Intune"](https://docs.microsoft.com/intune/protect/troubleshoot-bitlocker-policies).</span><span class="sxs-lookup"><span data-stu-id="a78ba-108">For information about troubleshooting bitlocker issues, see [Troubleshoot BitLocker policies in Microsoft Intune](https://docs.microsoft.com/intune/protect/troubleshoot-bitlocker-policies).</span></span>
 
 
<span data-ttu-id="a78ba-109">**DUK**</span><span class="sxs-lookup"><span data-stu-id="a78ba-109">**FAQ**</span></span>

 <span data-ttu-id="a78ba-110">K: kokių "Windows" palaikymo įrenginių šifravimo leidimų naudojant galinio punkto apsaugos strategiją?</span><span class="sxs-lookup"><span data-stu-id="a78ba-110">Q: Which editions of Windows support device encryption using the Endpoint Protection Policy?</span></span><br>
 <span data-ttu-id="a78ba-111">A: "Intune Endpoint Protection" strategijos parametrai vykdomi naudojant ["BitLocker" CSP](https://docs.microsoft.com/windows/client-management/mdm/bitlocker-csp).</span><span class="sxs-lookup"><span data-stu-id="a78ba-111">A: The settings in Intune Endpoint Protection Policy  are implemented using the [Bitlocker CSP](https://docs.microsoft.com/windows/client-management/mdm/bitlocker-csp).</span></span> <span data-ttu-id="a78ba-112">Ne visi "Windows" leidimai arba komponavimo versijos palaiko "BitLocker" CSP.</span><span class="sxs-lookup"><span data-stu-id="a78ba-112">Not all editions or builds of Windows support the Bitlocker CSP.</span></span> <br><br>
      <span data-ttu-id="a78ba-113">Šiuo metu palaikomi šie "Windows" leidimai: "Enterprise", "Education", mobilusis, mobiliųjų įrenginių įmonė ir profesionalai (1809 Komponavimo versija ir vėlesnė versija).</span><span class="sxs-lookup"><span data-stu-id="a78ba-113">At this time, the following Windows editions are supported: Enterprise, Education, Mobile, Mobile Enterprise, and Professional (build 1809 and later).</span></span>
 
<span data-ttu-id="a78ba-114">K: Jei įrenginys jau užšifruotas naudojant "BitLocker", kai "BitLocker" yra šifravimo metodo ir šifro stiprumo parametrai (XTS-AES – 128), pritaikys strategiją su skirtingais parametrais, automatiškai suaktyvins disko, kuriame yra nauji parametrai, šifravimą?</span><span class="sxs-lookup"><span data-stu-id="a78ba-114">Q: If a device is already encrypted with Bitlocker using the OS default settings for encryption method and cipher strength (XTS-AES-128), will applying a policy with different settings automatically trigger re-encryption of the drive with the new settings?</span></span><br>
<span data-ttu-id="a78ba-115">A.: Ne.</span><span class="sxs-lookup"><span data-stu-id="a78ba-115">A: No.</span></span> <span data-ttu-id="a78ba-116">Norint taikyti naujus šifro parametrus, pirmiausia reikia iššifruoti loginį diską.</span><span class="sxs-lookup"><span data-stu-id="a78ba-116">To apply the new cipher settings, the drive must first be decrypted.</span></span><br><br>
<span data-ttu-id="a78ba-117">**Pastaba:** "Autopilot" registruotam įrenginiams Automatinis šifravimas, įvykęs OOBE metu, nėra paleidžiamas, kol bus įvertinta Intune strategija, kuri leidžia naudoti strategijos parametrus, naudojamus vietoj OS numatytųjų reikšmių.</span><span class="sxs-lookup"><span data-stu-id="a78ba-117">**Note:** For devices being enrolled with Autopilot, the automatic encryption that would occur during OOBE is not triggered until Intune policy is evaluated, which allows the policy-based settings to be used in place of the OS defaults.</span></span>
 
<span data-ttu-id="a78ba-118">K: Jei įrenginys užšifruotas kaip "Intune" strategijos taikymas, jis bus iššifruotas pašalinus šią strategiją?</span><span class="sxs-lookup"><span data-stu-id="a78ba-118">Q: If a device is encrypted as a result of the  application of Intune policy, will it be decrypted when that policy is removed?</span></span><br>
<span data-ttu-id="a78ba-119">A: su šifravimu susijusios strategijos pašalinimas nesukelia loginių diskų iššifravimo.</span><span class="sxs-lookup"><span data-stu-id="a78ba-119">A: Removal of encryption-related policy does NOT result in decryption of the drives that were configured.</span></span>
 
<span data-ttu-id="a78ba-120">K: Kodėl Intune atitikties strategija rodo, kad mano įrenginyje nėra įgalintas "BitLocker", net jei jis yra?</span><span class="sxs-lookup"><span data-stu-id="a78ba-120">Q: Why does Intune Compliance Policy show that my device does not have Bitlocker enabled, even though it is?</span></span><br>
<span data-ttu-id="a78ba-121">A: "BitLocker" įgalintas parametras Intune atitikties strategijoje naudoja "Windows" įrenginio sveikatos patvirtinimo (DHA) klientą.</span><span class="sxs-lookup"><span data-stu-id="a78ba-121">A: The "Bitlocker enabled" setting in the Intune Compliance Policy utilizes the Windows Device Health Attestation  (DHA) client.</span></span> <span data-ttu-id="a78ba-122">Šis klientas tik matuoja įrenginio būseną įkrovimo metu.</span><span class="sxs-lookup"><span data-stu-id="a78ba-122">This client only measures device state at boot time.</span></span> <span data-ttu-id="a78ba-123">Taigi, jei įrenginys nebuvo paleistas, nes "BitLocker" šifravimas buvo užbaigtas, DHA kliento tarnyba nepateiks "BitLocker" kaip aktyvaus.</span><span class="sxs-lookup"><span data-stu-id="a78ba-123">So if a device has not been rebooted since Bitlocker encryption was completed, the DHA client service will not report Bitlocker as being active.</span></span>
 
 