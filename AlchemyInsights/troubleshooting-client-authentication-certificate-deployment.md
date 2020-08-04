---
title: Kliento autentifikavimo sertifikato diegimo trikčių diagnostika
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
- "1546"
- "9000076"
ms.openlocfilehash: 698329d7705af320c9f679b92532b58ac84e6624
ms.sourcegitcommit: e90b918f02102cd9764881c2d8c914567c6b070e
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 07/29/2020
ms.locfileid: "46555305"
---
# <a name="troubleshooting-client-authentication-certificate-deployment"></a><span data-ttu-id="d6475-102">Kliento autentifikavimo sertifikato diegimo trikčių diagnostika</span><span class="sxs-lookup"><span data-stu-id="d6475-102">Troubleshooting Client Authentication certificate deployment</span></span>

<span data-ttu-id="d6475-103">Intune NDES/SCEP ir PKCS/PFX kliento sertifikatų profiliai paprastai naudojami kartu su kitų tipų profiliais, pvz., "Wifi", "VPN" ir el. paštu, kad vartotojai galėtų autentifikuoti įmonės išteklius.</span><span class="sxs-lookup"><span data-stu-id="d6475-103">Intune NDES/SCEP and PKCS/PFX Client certificates profiles are commonly used in conjunction with other profiles types such as Wifi, VPN, and email to allow users to authenticate to corporate resources.</span></span> <span data-ttu-id="d6475-104">Kai šie profilio tipai yra susiję su kliento sertifikato profilio priklauso nuo sėkmingo diegimo, kad profilis.</span><span class="sxs-lookup"><span data-stu-id="d6475-104">When those profile types are linked to a client certificate profile are dependant on the successful deployment of that profile.</span></span>

<span data-ttu-id="d6475-105">Pradiniam infrastruktūros nustatymui ir susijusiai kliento sertifikato profilio konfigūracijai dažnai reikia šalinti triktis.</span><span class="sxs-lookup"><span data-stu-id="d6475-105">Initial infrastructure setup and associated configuration of the Client Certificate profile often require troubleshooting.</span></span> <span data-ttu-id="d6475-106">Išsamų vadovą sėkmingai nustatyti NDES jungtis ir trikčių šalinimo patarimų izoliuoti problemas, susijusias su sertifikato diegimas, žr.:</span><span class="sxs-lookup"><span data-stu-id="d6475-106">For a step-by-step guide to successful setup of the NDES connector and troubleshooting guidance to isolate issues with certificate deployment, see:</span></span> 

