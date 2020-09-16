---
title: Kliento autentifikavimo sertifikato diegimo trikčių diagnostika
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1546"
- "9000076"
ms.openlocfilehash: cecbd091447e63f2d5012ceaf96e050c92a171e6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47658994"
---
# <a name="troubleshooting-client-authentication-certificate-deployment"></a><span data-ttu-id="83a93-102">Kliento autentifikavimo sertifikato diegimo trikčių diagnostika</span><span class="sxs-lookup"><span data-stu-id="83a93-102">Troubleshooting Client Authentication certificate deployment</span></span>

<span data-ttu-id="83a93-103">Intune NDES/SCEP ir PKCS/PFX kliento sertifikatų profiliai paprastai naudojami kartu su kitų profilių tipais, pvz., "WiFi", VPN ir el. paštas, kad vartotojai galėtų autentifikuoti įmonės išteklius.</span><span class="sxs-lookup"><span data-stu-id="83a93-103">Intune NDES/SCEP and PKCS/PFX Client certificates profiles are commonly used in conjunction with other profiles types such as Wifi, VPN, and email to allow users to authenticate to corporate resources.</span></span> <span data-ttu-id="83a93-104">Kai šie profilių tipai yra susieti su kliento sertifikato profiliu, priklauso nuo sėkmingo šio profilio diegimo.</span><span class="sxs-lookup"><span data-stu-id="83a93-104">When those profile types are linked to a client certificate profile are dependant on the successful deployment of that profile.</span></span>

<span data-ttu-id="83a93-105">Pradinės infrastruktūros sąranka ir susieta kliento sertifikato profilio konfigūracija dažnai reikalauja trikčių diagnostikos.</span><span class="sxs-lookup"><span data-stu-id="83a93-105">Initial infrastructure setup and associated configuration of the Client Certificate profile often require troubleshooting.</span></span> <span data-ttu-id="83a93-106">Nuosekliam "NDES" jungties ir trikčių diagnostikos rekomendacijų nustatymui, siekiant izoliuoti problemas, susijusias su sertifikatų įdiegimu, rasite:</span><span class="sxs-lookup"><span data-stu-id="83a93-106">For a step-by-step guide to successful setup of the NDES connector and troubleshooting guidance to isolate issues with certificate deployment, see:</span></span> 

