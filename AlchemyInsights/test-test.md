---
title: Trūksta SharePoint Online terminas parduotuvė sąlygos
ms.author: pebaum
author: pebaum
ms.date: 10/30/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1243"
- "5200021"
ms.openlocfilehash: 28913b8e57e39d51e8957b7408c19337a119c589
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 12/15/2019
ms.locfileid: "40053521"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a><span data-ttu-id="35c0e-102">"BitLocker" šifravimo įgalinimas naudojant "Intune"</span><span class="sxs-lookup"><span data-stu-id="35c0e-102">Enabling Bitlocker Encryption with Intune</span></span>

<span data-ttu-id="35c0e-103">Intune galinio punkto apsaugos politika gali būti naudojama konfigūruoti Boitlocker šifravimo parametrus Windows įrenginių, kaip aprašyta: Windows10 (ir vėliau) parametrai apsaugoti įrenginius naudojant Intune</span><span class="sxs-lookup"><span data-stu-id="35c0e-103">Intune Endpoint Protection Policy can be used to configure Boitlocker encryption settings for Windows devices as described in : Windows10 (and later) settings to protect devices using Intune</span></span>

<span data-ttu-id="35c0e-104">Turėtumėte žinoti, kad daugelis naujesnių įrenginių, kuriuose veikia "Windows 10" palaiko automatinį "BitLocker" šifravimą, kuris suaktyvinamas netaikant MDM strategijos.</span><span class="sxs-lookup"><span data-stu-id="35c0e-104">You should be aware that many newer devices running Windows 10 support automatic bitlocker encryption which is triggered without the application of MDM policy.</span></span> <span data-ttu-id="35c0e-105">Tai gali paveikti strategijos taikymą, jei sukonfigūruoti ne numatytieji parametrai.</span><span class="sxs-lookup"><span data-stu-id="35c0e-105">This may impact application of policy if non default settings are configured.</span></span> <span data-ttu-id="35c0e-106">Daugiau informacijos rasite DUK.</span><span class="sxs-lookup"><span data-stu-id="35c0e-106">See FAQ for more detail.</span></span>


<span data-ttu-id="35c0e-107">DUK  klausimas: kokie "Windows" palaikymo įrenginių šifravimo leidimai naudojami naudojant galinio punkto apsaugos strategiją?</span><span class="sxs-lookup"><span data-stu-id="35c0e-107">FAQ  Q: Which editions of Windows support device encryption using the Endpoint Protection Policy?</span></span>
<span data-ttu-id="35c0e-108"> A: Intune galinio punkto apsaugos strategijos parametrai yra įgyvendinami naudojant BitLocker CSP.</span><span class="sxs-lookup"><span data-stu-id="35c0e-108"> A: The settings in Intune Endpoint Protection Policy  are implemented using the Bitlocker CSP.</span></span><span data-ttu-id="35c0e-109">Ne visi leidimai, nei komponavimo versijos "Windows" palaiko BitLocker CSP. 
     </span><span class="sxs-lookup"><span data-stu-id="35c0e-109">  Not all editions nor builds of Windows support the Bitlocker CSP. 
     </span></span> <span data-ttu-id="35c0e-110">Šiuo metu "Windows" leidimai: įmonė; Švietimas, Mobile, Mobile Enterprise ir Professional (nuo statyti 1809 ir vėliau) yra remiami.</span><span class="sxs-lookup"><span data-stu-id="35c0e-110">At this time Windows Editions: Enterprise; Education, Mobile, Mobile Enterprise and Professional (from build 1809 onwards) are supported.</span></span>




<span data-ttu-id="35c0e-111">Q: Jei įrenginys jau yra užšifruotas su "BitLocker" naudojant OS numatytuosius parametrus šifravimo metodas ir šifro stiprumas (XTS-AES-128) bus taikyti politiką su skirtingais parametrais automatiškai sukelti iš naujo šifravimo disko su naujais parametrais?</span><span class="sxs-lookup"><span data-stu-id="35c0e-111">Q: If a device is already encrypted with Bitlocker using the OS default settings for encryption method and cipher strength (XTS-AES-128)  will applying a policy with different settings automatically trigger re-encryption of the drive with the new settings?</span></span>

<span data-ttu-id="35c0e-112">A: ne.</span><span class="sxs-lookup"><span data-stu-id="35c0e-112">A: No.</span></span> <span data-ttu-id="35c0e-113">Norint taikyti naują šifro parametrus, pirmiausia turi būti iššifruotas diskas.</span><span class="sxs-lookup"><span data-stu-id="35c0e-113">In order to apply the new cipher settings the drive must first be decrypted.</span></span>

<span data-ttu-id="35c0e-114">Pastaba įrenginiuose, kurie įtraukti į AutoPilot automatinio šifravimo, kad atsirastų per OOBE nėra paleidžiamas kol Intune strategija yra vertinama, kuri leidžia strategijos parametrus, kurie turi būti naudojami vietoj OS numatytosios</span><span class="sxs-lookup"><span data-stu-id="35c0e-114">Note For devices being enrolled with Autopilot the automatic encryption that would occur during OOBE is not triggered until Intune policy is evaluated which allows the policy based settings to be used in place of the OS defaults</span></span>




<span data-ttu-id="35c0e-115">Q Jei prietaisas yra užšifruotas dėl Intune politikos taikymo bus iššifruoti, kai ši politika yra pašalinama?</span><span class="sxs-lookup"><span data-stu-id="35c0e-115">Q If a device is encrypted as a result of the  application of Intune policy will it be decrypted when that policy is removed?</span></span>

<span data-ttu-id="35c0e-116">A: pašalinus šifravimo susijusios politikos ne rezultatas iššifravimas diskus, kurie buvo sukonfigūruotas.</span><span class="sxs-lookup"><span data-stu-id="35c0e-116">A: Removal of encryption related policy does NOT result in decryption of the drives which were configured.</span></span>




<span data-ttu-id="35c0e-117">Klausimas: Kodėl Intune atitikties strategija rodo, kad mano įrenginys neturi "BitLocker įjungta", bet ji yra?</span><span class="sxs-lookup"><span data-stu-id="35c0e-117">Q: Why does intune Compliance policy show that my device does not have "Bitlocker Enabled" but it is?</span></span>

<span data-ttu-id="35c0e-118">A: "BitLocker" įjungtas "parametras Intune atitikties strategijos naudoja Windows įrenginio sveikatos patvirtinimo (DHA) klientas.</span><span class="sxs-lookup"><span data-stu-id="35c0e-118">A: The "Bitlocker enabled" setting in intune compliance policy utilizes the Windows Device Health Attestation  (DHA) client.</span></span> <span data-ttu-id="35c0e-119">Šis klientas tik priemonės prietaiso būseną įkrovos metu.</span><span class="sxs-lookup"><span data-stu-id="35c0e-119">This client only measures device state at boot time.</span></span> <span data-ttu-id="35c0e-120">Taigi, jei įrenginys buvo paleistas iš naujo, nes "BitLocker" šifravimas buvo baigtas DHA klientų aptarnavimo nepateiks "BitLocker" kaip aktyvus.</span><span class="sxs-lookup"><span data-stu-id="35c0e-120">So if a device has not been rebooted since bitlocker encryption was completed the DHA client service will not report bitlocker as being active.</span></span>