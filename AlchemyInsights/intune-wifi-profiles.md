---
title: "\"Intune\" \"Wi-Fi\" profiliai"
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1548"
- "9000076"
ms.openlocfilehash: e5e1007abadb8ddb30ca110d465131ec791e44b7
ms.sourcegitcommit: e90b918f02102cd9764881c2d8c914567c6b070e
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 07/29/2020
ms.locfileid: "46555314"
---
# <a name="intune-wi-fi-profiles"></a><span data-ttu-id="50b3a-102">"Intune" "Wi-Fi" profiliai</span><span class="sxs-lookup"><span data-stu-id="50b3a-102">Intune Wi-Fi profiles</span></span>

<span data-ttu-id="50b3a-103">Sėkmingas "Wi-Fi" ryšio diegimas MDM klientams priklauso nuo tinkamai įdiegto profilio, kuris atspindi įmonės "Wi-Fi" infrastruktūros reikalavimus.</span><span class="sxs-lookup"><span data-stu-id="50b3a-103">Successful implementation of Wi-Fi connectivity for MDM clients depends on a correctly deployed profile that reflects the requirements of the corporate Wi-Fi infrastructure.</span></span> <span data-ttu-id="50b3a-104">Norėdami peržiūrėti atitinkamus parametrus kliento platformose, kurį tiriate, žr.:</span><span class="sxs-lookup"><span data-stu-id="50b3a-104">To review the appropriate settings for the client platforms you are investigating, see:</span></span> 