- [<span data-ttu-id="83a93-107">Konfigūruokite infrastruktūrą, skirtą "SCEP" su Intune</span><span class="sxs-lookup"><span data-stu-id="83a93-107">Configure infrastructure to support SCEP with Intune</span></span>](https://support.microsoft.com/help/4459540/troubleshoot-ndes-configuration-for-use-with-intune)
- [<span data-ttu-id="83a93-108">"SCEP" sertifikatų profilių trikčių šalinimas naudojant "Microsoft Intune"</span><span class="sxs-lookup"><span data-stu-id="83a93-108">Overview for troubleshooting SCEP certificate profiles with Microsoft Intune</span></span>](https://support.microsoft.com/help/4457481/troubleshooting-scep-certificate-profile-deployment-in-intune)

<span data-ttu-id="83a93-109">Naudokite nurodomus "PowerShell" scenarijus, kad patikrintumėte savo konfigūraciją.</span><span class="sxs-lookup"><span data-stu-id="83a93-109">Use the referenced powershell scripts to help verify your configuration.</span></span> <span data-ttu-id="83a93-110">Daugiau informacijos ieškokite " [Intune" sertifikato jungties patvirtinimo scenarijuose](https://github.com/microsoftgraph/powershell-intune-samples/tree/master/CertificationAuthority).</span><span class="sxs-lookup"><span data-stu-id="83a93-110">For more info, see [Intune Certificate connector verification scripts](https://github.com/microsoftgraph/powershell-intune-samples/tree/master/CertificationAuthority).</span></span>

  
<span data-ttu-id="83a93-111">**Kitos dažnai pasitaikančių problemų**</span><span class="sxs-lookup"><span data-stu-id="83a93-111">**Other common issues**</span></span>

<span data-ttu-id="83a93-112">**Kai bandau įdiegti Intune sertifikato jungtį "NDES" jungties serveryje, gaunu pranešimą "slaptažodžio sertifikato užklausoje negalima patikrinti. Jis galėjo būti jau panaudotas. Gaukite naują slaptažodį, kad pateiktumėte šią užklausą. "**</span><span class="sxs-lookup"><span data-stu-id="83a93-112">**When I try to install the Intune certificate connector on the NDES connector server, I get the message, "The password in the certificate request cannot be verified. It may have been used already. Obtain a new password to submit with this request."**</span></span>  

<span data-ttu-id="83a93-113">Šis pranešimas reiškia, kad turite vykdyti sertifikato jungties diegimą kaip administratorius.</span><span class="sxs-lookup"><span data-stu-id="83a93-113">This message means that you need to run the certificate connector installation as an Administrator.</span></span>

<span data-ttu-id="83a93-114">Kai kuriose aplinkose serveriuose, kuriuose veikia "Intune" sertifikatas, turi būti naudojamas tarpinis serveris, kad prisijungtumėte prie "Intune", todėl sertifikato jungtis turi naudoti tarpinį serverį.</span><span class="sxs-lookup"><span data-stu-id="83a93-114">In some environments, the servers where the Intune Certificate runs must use a proxy server to connect to Intune, and so the Certificate Connector must use a proxy.</span></span> <span data-ttu-id="83a93-115">Kai kuriais atvejais NDES jungtis nepaiso sukonfigūruotų tarpinio serverio parametrų, todėl gali reikėti sukonfigūruoti tarpinio serverio parametrus "LocalSystem" saugos kontekste.</span><span class="sxs-lookup"><span data-stu-id="83a93-115">In some circumstances, the NDES Connector ignores the configured proxy settings, and it might be necessary to configure the proxy settings while running in the security context of LocalSystem.</span></span> 
 
<span data-ttu-id="83a93-116">Sprendimas yra paleisti "Internet Explorer" kaip sistemą ir sukonfigūruoti tarpinį serverį IE.</span><span class="sxs-lookup"><span data-stu-id="83a93-116">The solution is to run Internet Explorer as SYSTEM and configure a proxy in IE.</span></span> <span data-ttu-id="83a93-117">Iš naujo paleidus "Intune Connector" tarnybą, "NDES Connector" prisijungia prie Intune.</span><span class="sxs-lookup"><span data-stu-id="83a93-117">After a restart of the Intune Connector Service, the NDES Connector connects to Intune.</span></span>

<span data-ttu-id="83a93-118">**Vartotojų įrenginiai nebegauna SCEP sertifikatų iš NDES.**</span><span class="sxs-lookup"><span data-stu-id="83a93-118">**User devices are no longer receiving SCEP certificates from NDES.**</span></span>

<span data-ttu-id="83a93-119">Gali būti, kad kliento autentifikavimo sertifikatas, išduotas NDES serveriui ir nurodytas NDES jungties diegimo metu, nebegalioja arba jo nėra.</span><span class="sxs-lookup"><span data-stu-id="83a93-119">It is possible that the Client Authentication certificate issued to the NDES server, and specified during the NDES connector installation, has expired or is missing.</span></span> <span data-ttu-id="83a93-120">Norėdami išspręsti:</span><span class="sxs-lookup"><span data-stu-id="83a93-120">To resolve:</span></span> 
 
1. <span data-ttu-id="83a93-121">Pašalinkite NDES jungtį.</span><span class="sxs-lookup"><span data-stu-id="83a93-121">Uninstall the NDES connector.</span></span>  
2. <span data-ttu-id="83a93-122">Naudodami šiuos duomenis prašykite naujo kliento autentifikavimo arba serverio autentifikavimo sertifikato:</span><span class="sxs-lookup"><span data-stu-id="83a93-122">Use these details to request a new client authentication or server authentication certificate:</span></span> 
 
    - <span data-ttu-id="83a93-123">Temos pavadinimas: CN = išorinis FQDN</span><span class="sxs-lookup"><span data-stu-id="83a93-123">Subject name: CN=external fqdn</span></span>  
    - <span data-ttu-id="83a93-124">Tema Alternatyvi Vardas (abu būtini): DNS = išorinis FQDN, DNS = vidinis FQDN</span><span class="sxs-lookup"><span data-stu-id="83a93-124">Subject alternative name (both are required): DNS=external fqdn, DNS=internal fqdn</span></span> 
 
3. <span data-ttu-id="83a93-125">Iš naujo įdiekite NDES jungtį su nauju sertifikatu.</span><span class="sxs-lookup"><span data-stu-id="83a93-125">Reinstall the NDES connector with the new certificate.</span></span>