- [<span data-ttu-id="d6475-107">Konfigūruoti infrastruktūrą, palaikančią SCEP su Intune</span><span class="sxs-lookup"><span data-stu-id="d6475-107">Configure infrastructure to support SCEP with Intune</span></span>](https://support.microsoft.com/help/4459540/troubleshoot-ndes-configuration-for-use-with-intune)
- [<span data-ttu-id="d6475-108">Scep sertifikatų profilių trikčių diagnostika naudojant "Microsoft Intune"</span><span class="sxs-lookup"><span data-stu-id="d6475-108">Overview for troubleshooting SCEP certificate profiles with Microsoft Intune</span></span>](https://support.microsoft.com/help/4457481/troubleshooting-scep-certificate-profile-deployment-in-intune)

<span data-ttu-id="d6475-109">Naudokite nurodytą "PowerShell" scenarijus, kad padėtumėte patikrinti konfigūraciją.</span><span class="sxs-lookup"><span data-stu-id="d6475-109">Use the referenced powershell scripts to help verify your configuration.</span></span> <span data-ttu-id="d6475-110">Daugiau informacijos ieškokite [Intune Certificate connector verification scripts](https://github.com/microsoftgraph/powershell-intune-samples/tree/master/CertificationAuthority).</span><span class="sxs-lookup"><span data-stu-id="d6475-110">For more info, see [Intune Certificate connector verification scripts](https://github.com/microsoftgraph/powershell-intune-samples/tree/master/CertificationAuthority).</span></span>

  
<span data-ttu-id="d6475-111">**Kitos bendros problemos**</span><span class="sxs-lookup"><span data-stu-id="d6475-111">**Other common issues**</span></span>

<span data-ttu-id="d6475-112">**Kai bandau įdiegti Intune sertifikato jungtį NDES jungties serveryje, gaunu pranešimą" sertifikato užklausos slaptažodžio patikrinti negalima. Jis gali būti naudojamas jau. Gaukite naują slaptažodį, kad pateiktumėte su šia užklausa."**</span><span class="sxs-lookup"><span data-stu-id="d6475-112">**When I try to install the Intune certificate connector on the NDES connector server, I get the message, "The password in the certificate request cannot be verified. It may have been used already. Obtain a new password to submit with this request."**</span></span>  

<span data-ttu-id="d6475-113">Šis pranešimas reiškia, kad turite paleisti sertifikato jungties diegimą kaip administratorius.</span><span class="sxs-lookup"><span data-stu-id="d6475-113">This message means that you need to run the certificate connector installation as an Administrator.</span></span>

<span data-ttu-id="d6475-114">Kai kuriose aplinkose, serveriai, kuriuose veikia Intune sertifikatas turi naudoti tarpinį serverį prisijungti prie Intune, ir todėl sertifikato jungtis turi naudoti tarpinį serverį.</span><span class="sxs-lookup"><span data-stu-id="d6475-114">In some environments, the servers where the Intune Certificate runs must use a proxy server to connect to Intune, and so the Certificate Connector must use a proxy.</span></span> <span data-ttu-id="d6475-115">Tam tikrais atvejais NDES jungtis nepaiso sukonfigūruotų tarpinio serverio parametrų, todėl gali reikėti konfigūruoti tarpinio serverio parametrus vykdant "LocalSystem" saugos kontekstą.</span><span class="sxs-lookup"><span data-stu-id="d6475-115">In some circumstances, the NDES Connector ignores the configured proxy settings, and it might be necessary to configure the proxy settings while running in the security context of LocalSystem.</span></span> 
 
<span data-ttu-id="d6475-116">Sprendimas yra paleisti "Internet Explorer" kaip sistemą ir konfigūruoti tarpinį serverį IE.</span><span class="sxs-lookup"><span data-stu-id="d6475-116">The solution is to run Internet Explorer as SYSTEM and configure a proxy in IE.</span></span> <span data-ttu-id="d6475-117">Iš naujo paleidus Intune jungtis paslaugos, NDES jungtis prisijungia prie Intune.</span><span class="sxs-lookup"><span data-stu-id="d6475-117">After a restart of the Intune Connector Service, the NDES Connector connects to Intune.</span></span>

<span data-ttu-id="d6475-118">**Vartotojo įrenginiai nebegauja SCEP sertifikatų iš NDES.**</span><span class="sxs-lookup"><span data-stu-id="d6475-118">**User devices are no longer receiving SCEP certificates from NDES.**</span></span>

<span data-ttu-id="d6475-119">Gali būti, kad kliento autentifikavimo sertifikato, išduoto NDES serverio ir nurodyta NDES jungties diegimo metu, baigėsi arba jo nėra.</span><span class="sxs-lookup"><span data-stu-id="d6475-119">It is possible that the Client Authentication certificate issued to the NDES server, and specified during the NDES connector installation, has expired or is missing.</span></span> <span data-ttu-id="d6475-120">Norėdami išspręsti:</span><span class="sxs-lookup"><span data-stu-id="d6475-120">To resolve:</span></span> 
 
1. <span data-ttu-id="d6475-121">Pašalinti NDES jungtis.</span><span class="sxs-lookup"><span data-stu-id="d6475-121">Uninstall the NDES connector.</span></span>  
2. <span data-ttu-id="d6475-122">Naudokite šią informaciją norėdami pateikti užklausą dėl naujo kliento autentifikavimo arba serverio autentifikavimo sertifikato:</span><span class="sxs-lookup"><span data-stu-id="d6475-122">Use these details to request a new client authentication or server authentication certificate:</span></span> 
 
    - <span data-ttu-id="d6475-123">Temos pavadinimas: CN = išorinis fqdn</span><span class="sxs-lookup"><span data-stu-id="d6475-123">Subject name: CN=external fqdn</span></span>  
    - <span data-ttu-id="d6475-124">Tema alternatyvus pavadinimas (abu yra privalomi): DNS = išorinis fqdn, DNS = vidaus fqdn</span><span class="sxs-lookup"><span data-stu-id="d6475-124">Subject alternative name (both are required): DNS=external fqdn, DNS=internal fqdn</span></span> 
 
3. <span data-ttu-id="d6475-125">Iš naujo įdiekite NDES jungtis su nauju sertifikatu.</span><span class="sxs-lookup"><span data-stu-id="d6475-125">Reinstall the NDES connector with the new certificate.</span></span>