---
title: DataProtection-"BitLocker"
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1802"
- "9000220"
ms.openlocfilehash: c23a2a2bde240900119382a9c1185a6e02520149
ms.sourcegitcommit: 123e9fe46e99719dd271e75a66555861e968f4a2
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 12/30/2019
ms.locfileid: "40908717"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a><span data-ttu-id="4b811-102">"BitLocker" šifravimo įgalinimas naudojant "Intune"</span><span class="sxs-lookup"><span data-stu-id="4b811-102">Enabling Bitlocker encryption with Intune</span></span>

 <span data-ttu-id="4b811-103">Intune Endpoint Protection politika gali būti naudojama konfigūruoti BitLocker šifravimo parametrus Windows įrenginiams.</span><span class="sxs-lookup"><span data-stu-id="4b811-103">Intune Endpoint Protection Policy can be used to configure Bitlocker encryption settings for Windows devices.</span></span> <span data-ttu-id="4b811-104">Daugiau informacijos rasite ["Windows 10" (ir naujesniuose) parametruose, kad apsaugotume įrenginius naudojant "Intune"](https://docs.microsoft.com/intune/endpoint-protection-windows-10#windows-encryption).</span><span class="sxs-lookup"><span data-stu-id="4b811-104">For more information, see [Windows 10 (and later) settings to protect devices using Intune](https://docs.microsoft.com/intune/endpoint-protection-windows-10#windows-encryption).</span></span>
 
<span data-ttu-id="4b811-105">Turėtumėte žinoti, kad daug naujesnių įrenginių, kuriuose veikia "Windows 10", palaiko automatinį "BitLocker" šifravimą, kuris paleidžiamas netaikant MDM strategijos.</span><span class="sxs-lookup"><span data-stu-id="4b811-105">You should be aware that many newer devices running Windows 10 support automatic Bitlocker encryption, which is triggered without the application of MDM policy.</span></span> <span data-ttu-id="4b811-106">Tai gali paveikti strategijos taikymą, jei sukonfigūruoti ne numatytieji parametrai.</span><span class="sxs-lookup"><span data-stu-id="4b811-106">This may impact application of policy if non-default settings are configured.</span></span> <span data-ttu-id="4b811-107">Daugiau informacijos rasite toliau pateiktuose DUK.</span><span class="sxs-lookup"><span data-stu-id="4b811-107">See the following FAQ for more detail.</span></span>
 
<span data-ttu-id="4b811-108">Informacijos apie "BitLocker" trikčių šalinimą rasite ["Microsoft Intune" "BitLocker" strategijos trikčių diagnostika](https://docs.microsoft.com/intune/protect/troubleshoot-bitlocker-policies).</span><span class="sxs-lookup"><span data-stu-id="4b811-108">For information about troubleshooting bitlocker issues, see [Troubleshoot BitLocker policies in Microsoft Intune](https://docs.microsoft.com/intune/protect/troubleshoot-bitlocker-policies).</span></span>
 
 
<span data-ttu-id="4b811-109">**Duk**</span><span class="sxs-lookup"><span data-stu-id="4b811-109">**FAQ**</span></span>

 <span data-ttu-id="4b811-110">Klausimas: kokie leidimai Windows palaikymo įrenginių šifravimo naudojant galinio punkto apsaugos strategijos?</span><span class="sxs-lookup"><span data-stu-id="4b811-110">Q: Which editions of Windows support device encryption using the Endpoint Protection Policy?</span></span><br>
 <span data-ttu-id="4b811-111">A: Intune galinio punkto apsaugos strategijos parametrai yra įgyvendinami naudojant " [BitLocker" CSP](https://docs.microsoft.com/windows/client-management/mdm/bitlocker-csp).</span><span class="sxs-lookup"><span data-stu-id="4b811-111">A: The settings in Intune Endpoint Protection Policy  are implemented using the [Bitlocker CSP](https://docs.microsoft.com/windows/client-management/mdm/bitlocker-csp).</span></span> <span data-ttu-id="4b811-112">Ne visi leidimai ar komponavimo versijos Windows palaiko BitLocker CSP.</span><span class="sxs-lookup"><span data-stu-id="4b811-112">Not all editions or builds of Windows support the Bitlocker CSP.</span></span> <br><br>
      <span data-ttu-id="4b811-113">Šiuo metu palaikomi šie Windows leidimai: Enterprise, Education, Mobile, Mobile Enterprise ir Professional (statyti 1809 ir vėliau).</span><span class="sxs-lookup"><span data-stu-id="4b811-113">At this time, the following Windows editions are supported: Enterprise, Education, Mobile, Mobile Enterprise, and Professional (build 1809 and later).</span></span>
 
<span data-ttu-id="4b811-114">Q: Jei įrenginys jau yra užšifruotas naudojant "BitLocker" naudodami numatytuosius OS parametrus šifravimo metodui ir šifro patvarumui (XTS-AES-128), taikant strategiją su skirtingais parametrais, automatiškai suaktyvins disko šifravimą su naujais parametrais?</span><span class="sxs-lookup"><span data-stu-id="4b811-114">Q: If a device is already encrypted with Bitlocker using the OS default settings for encryption method and cipher strength (XTS-AES-128), will applying a policy with different settings automatically trigger re-encryption of the drive with the new settings?</span></span><br>
<span data-ttu-id="4b811-115">A: ne.</span><span class="sxs-lookup"><span data-stu-id="4b811-115">A: No.</span></span> <span data-ttu-id="4b811-116">Norint taikyti naują šifro parametrus, diskas pirmiausia turi būti iššifruotas.</span><span class="sxs-lookup"><span data-stu-id="4b811-116">To apply the new cipher settings, the drive must first be decrypted.</span></span><br><br>
<span data-ttu-id="4b811-117">**Pastaba:** Prietaisų, kurie mokosi su Autopilotas, automatinio šifravimo, kad atsirastų OOBE metu nėra paleidžiamas kol Intune strategija yra vertinama, kuri leidžia strategijos parametrai turi būti naudojami vietoj OS numatytąsias reikšmes.</span><span class="sxs-lookup"><span data-stu-id="4b811-117">**Note:** For devices being enrolled with Autopilot, the automatic encryption that would occur during OOBE is not triggered until Intune policy is evaluated, which allows the policy-based settings to be used in place of the OS defaults.</span></span>
 
<span data-ttu-id="4b811-118">Q: Jei įrenginys yra užšifruotas dėl Intune strategijos taikymo, ar jis bus iššifruoti, kai ši politika bus pašalinta?</span><span class="sxs-lookup"><span data-stu-id="4b811-118">Q: If a device is encrypted as a result of the  application of Intune policy, will it be decrypted when that policy is removed?</span></span><br>
<span data-ttu-id="4b811-119">A: pašalinus šifravimo susijusios politikos ne rezultatas iššifravimas diskus, kurie buvo sukonfigūruotas.</span><span class="sxs-lookup"><span data-stu-id="4b811-119">A: Removal of encryption-related policy does NOT result in decryption of the drives that were configured.</span></span>
 
<span data-ttu-id="4b811-120">Klausimas: Kodėl Intune atitikties politika rodo, kad mano įrenginys nėra įgalintas "BitLocker", nors ji yra?</span><span class="sxs-lookup"><span data-stu-id="4b811-120">Q: Why does Intune Compliance Policy show that my device does not have Bitlocker enabled, even though it is?</span></span><br>
<span data-ttu-id="4b811-121">A: "BitLocker" įjungtas "nustatymas Intune atitikties strategijos naudoja" Windows "įrenginio sveikatos patvirtinimo (DHA) kliento.</span><span class="sxs-lookup"><span data-stu-id="4b811-121">A: The "Bitlocker enabled" setting in the Intune Compliance Policy utilizes the Windows Device Health Attestation  (DHA) client.</span></span> <span data-ttu-id="4b811-122">Šis klientas tik priemonės prietaiso būseną įkrovos metu.</span><span class="sxs-lookup"><span data-stu-id="4b811-122">This client only measures device state at boot time.</span></span> <span data-ttu-id="4b811-123">Taigi, jei įrenginys nebuvo paleistas, nes "BitLocker" šifravimas buvo baigtas, DHA kliento tarnyba nebus pranešti "BitLocker" kaip aktyvus.</span><span class="sxs-lookup"><span data-stu-id="4b811-123">So if a device has not been rebooted since Bitlocker encryption was completed, the DHA client service will not report Bitlocker as being active.</span></span>
 
 