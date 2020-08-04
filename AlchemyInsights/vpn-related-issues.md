---
title: Su VPN susijusios problemos
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
- "1545"
- "9000076"
ms.openlocfilehash: 134d78f30216dfd268c5999a5032b7d7ad1d7dd8
ms.sourcegitcommit: 0e50dfcdb3f6aa72368279e23b83efecb9dc9c3f
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 07/28/2020
ms.locfileid: "46555233"
---
# <a name="vpn-related-issues"></a><span data-ttu-id="be204-102">Su VPN susijusios problemos</span><span class="sxs-lookup"><span data-stu-id="be204-102">VPN related issues</span></span>

<span data-ttu-id="be204-103">Sėkmingas VPN ryšio diegimas MDM klientams priklauso nuo įdiegto profilio, kuris teisingai atspindi VPN infrastruktūros reikalavimus.</span><span class="sxs-lookup"><span data-stu-id="be204-103">Successful implementation of VPN connectivity for MDM clients depends on a deployed profile that correctly reflects the requirements of the VPN infrastructure.</span></span> <span data-ttu-id="be204-104">Atitinkamų parametrų kliento platformose, kurį tiriate, žr.:</span><span class="sxs-lookup"><span data-stu-id="be204-104">For the appropriate settings for the client platforms you are investigating, see:</span></span> 

