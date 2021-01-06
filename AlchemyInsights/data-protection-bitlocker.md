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
ms.openlocfilehash: 0b305931a7279d8f1085c411cc9b47c991e1ee44
ms.sourcegitcommit: 9c4b4853ff53f21c0177d48821846070bb00637c
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 01/06/2021
ms.locfileid: "49768825"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a><span data-ttu-id="c2a1b-102">"BitLocker" šifravimo su "Intune" įgalinimas</span><span class="sxs-lookup"><span data-stu-id="c2a1b-102">Enabling Bitlocker encryption with Intune</span></span>

 <span data-ttu-id="c2a1b-103">"Intune Endpoint Protection" strategiją galima naudoti konfigūruojant "BitLocker" šifravimo parametrus "Windows" įrenginiuose.</span><span class="sxs-lookup"><span data-stu-id="c2a1b-103">Intune Endpoint Protection Policy can be used to configure Bitlocker encryption settings for Windows devices.</span></span> <span data-ttu-id="c2a1b-104">Daugiau informacijos rasite ["Windows 10" (ir vėlesnės versijos) parametruose, kad apsaugotumėte įrenginius naudodami Intune](https://docs.microsoft.com/intune/endpoint-protection-windows-10#windows-encryption).</span><span class="sxs-lookup"><span data-stu-id="c2a1b-104">For more information, see [Windows 10 (and later) settings to protect devices using Intune](https://docs.microsoft.com/intune/endpoint-protection-windows-10#windows-encryption).</span></span>
 
<span data-ttu-id="c2a1b-105">Turėtumėte žinoti, kad daugelis naujesnių įrenginių, kuriuose veikia "Windows 10", palaiko automatinį "BitLocker" šifravimą, kuris paleidžiamas nenaudojant MDM strategijos.</span><span class="sxs-lookup"><span data-stu-id="c2a1b-105">You should be aware that many newer devices running Windows 10 support automatic Bitlocker encryption, which is triggered without the application of MDM policy.</span></span> <span data-ttu-id="c2a1b-106">Tai gali turėti įtakos strategijos taikymui, jei nenumatytieji parametrai yra sukonfigūruoti.</span><span class="sxs-lookup"><span data-stu-id="c2a1b-106">This may impact application of policy if non-default settings are configured.</span></span> <span data-ttu-id="c2a1b-107">Daugiau informacijos rasite toliau pateiktuose DUK.</span><span class="sxs-lookup"><span data-stu-id="c2a1b-107">See the following FAQ for more detail.</span></span>
 
<span data-ttu-id="c2a1b-108">Informacijos apie "BitLocker" problemų diagnostiką ieškokite ["BitLocker" strategijų trikčių diagnostika "Microsoft Intune"](https://docs.microsoft.com/intune/protect/troubleshoot-bitlocker-policies).</span><span class="sxs-lookup"><span data-stu-id="c2a1b-108">For information about troubleshooting bitlocker issues, see [Troubleshoot BitLocker policies in Microsoft Intune](https://docs.microsoft.com/intune/protect/troubleshoot-bitlocker-policies).</span></span>
 
 
<span data-ttu-id="c2a1b-109">**DUK**</span><span class="sxs-lookup"><span data-stu-id="c2a1b-109">**FAQ**</span></span>

<span data-ttu-id="c2a1b-110">K: kokių "Windows" palaikymo įrenginių šifravimo leidimų naudojant galinio punkto apsaugos strategiją?</span><span class="sxs-lookup"><span data-stu-id="c2a1b-110">Q: Which editions of Windows support device encryption using the Endpoint Protection Policy?</span></span><br>
<span data-ttu-id="c2a1b-111">A: "Intune Endpoint Protection" strategijos parametrai vykdomi naudojant ["BitLocker" CSP](https://docs.microsoft.com/windows/client-management/mdm/bitlocker-csp).</span><span class="sxs-lookup"><span data-stu-id="c2a1b-111">A: The settings in Intune Endpoint Protection Policy are implemented using the [Bitlocker CSP](https://docs.microsoft.com/windows/client-management/mdm/bitlocker-csp).</span></span> <span data-ttu-id="c2a1b-112">Ne visi "Windows" leidimai arba komponavimo versijos palaiko "BitLocker" CSP.</span><span class="sxs-lookup"><span data-stu-id="c2a1b-112">Not all editions or builds of Windows support the Bitlocker CSP.</span></span> <br><br>

<span data-ttu-id="c2a1b-113">K: kaip "BitLocker" galima įjungti įrenginiuose be galutinio vartotojo veiksmo?</span><span class="sxs-lookup"><span data-stu-id="c2a1b-113">Q: How can Bitlocker be enabled on devices without requiring end user interaction?</span></span><br>
<span data-ttu-id="c2a1b-114">A: tol, kol bus įvykdytos būtinos prielaidos, galima įjungti "BitLocker" tylųjį šifravimą per Intune.</span><span class="sxs-lookup"><span data-stu-id="c2a1b-114">A: So long as the necessary pre-requisites are met it is possible to enable Bitlocker "Silent Encryption" through Intune.</span></span> <span data-ttu-id="c2a1b-115">Peržiūrėkite išsamią informaciją apie įrenginio reikalavimus ir pavyzdinius strategijos parametrus, kad būtų įgalintas tylus šifravimas šiame doc: [tyliai įjunkite "BitLocker" šifravimą](https://docs.microsoft.com/mem/intune/protect/encrypt-devices#silently-enable-bitlocker-on-devices).</span><span class="sxs-lookup"><span data-stu-id="c2a1b-115">See the details of the device requirements and example policy settings to enable silent encryption in the following doc: [Silently Enable Bitlocker Encryption](https://docs.microsoft.com/mem/intune/protect/encrypt-devices#silently-enable-bitlocker-on-devices).</span></span> <br><br>

<span data-ttu-id="c2a1b-116">K: Jei įrenginys jau užšifruotas naudojant "BitLocker", kai "BitLocker" yra šifravimo metodo ir šifro stiprumo parametrai (XTS-AES – 128), pritaikys strategiją su skirtingais parametrais, automatiškai suaktyvins disko, kuriame yra nauji parametrai, šifravimą?</span><span class="sxs-lookup"><span data-stu-id="c2a1b-116">Q: If a device is already encrypted with Bitlocker using the OS default settings for encryption method and cipher strength (XTS-AES-128), will applying a policy with different settings automatically trigger re-encryption of the drive with the new settings?</span></span><br>
<span data-ttu-id="c2a1b-117">A.: Ne.</span><span class="sxs-lookup"><span data-stu-id="c2a1b-117">A: No.</span></span> <span data-ttu-id="c2a1b-118">Norint taikyti naujus šifro parametrus, pirmiausia reikia iššifruoti loginį diską.</span><span class="sxs-lookup"><span data-stu-id="c2a1b-118">To apply the new cipher settings, the drive must first be decrypted.</span></span><br><br>
<span data-ttu-id="c2a1b-119">**Pastaba:** "Autopilot" registruotam įrenginiams Automatinis šifravimas, įvykęs OOBE metu, nėra paleidžiamas, kol bus įvertinta Intune strategija, kuri leidžia naudoti strategijos parametrus, naudojamus vietoj OS numatytųjų reikšmių.</span><span class="sxs-lookup"><span data-stu-id="c2a1b-119">**Note:** For devices being enrolled with Autopilot, the automatic encryption that would occur during OOBE is not triggered until Intune policy is evaluated, which allows the policy-based settings to be used in place of the OS defaults.</span></span>
 
<span data-ttu-id="c2a1b-120">K: Jei įrenginys užšifruotas kaip "Intune" strategijos taikymas, jis bus iššifruotas pašalinus šią strategiją?</span><span class="sxs-lookup"><span data-stu-id="c2a1b-120">Q: If a device is encrypted as a result of the  application of Intune policy, will it be decrypted when that policy is removed?</span></span><br>
<span data-ttu-id="c2a1b-121">A: su šifravimu susijusios strategijos pašalinimas nesukelia loginių diskų iššifravimo.</span><span class="sxs-lookup"><span data-stu-id="c2a1b-121">A: Removal of encryption-related policy does NOT result in decryption of the drives that were configured.</span></span>
 
<span data-ttu-id="c2a1b-122">K: Kodėl Intune atitikties strategija rodo, kad mano įrenginyje nėra įgalintas "BitLocker", net jei jis yra?</span><span class="sxs-lookup"><span data-stu-id="c2a1b-122">Q: Why does Intune Compliance Policy show that my device does not have Bitlocker enabled, even though it is?</span></span><br>
<span data-ttu-id="c2a1b-123">A: "BitLocker" įgalintas parametras Intune atitikties strategijoje naudoja "Windows" įrenginio sveikatos patvirtinimo (DHA) klientą.</span><span class="sxs-lookup"><span data-stu-id="c2a1b-123">A: The "Bitlocker enabled" setting in the Intune Compliance Policy utilizes the Windows Device Health Attestation  (DHA) client.</span></span> <span data-ttu-id="c2a1b-124">Šis klientas tik matuoja įrenginio būseną įkrovimo metu.</span><span class="sxs-lookup"><span data-stu-id="c2a1b-124">This client only measures device state at boot time.</span></span> <span data-ttu-id="c2a1b-125">Taigi, jei įrenginys nebuvo paleistas, nes "BitLocker" šifravimas buvo užbaigtas, DHA kliento tarnyba nepateiks "BitLocker" kaip aktyvaus.</span><span class="sxs-lookup"><span data-stu-id="c2a1b-125">So if a device has not been rebooted since Bitlocker encryption was completed, the DHA client service will not report Bitlocker as being active.</span></span>
 
 