[<span data-ttu-id="50b3a-105">"Wi-Fi" parametrų įtraukimas įrenginiams, kuriuose veikia "Android" programoje "Microsoft Intune"</span><span class="sxs-lookup"><span data-stu-id="50b3a-105">Add Wi-Fi settings for devices running Android in Microsoft Intune</span></span>](https://docs.microsoft.com/intune/wi-fi-settings-android)

[<span data-ttu-id="50b3a-106">"Wi-Fi" parametrų įtraukimas į "Android Enterprise" skirtus ir visiškai valdomus įrenginius programoje "Microsoft Intune"</span><span class="sxs-lookup"><span data-stu-id="50b3a-106">Add Wi-Fi settings for Android Enterprise dedicated and fully managed devices in Microsoft Intune</span></span>](https://docs.microsoft.com/intune/wi-fi-settings-android-enterprise)

[<span data-ttu-id="50b3a-107">"Wi-Fi" parametrų įtraukimas į "iOS" ir "iPadOS" įrenginius programoje "Microsoft Intune"</span><span class="sxs-lookup"><span data-stu-id="50b3a-107">Add Wi-Fi settings for iOS and iPadOS devices in Microsoft Intune</span></span>](https://docs.microsoft.com/intune/wi-fi-settings-ios)

[<span data-ttu-id="50b3a-108">"Wi-Fi" parametrų įtraukimas į "Windows 10" ir naujesnius įrenginius "Intune"</span><span class="sxs-lookup"><span data-stu-id="50b3a-108">Add Wi-Fi settings for Windows 10 and later devices in Intune</span></span>](https://docs.microsoft.com/intune/wi-fi-settings-windows)

[<span data-ttu-id="50b3a-109">"Wi-Fi" parametrų importavimas "Windows" įrenginiams "Intune"</span><span class="sxs-lookup"><span data-stu-id="50b3a-109">Import Wi-Fi settings for Windows devices in Intune</span></span>](https://docs.microsoft.com/intune/wi-fi-settings-import-windows-8-1)

<span data-ttu-id="50b3a-110">**Dažniausiai pasitaikančios problemos**</span><span class="sxs-lookup"><span data-stu-id="50b3a-110">**Common Issues**</span></span>

<span data-ttu-id="50b3a-111">**Diegiau "Wi-Fi" profilį, kuris priklauso nuo įdiegto sertifikato, nurodyto "Wi-Fi" profilyje. Tačiau konfigūracijos profiliai rodo klaidos būseną.**</span><span class="sxs-lookup"><span data-stu-id="50b3a-111">**I'm deploying a Wi-Fi profile that is dependent on a deployed certificate specified in the Wi-Fi profile. However, the configuration profiles are showing an error status.**</span></span>

<span data-ttu-id="50b3a-112">Patikrinkite, ar jūsų įrenginys gavo sertifikatą.</span><span class="sxs-lookup"><span data-stu-id="50b3a-112">Check that your device received the certificate.</span></span>

1. <span data-ttu-id="50b3a-113">Intune eikite į **Visi įrenginiai** ir pasirinkite įrenginį > **Įrenginio konfigūraciją**.</span><span class="sxs-lookup"><span data-stu-id="50b3a-113">In Intune, go to **All Devices** and select the device > **Device configuration**.</span></span>

2. <span data-ttu-id="50b3a-114">Patikrinkite, ar visi numatyti profiliai yra išvardyti ir sėkmingai.</span><span class="sxs-lookup"><span data-stu-id="50b3a-114">Check that all expected profiles are listed and in a successful state.</span></span>

3. <span data-ttu-id="50b3a-115">Jei turite tarpinių sertifikatų "Android" profilyje, įsitikinkite, kad jie įdiegti "Android" įrenginiuose.</span><span class="sxs-lookup"><span data-stu-id="50b3a-115">For an Android profile, if you have intermediate certificates in your certificate chain, make sure they are deployed to Android devices.</span></span>

    <span data-ttu-id="50b3a-116">Norėdami patikrinti sertifikato būseną, eikite į **Įrenginio konfigūracijos**  >  **profiliai**  >  **"Android" tarpinių CA**  >  **ypatybės**  >  **Patikimas sertifikatas**.</span><span class="sxs-lookup"><span data-stu-id="50b3a-116">To check the certificate status, go to **Device configuration** > **Profiles** > **Android intermediate CA** > **Properties** > **Trusted Certificate**.</span></span>

<span data-ttu-id="50b3a-117">Jei vis tiek matote klaidų, peržiūrėkite procedūras ir trikčių šalinimo skyrius.</span><span class="sxs-lookup"><span data-stu-id="50b3a-117">If you continue to see errors, review the procedures and troubleshooting sections.</span></span> <span data-ttu-id="50b3a-118">Daugiau informacijos ieškokite [SCEP sertifikatų profilių trikčių diagnostika naudojant "Microsoft Intune".](https://support.microsoft.com/help/4457481/troubleshooting-scep-certificate-profile-deployment-in-intune)</span><span class="sxs-lookup"><span data-stu-id="50b3a-118">For more info, see [Overview for troubleshooting SCEP certificate profiles with Microsoft Intune](https://support.microsoft.com/help/4457481/troubleshooting-scep-certificate-profile-deployment-in-intune).</span></span>

<span data-ttu-id="50b3a-119">**Įrenginyje diegiau "Wi-Fi" profilį. "Intune" rodo, kad jis buvo sėkmingas, tačiau įrenginys neprisijungia prie "Wi-Fi".**</span><span class="sxs-lookup"><span data-stu-id="50b3a-119">**I deployed a Wi-Fi profile to a device. Intune is showing that it was successful, but the device is not connecting to the Wi-Fi.**</span></span>

<span data-ttu-id="50b3a-120">Sėkminga būsena reiškia, kad "Intune" sėkmingai įdiegė profilį kaip sukonfigūruotas.</span><span class="sxs-lookup"><span data-stu-id="50b3a-120">A successful status means that Intune has successfully deployed the profile as configured.</span></span> <span data-ttu-id="50b3a-121">Tačiau šios konfigūracijos gali neatitikti tinklo ir (arba) autentifikavimo reikalavimų.</span><span class="sxs-lookup"><span data-stu-id="50b3a-121">However, these configurations might not match your network and/or authentication requirements.</span></span> <span data-ttu-id="50b3a-122">Jei norite gauti daugiau informacijos apie bandė ryšį, peržiūrėti žurnalus infrastruktūros ir autentifikavimo tarnyba (Wi-Fi prieigos taško valdiklyje ir NPS/Radius serveryje).</span><span class="sxs-lookup"><span data-stu-id="50b3a-122">For more details about the attempted connection, review logs in the infrastructure and authentication service (on the Wi-Fi Access point controller and NPS/Radius server).</span></span> <span data-ttu-id="50b3a-123">Jums gali tekti dirbti su tinklo infrastruktūros komanda arba trečiosios šalies "Wi-Fi" tiekėju, kad galėtumėte rinkti ir peržiūrėti žurnalus.</span><span class="sxs-lookup"><span data-stu-id="50b3a-123">You might have to work with your network infrastructure team, or the third-party Wi-Fi vendor, to gather and review logs.</span></span>