[<span data-ttu-id="be204-105">"Windows 10" ir "Windows Holographic" įrenginio parametrai VPN ryšiams įtraukti naudojant "Intune"</span><span class="sxs-lookup"><span data-stu-id="be204-105">Windows 10 and Windows Holographic device settings to add VPN connections using Intune</span></span>](https://docs.microsoft.com/intune/vpn-settings-windows-10)  
[<span data-ttu-id="be204-106">VPN parametrų įtraukimas "iOS" ir "iPadOS" įrenginiuose programoje "Microsoft Intune"</span><span class="sxs-lookup"><span data-stu-id="be204-106">Add VPN settings on iOS and iPadOS devices in Microsoft Intune</span></span>](https://docs.microsoft.com/intune/vpn-settings-ios)  
[<span data-ttu-id="be204-107">"Android" įrenginio nustatymai konfigūruoti VPN Intune</span><span class="sxs-lookup"><span data-stu-id="be204-107">Android device settings to configure VPN in Intune</span></span>](https://docs.microsoft.com/intune/vpn-settings-android)  
[<span data-ttu-id="be204-108">VPN parametrų įtraukimas "macOS" įrenginiuose "Microsoft Intune"</span><span class="sxs-lookup"><span data-stu-id="be204-108">Add VPN settings on macOS devices in Microsoft Intune</span></span>](https://docs.microsoft.com/mem/intune/configuration/vpn-settings-macos)

<span data-ttu-id="be204-109">Jei jūsų VPN profilis naudoja sertifikatu pagrįstą autentifikavimą, įsitikinkite, kad sėkmingai įdiegti šakninis sertifikatas ir kliento autentifikavimo sertifikato profiliai, susieti su VPN profiliu.</span><span class="sxs-lookup"><span data-stu-id="be204-109">If your VPN profile uses certificate based authentication, make sure that the root certificate and client authentication certificate profiles linked to the VPN profile are deployed successfully.</span></span>

<span data-ttu-id="be204-110">**Dažniausiai pasitaikančios problemos**</span><span class="sxs-lookup"><span data-stu-id="be204-110">**Common Issues**</span></span>

<span data-ttu-id="be204-111">**Aš įdiegiau VPN profilį įrenginyje. "Intune" rodo, kad jis buvo sėkmingas, tačiau įrenginys neprisijungia prie VPN.**</span><span class="sxs-lookup"><span data-stu-id="be204-111">**I deployed a VPN profile to a device. Intune is showing that it was successful, but the device is not connecting to the VPN.**</span></span>

<span data-ttu-id="be204-112">Sėkminga būsena reiškia, kad "Intune" sėkmingai įdiegė profilį kaip sukonfigūruotas.</span><span class="sxs-lookup"><span data-stu-id="be204-112">A successful status means that Intune has successfully deployed the profile as configured.</span></span> <span data-ttu-id="be204-113">Tačiau šios konfigūracijos gali neatitikti tinklo ir (arba) autentifikavimo reikalavimų.</span><span class="sxs-lookup"><span data-stu-id="be204-113">However, these configurations might not match your network and/or authentication requirements.</span></span> <span data-ttu-id="be204-114">Peržiūrėkite žurnalus infrastruktūros ir autentifikavimo tarnybos (VPN serverio ir NPS/Radius serverio) daugiau informacijos apie bandė ryšį.</span><span class="sxs-lookup"><span data-stu-id="be204-114">Review logs in the infrastructure and authentication service (on the VPN server and NPS/Radius server) for more details about the attempted connection.</span></span> <span data-ttu-id="be204-115">Norint rinkti ir peržiūrėti žurnalus, gali reikėti dirbti su tinklo infrastruktūros komanda arba trečiosios šalies VPN tiekėju.</span><span class="sxs-lookup"><span data-stu-id="be204-115">You might need to work with your network infrastructure team, or the third-party VPN vendor, to gather and review logs.</span></span>

<span data-ttu-id="be204-116">**Kai konfigūruoju pasirinktinį VPN, skirtą "iOS", kiekvienos programos VPN funkcija nepasiekiama.**</span><span class="sxs-lookup"><span data-stu-id="be204-116">**When I configure a custom VPN for iOS, the per-app VPN feature isn't made available.**</span></span>

<span data-ttu-id="be204-117">"iOS" įrenginių "Intune" programos VPN šiuo metu galimas konkrečiam teikėjų ir partnerių sąrašui, kuris taip pat turi atitikti sertifikato sąlygas prieš konfigūruodami programos VPN.</span><span class="sxs-lookup"><span data-stu-id="be204-117">Per-app VPN for iOS devices in Intune is currently available to a specific list of providers and partners, who must also meet the certificate prerequisites before configuring a per-app VPN.</span></span> <span data-ttu-id="be204-118">Daugiau informacijos rasite ["iOS" / "iPadOS" įrenginių nustatymas už programėlę Virtualusis privatusis tinklas (VPN) in Intune](https://docs.microsoft.com/intune/vpn-setting-configure-per-app).</span><span class="sxs-lookup"><span data-stu-id="be204-118">For more info, see [Set up per-app Virtual Private Network (VPN) for iOS/iPadOS devices in Intune](https://docs.microsoft.com/intune/vpn-setting-configure-per-app).</span></span> 

<span data-ttu-id="be204-119">Daugiau informacijos apie visus VPN ryšio tipus in Intune rasite [VPN profilių kūrimas, kad prisijungtumėte prie VPN serverių intune](https://docs.microsoft.com/intune/vpn-settings-configure).</span><span class="sxs-lookup"><span data-stu-id="be204-119">For more info about all VPN connection types in Intune, see [Create VPN profiles to connect to VPN servers in Intune](https://docs.microsoft.com/intune/vpn-settings-configure).</span></span>  

<span data-ttu-id="be204-120">**"iOS" pareikalavus VPN neįsijungia, kai pasiekiamas sukonfigūruotas domenas**</span><span class="sxs-lookup"><span data-stu-id="be204-120">**iOS On-Demand VPN is not triggering when a configured domain is accessed**</span></span>

<span data-ttu-id="be204-121">Norėdami patikrinti automatinius VPN parametrus, nustatykite šias reikšmes:</span><span class="sxs-lookup"><span data-stu-id="be204-121">To test automatic VPN settings, set the following values:</span></span>

<span data-ttu-id="be204-122">Noriu atlikti šiuos veiksmus: **Įvertinkite kiekvieną bandymą prisijungti**</span><span class="sxs-lookup"><span data-stu-id="be204-122">I want to do the following: **Evaluate each connection attempt**</span></span> 

<span data-ttu-id="be204-123">Pasirinkite, ar norite prisijungti: **jei reikia, prisijunkite**</span><span class="sxs-lookup"><span data-stu-id="be204-123">Choose whether to connect: **Connect if needed**</span></span>

<span data-ttu-id="be204-124">Kai vartotojai pasiekia šiuos domenus: **paskirties** *domeno vardas*</span><span class="sxs-lookup"><span data-stu-id="be204-124">When users access these domains: **target** *domain name*</span></span>

<span data-ttu-id="be204-125">Jei pirmiau konfigūracija nesėkminga, pridėkite šį elementą:</span><span class="sxs-lookup"><span data-stu-id="be204-125">If the above configuration is not successful, add the following element:</span></span>

<span data-ttu-id="be204-126">Kai šis URL nepasiekiamas, priverskite prisijungti VPN: **BADURL**</span><span class="sxs-lookup"><span data-stu-id="be204-126">When this URL is unreachable, force connect the VPN: **BADURL**</span></span>