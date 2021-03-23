---
title: Vieno prisijungimo prie "Azure AD" įrenginių trikčių šalinimas
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003246"
- "9327"
ms.openlocfilehash: d11c24719eb2db9e9fd87c158c80cec5cb75b946
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 03/19/2021
ms.locfileid: "51036174"
---
# <a name="troubleshoot-single-sign-on-for-azure-ad-joined-devices"></a><span data-ttu-id="7a51d-102">Vieno prisijungimo prie "Azure AD" įrenginių trikčių šalinimas</span><span class="sxs-lookup"><span data-stu-id="7a51d-102">Troubleshoot Single-sign on for Azure AD Joined Devices</span></span>

<span data-ttu-id="7a51d-103">Jei turite vietinę "Active Directory" (AD) aplinką ir norite prisijungti prie savo skelbimų domeno prijungtuose kompiuteriuose į "Azure AD", galite tai atlikti atlikdami hibridinio "Azure AD" sujungimą.</span><span class="sxs-lookup"><span data-stu-id="7a51d-103">If you have an on-premises Active Directory (AD) environment and you want to join your AD domain-joined computers to Azure AD, you can accomplish this by doing hybrid Azure AD join.</span></span> <span data-ttu-id="7a51d-104">[Kaip: Suplanuokite hibridinį "Azure Active Directory" prisijungti prie diegimo](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan) suteikia jums susijusius veiksmus, kad įdiegtumėte hibridinio "Azure AD" sujungimą į aplinką.</span><span class="sxs-lookup"><span data-stu-id="7a51d-104">[How To: Plan your hybrid Azure Active Directory join implementation](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan) provides you with the related steps to implement a hybrid Azure AD join in your environment.</span></span>

<span data-ttu-id="7a51d-105">Daugiau informacijos ieškokite ["AZURE AD" sujungtų įrenginių konfigūravimas vietiniame Single-Sign "Windows Hello" verslui naudojimas](https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-aadj-sso-base).</span><span class="sxs-lookup"><span data-stu-id="7a51d-105">For more information, see [Configure Azure AD joined devices for On-premises Single-Sign On using Windows Hello for Business](https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-aadj-sso-base).</span></span>

<span data-ttu-id="7a51d-106">**Pirminio atnaujinimo atpažinimo ženklo (PRT) problemos**</span><span class="sxs-lookup"><span data-stu-id="7a51d-106">**Primary Refresh Token (PRT) issues**</span></span>

<span data-ttu-id="7a51d-107">Pirminis atnaujinimo žetonas (PRT) yra pagrindinis "Azure AD" autentifikavimo "Windows 10", "Windows Server" 2016 ir naujesnės versijos, "iOS" ir "Android" įrenginių artefaktas.</span><span class="sxs-lookup"><span data-stu-id="7a51d-107">A Primary Refresh Token (PRT) is a key artifact of Azure AD authentication on Windows 10, Windows Server 2016 and later versions, iOS, and Android devices.</span></span> <span data-ttu-id="7a51d-108">Tai yra JSON žiniatinklio žetonas (JWT), specialiai išduotas "Microsoft" pirmos šalies simboliniams brokeriams, kad būtų galima įjungti viengubus autentifikacijos (SSO) taikomąsias programas, naudojamas tuose įrenginiuose.</span><span class="sxs-lookup"><span data-stu-id="7a51d-108">It is a JSON Web Token (JWT) specially issued to Microsoft first party token brokers to enable single sign-on (SSO) across the applications used on those devices.</span></span> <span data-ttu-id="7a51d-109">Išsamesnės informacijos apie tai, kaip išduodamas PRT, naudojamas ir saugomas "Windows 10" įrenginiuose, rasite [kas yra pirminis atnaujinimo žetonas?](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token).</span><span class="sxs-lookup"><span data-stu-id="7a51d-109">For details on how a PRT is issued, used, and protected on Windows 10 devices, see [What is a Primary Refresh Token?](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token).</span></span>

<span data-ttu-id="7a51d-110">**WamDefaultSet: taip ir AzureADPrt: taip**</span><span class="sxs-lookup"><span data-stu-id="7a51d-110">**WamDefaultSet: YES and AzureADPrt: YES**</span></span>

<span data-ttu-id="7a51d-111">Šie laukai nurodo, ar vartotojas sėkmingai autentifikuotas "Azure AD" prisijungiant prie įrenginio.</span><span class="sxs-lookup"><span data-stu-id="7a51d-111">These fields indicate whether the user has successfully authenticated to Azure AD when signing in to the device.</span></span> <span data-ttu-id="7a51d-112">Jei reikšmės yra **ne**, taip gali būti dėl:</span><span class="sxs-lookup"><span data-stu-id="7a51d-112">If the values are **NO**, it could be due to:</span></span>

- <span data-ttu-id="7a51d-113">Netinkamas saugyklos raktas TPM, susietame su įrenginiu, kai registruojama</span><span class="sxs-lookup"><span data-stu-id="7a51d-113">Bad storage key in the TPM associated with the device upon registration (check the KeySignTest while running elevated)</span></span>
- <span data-ttu-id="7a51d-114">Alternatyvus prisijungimo ID</span><span class="sxs-lookup"><span data-stu-id="7a51d-114">Alternate Login ID</span></span>
- <span data-ttu-id="7a51d-115">Nerastas HTTP tarpinis serveris</span><span class="sxs-lookup"><span data-stu-id="7a51d-115">HTTP Proxy not found</span></span>

<span data-ttu-id="7a51d-116">Norėdami šalinti įrenginius naudodami komandą dsregcmd, žiūrėkite [SSO būseną](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state).</span><span class="sxs-lookup"><span data-stu-id="7a51d-116">To troubleshoot devices using the dsregcmd command, see [SSO state](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state).</span></span>
