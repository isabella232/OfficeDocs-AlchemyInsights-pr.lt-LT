---
title: Single-Sign "Azure Active Directory" prijungtiems įrenginiams
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/24/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003257"
- "9891"
ms.openlocfilehash: f6426a3fb4addc24c5041196fe837134bf0d296b
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 03/29/2021
ms.locfileid: "51405050"
---
# <a name="single-sign-on-for-azure-active-directory-joined-devices"></a><span data-ttu-id="de279-102">Vienkartinis prisijungimas prie "Azure Active Directory" prijungtų įrenginių</span><span class="sxs-lookup"><span data-stu-id="de279-102">Single-sign on for Azure Active Directory Joined Devices</span></span>

<span data-ttu-id="de279-103">Jei turite vietinę "Active Directory" (AD) aplinką ir norite prisijungti prie ad domenu prijungtų kompiuterių prie "Azure AD", tai galite atlikti atlikdami hibridinį "Azure AD" prisijungimą.</span><span class="sxs-lookup"><span data-stu-id="de279-103">If you have an on-premises Active Directory (AD) environment and you want to join your AD domain-joined computers to Azure AD, you can accomplish this by doing hybrid Azure AD join.</span></span> <span data-ttu-id="de279-104">[Kaip: hibridinio "Azure Active Directory"](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan) sujungimo diegimo planas pateikia susijusius veiksmus, kaip įdiegti hibridinį "Azure AD" prisijungimą jūsų aplinkoje.</span><span class="sxs-lookup"><span data-stu-id="de279-104">[How To: Plan your hybrid Azure Active Directory join implementation](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan) provides you with the related steps to implement a hybrid Azure AD join in your environment.</span></span>

[<span data-ttu-id="de279-105">"Azure AD" prijungtų įrenginių konfigūravimas vietiniams įrenginiams Single-Sign Naudojant "Windows Hello" verslui</span><span class="sxs-lookup"><span data-stu-id="de279-105">Configure Azure AD joined devices for On-premises Single-Sign On using Windows Hello for Business</span></span>](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan) 

<span data-ttu-id="de279-106">**Pirminio atnaujinimo atpažinimo ženklo (PRT) problemos** Pirminis atnaujinimo atpažinimo ženklas (PRT) yra pagrindinis "Azure AD" autentifikavimo "Windows 10", "Windows Server 2016" ir naujesnėse versijose, "iOS" ir "Android" įrenginiuose artefaktas.</span><span class="sxs-lookup"><span data-stu-id="de279-106">**Primary Refresh Token (PRT) issues** A Primary Refresh Token (PRT) is a key artifact of Azure AD authentication on Windows 10, Windows Server 2016 and later versions, iOS, and Android devices.</span></span> <span data-ttu-id="de279-107">Tai JSON žiniatinklio atpažinimo ženklas (JWT), specialiai išduotas "Microsoft" pirmosios šalies atpažinimo ženklų tarpininkams, kad įgalintumėte bendrąją a prisijungimo funkciją (SSO) visuose tuose įrenginiuose naudojamose programose.</span><span class="sxs-lookup"><span data-stu-id="de279-107">It is a JSON Web Token (JWT) specially issued to Microsoft first party token brokers to enable single sign-on (SSO) across the applications used on those devices.</span></span> <span data-ttu-id="de279-108">[Dalyje Kas yra pirminis atnaujinimo atpažinimo ženklas?](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token)pateiksime išsamią informaciją, kaip "Windows 10" įrenginiuose išleidžiamas, naudojamas ir apsaugotas PRT.</span><span class="sxs-lookup"><span data-stu-id="de279-108">[In What is a Primary Refresh Token?](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token), we will provide details on how a PRT is issued, used, and protected on Windows 10 devices.</span></span>

<span data-ttu-id="de279-109">**WamDefaultSet: YES ir AzureADPrt: TAIP** Šie laukai nurodo, ar vartotojas sėkmingai autentifikavo "Azure AD", kai prisijungia prie įrenginio.</span><span class="sxs-lookup"><span data-stu-id="de279-109">**WamDefaultSet: YES and AzureADPrt: YES** These fields indicate whether the user has successfully authenticated to Azure AD when signing in to the device.</span></span> <span data-ttu-id="de279-110">Jei reikšmės yra **NE**, gali būti, kad:</span><span class="sxs-lookup"><span data-stu-id="de279-110">If the values are **NO**, it could be due:</span></span>

- <span data-ttu-id="de279-111">Netinkamas saugyklos raktas TPM, susietas su įrenginiu registruojantis (patikrinkite KeySignTest paleisdami padidintą versiją).</span><span class="sxs-lookup"><span data-stu-id="de279-111">Bad storage key in the TPM associated with the device upon registration (check the KeySignTest while running elevated).</span></span>
- <span data-ttu-id="de279-112">Alternatyvus prisijungimo ID</span><span class="sxs-lookup"><span data-stu-id="de279-112">Alternate Login ID</span></span>
- <span data-ttu-id="de279-113">HTTP tarpinis serveris nerastas</span><span class="sxs-lookup"><span data-stu-id="de279-113">HTTP Proxy not found</span></span>

<span data-ttu-id="de279-114">Įrenginių trikčių šalinimas naudojant komandą dsregcmd – [SSO būsena](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state)</span><span class="sxs-lookup"><span data-stu-id="de279-114">Troubleshoot devices using the dsregcmd command - [SSO state](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state)</span></span>
