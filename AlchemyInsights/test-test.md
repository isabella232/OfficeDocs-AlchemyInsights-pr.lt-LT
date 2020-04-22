---
title: "\"SharePoint Online\" terminų saugykloje trūksta sąlygų"
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1243"
- "5200021"
ms.openlocfilehash: 54ac2dbc1f45f88541c2338f3b55a777b4b57123
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 04/22/2020
ms.locfileid: "43766861"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a><span data-ttu-id="0bc05-102">"BitLocker" šifravimo įgalinimas naudojant "Intune"</span><span class="sxs-lookup"><span data-stu-id="0bc05-102">Enabling Bitlocker Encryption with Intune</span></span>

<span data-ttu-id="0bc05-103">Intune Endpoint Protection Policy gali būti naudojamas konfigūruoti Boitlocker šifravimo parametrus Windows įrenginių, kaip aprašyta: Windows10 (ir vėliau) parametrus apsaugoti įrenginius naudojant Intune</span><span class="sxs-lookup"><span data-stu-id="0bc05-103">Intune Endpoint Protection Policy can be used to configure Boitlocker encryption settings for Windows devices as described in : Windows10 (and later) settings to protect devices using Intune</span></span>

<span data-ttu-id="0bc05-104">Turėtumėte žinoti, kad daugelis naujesnių įrenginių, kuriuose veikia "Windows 10", palaiko automatinį "bitLocker" šifravimą, kuris paleidžiamas be MDM strategijos taikymo.</span><span class="sxs-lookup"><span data-stu-id="0bc05-104">You should be aware that many newer devices running Windows 10 support automatic bitlocker encryption which is triggered without the application of MDM policy.</span></span> <span data-ttu-id="0bc05-105">Tai gali turėti įtakos strategijos taikymui, jei nenumatytieji parametrai yra sukonfigūruoti.</span><span class="sxs-lookup"><span data-stu-id="0bc05-105">This may impact application of policy if non default settings are configured.</span></span> <span data-ttu-id="0bc05-106">Daugiau informacijos rasite DUK.</span><span class="sxs-lookup"><span data-stu-id="0bc05-106">See FAQ for more detail.</span></span>


<span data-ttu-id="0bc05-107">DUK  Q: Kurie "Windows" palaikymo įrenginių šifravimo leidimai naudojant galinio punkto apsaugos strategiją?</span><span class="sxs-lookup"><span data-stu-id="0bc05-107">FAQ  Q: Which editions of Windows support device encryption using the Endpoint Protection Policy?</span></span>
<span data-ttu-id="0bc05-108"> A: Intune Endpoint Protection strategijos parametrai yra įgyvendinami naudojant "BitLocker" CSP.</span><span class="sxs-lookup"><span data-stu-id="0bc05-108"> A: The settings in Intune Endpoint Protection Policy  are implemented using the Bitlocker CSP.</span></span><span data-ttu-id="0bc05-109">Ne visi "Windows" leidimai ir komponavimo versijos palaiko "BitLocker" CSP. 
     </span><span class="sxs-lookup"><span data-stu-id="0bc05-109">  Not all editions nor builds of Windows support the Bitlocker CSP. 
     </span></span> <span data-ttu-id="0bc05-110">Šiuo metu "Windows" leidimai: įmonė; "Education", "Mobile", "Mobile" ir "Professional" (nuo 1809 m. komponavimo versijos) yra remiamos.</span><span class="sxs-lookup"><span data-stu-id="0bc05-110">At this time Windows Editions: Enterprise; Education, Mobile, Mobile Enterprise and Professional (from build 1809 onwards) are supported.</span></span>




<span data-ttu-id="0bc05-111">Klausimas: Jei įrenginys jau užšifruotas su "BitLocker" naudojant OS numatytuosius parametrus šifravimo metodui ir šifravimo stiprumas (XTS-AES-128) taiks strategiją su skirtingais parametrais automatiškai sukelti pakartotinį disko šifravimą su naujais parametrais?</span><span class="sxs-lookup"><span data-stu-id="0bc05-111">Q: If a device is already encrypted with Bitlocker using the OS default settings for encryption method and cipher strength (XTS-AES-128)  will applying a policy with different settings automatically trigger re-encryption of the drive with the new settings?</span></span>

<span data-ttu-id="0bc05-112">Ats.: Ne.</span><span class="sxs-lookup"><span data-stu-id="0bc05-112">A: No.</span></span> <span data-ttu-id="0bc05-113">Norint taikyti naujus šifravimo parametrus, diskas pirmiausia turi būti iššifruotas.</span><span class="sxs-lookup"><span data-stu-id="0bc05-113">In order to apply the new cipher settings the drive must first be decrypted.</span></span>

<span data-ttu-id="0bc05-114">Pastaba Įrenginiams, įtrauktiems su autopilotu, automatinis šifravimas, kuris įvyktų OOBE metu, neįjungiamas, kol neįvertinama Intune strategija, kuri leidžia naudoti strategijos pagrindu pagrįstus parametrus vietoj os numatytųjų reikšmių</span><span class="sxs-lookup"><span data-stu-id="0bc05-114">Note For devices being enrolled with Autopilot the automatic encryption that would occur during OOBE is not triggered until Intune policy is evaluated which allows the policy based settings to be used in place of the OS defaults</span></span>




<span data-ttu-id="0bc05-115">K Jei įrenginys yra užšifruotas dėl Intune strategijos taikymo, ar jis bus iššifruotas, kai ši strategija bus pašalinta?</span><span class="sxs-lookup"><span data-stu-id="0bc05-115">Q If a device is encrypted as a result of the  application of Intune policy will it be decrypted when that policy is removed?</span></span>

<span data-ttu-id="0bc05-116">A: Šifravimo susijusios strategijos pašalinimas nesukelia sukonfigūruotidiskų iššifravimo.</span><span class="sxs-lookup"><span data-stu-id="0bc05-116">A: Removal of encryption related policy does NOT result in decryption of the drives which were configured.</span></span>




<span data-ttu-id="0bc05-117">K: Kodėl intune atitikties strategija rodo, kad mano įrenginyje nėra "BitLocker Įjungta", bet tai yra?</span><span class="sxs-lookup"><span data-stu-id="0bc05-117">Q: Why does intune Compliance policy show that my device does not have "Bitlocker Enabled" but it is?</span></span>

<span data-ttu-id="0bc05-118">A: "BitLocker įjungtas" parametras intune atitikties strategija naudoja Windows įrenginio sveikatos patvirtinimo (Dha) kliento.</span><span class="sxs-lookup"><span data-stu-id="0bc05-118">A: The "Bitlocker enabled" setting in intune compliance policy utilizes the Windows Device Health Attestation  (DHA) client.</span></span> <span data-ttu-id="0bc05-119">Šis klientas matuoja tik įrenginio būseną įkrovos metu.</span><span class="sxs-lookup"><span data-stu-id="0bc05-119">This client only measures device state at boot time.</span></span> <span data-ttu-id="0bc05-120">Taigi, jei įrenginys nebuvo paleistas iš naujo, nes "bitLocker" šifravimas buvo baigtas, Dha kliento tarnyba nepraneš apie "bitLocker" kaip aktyvų.</span><span class="sxs-lookup"><span data-stu-id="0bc05-120">So if a device has not been rebooted since bitlocker encryption was completed the DHA client service will not report bitlocker as being active.</span></span>