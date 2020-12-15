---
title: Automatinis prisijungimas prie "Microsoft Edge"
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003848"
- "6898"
ms.openlocfilehash: 68a1119abd0a3f687b6448bb6e58c6485c239c0f
ms.sourcegitcommit: 94036315916fbc79dca2a692c2e9bc1139dd28f6
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 12/08/2020
ms.locfileid: "49677768"
---
# <a name="sign-in-to-microsoft-edge-automatically"></a><span data-ttu-id="cf99c-102">Automatinis prisijungimas prie "Microsoft Edge"</span><span class="sxs-lookup"><span data-stu-id="cf99c-102">Sign in to Microsoft Edge automatically</span></span>

<span data-ttu-id="cf99c-103">"Microsoft Edge" naudoja numatytąjį OS abonementą, kad automatiškai prisijungtų vartotojui pagal vartotojo įrenginio konfigūraciją.</span><span class="sxs-lookup"><span data-stu-id="cf99c-103">Microsoft Edge uses the OS's default account to automatically sign in a user according to how the user's device is configured.</span></span> 

<span data-ttu-id="cf99c-104">Kiekvieno įrenginio konfigūracijos tipo ir jo priklausomo vartotojo prisijungimo proceso scenarijai aprašyti toliau:</span><span class="sxs-lookup"><span data-stu-id="cf99c-104">The scenarios of each type of device configuration and its dependent user sign-in process are described below:</span></span>

1. <span data-ttu-id="cf99c-105">**Įrenginys yra hibridinis/AAD-J**: Ši parinktis pasiekiama "Windows 10", "Windows 10", "Windows" ir atitinkamose serverio versijose.</span><span class="sxs-lookup"><span data-stu-id="cf99c-105">**The device is hybrid/AAD-J**: This option is available on Windows 10, down-level Windows, and corresponding server versions.</span></span> <span data-ttu-id="cf99c-106">Vartotojai automatiškai pasirašomi naudojant "Azure Active Directory" (AD) paskyras.</span><span class="sxs-lookup"><span data-stu-id="cf99c-106">Users are automatically signed in with their Azure Active Directory (AD)accounts.</span></span>
2. <span data-ttu-id="cf99c-107">**Įrenginys yra domeno prisijungęs**: Ši parinktis pasiekiama "Windows 10", "Windows 10", "Windows" ir atitinkamose serverio versijose.</span><span class="sxs-lookup"><span data-stu-id="cf99c-107">**The device is domain-joined**: This option is available on Windows 10, down-level Windows, and corresponding server versions.</span></span> <span data-ttu-id="cf99c-108">Pagal numatytuosius parametrą vartotojai, turintys domeno paskyras, automatiškai nepasirašomi; Norėdami įgalinti automatinį jų papildymą, naudokite " **Configureonpremisesaccountautosignin** " strategiją.</span><span class="sxs-lookup"><span data-stu-id="cf99c-108">By default, users with domain accounts are not signed in automatically; to enable automatic sign-in for them, use the **ConfigureOnPremisesAccountAutoSignIn** policy.</span></span> <span data-ttu-id="cf99c-109">Norėdami įgalinti automatinį prisijungimą vartotojams su "Azure AD" paskyromis, apsvarstykite galimybę naudoti hibridinius įrenginius.</span><span class="sxs-lookup"><span data-stu-id="cf99c-109">To enable automatic sign-in for users with Azure AD accounts, consider hybrid-joining their devices.</span></span>
3. <span data-ttu-id="cf99c-110">**OS Numatytoji paskyra yra "Microsoft" abonementas**: Ši parinktis pasiekiama "Windows 10" RS3 (1709 versija, Komponavimo versija 10.0.16299) ir vėlesnės versijos.</span><span class="sxs-lookup"><span data-stu-id="cf99c-110">**The OS's default account is a Microsoft account**: This option is available on Windows 10 RS3 (version 1709, build 10.0.16299) and later versions.</span></span> <span data-ttu-id="cf99c-111">Vargu, ar scenarijus gali įvykti įmonės įrenginiuose.</span><span class="sxs-lookup"><span data-stu-id="cf99c-111">The scenario is unlikely to occur on enterprise devices.</span></span> <span data-ttu-id="cf99c-112">Tačiau jei OS numatytoji "Microsoft" paskyra yra "Microsoft" paskyra, tada "Microsoft Edge" automatiškai prisimins vartotoją su "Microsoft" abonementu.</span><span class="sxs-lookup"><span data-stu-id="cf99c-112">However, if the OS's default account is a Microsoft account, then Microsoft Edge will automatically sign in the user with the Microsoft account.</span></span>
 
 
