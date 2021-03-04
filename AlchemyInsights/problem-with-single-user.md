---
title: Problema su vienu vartotoju
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
- "9004687"
- "8469"
ms.openlocfilehash: f3564063a3adf291ec4909ffeb2f6de0e478da96
ms.sourcegitcommit: f4ba304b92ed01e35273ecda67e9dc3ad9d475c1
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 03/04/2021
ms.locfileid: "50430200"
---
# <a name="problem-with-single-user"></a><span data-ttu-id="ad2fa-102">Problema su vienu vartotoju</span><span class="sxs-lookup"><span data-stu-id="ad2fa-102">Problem with single user</span></span>

- <span data-ttu-id="ad2fa-103">Vartotojas gali būti nesukonfigūruotas, nes tarnyba dar neturėjo galimybės įvertinti vartotojo.</span><span class="sxs-lookup"><span data-stu-id="ad2fa-103">The user may not have been provisioned because the service hasn't had a chance to evaluate the user yet.</span></span> <span data-ttu-id="ad2fa-104">Peržiūrėkite nurodymus, kaip ilgai trunka parengimas, taip pat ir eigos juostos parengimo konfigūravimo puslapyje.</span><span class="sxs-lookup"><span data-stu-id="ad2fa-104">Review the guidance for how long provisioning takes as well as the progress bar on the provisioning configuration page.</span></span> <span data-ttu-id="ad2fa-105">Jei stabili būsena, nurodyta sekcijoje papildoma informacija, yra prieš vartotojo sukūrimo/atnaujinimo/panaikinimo datą, tai reiškia, kad dar neįvertinome vartotojo.</span><span class="sxs-lookup"><span data-stu-id="ad2fa-105">If the steady state specified in the additional details section is before the date the user was created/updated/deleted, it means we have not evaluated the user yet.</span></span> <span data-ttu-id="ad2fa-106">Pagal šį scenarijų, geriausia, ką reikia padaryti – palaukite, kol bus baigta parengimo tarnyba.</span><span class="sxs-lookup"><span data-stu-id="ad2fa-106">In this scenario, the best thing to do is wait for the provisioning service to finish.</span></span>

  - <span data-ttu-id="ad2fa-107">Atkreipkite dėmesį, kad mūsų paslauga yra tik apie vartotojų pakeitimą šaltinio sistemoje (debesies HR).</span><span class="sxs-lookup"><span data-stu-id="ad2fa-107">Note that our service is only aware of changes to a user in the source system (Cloud HR).</span></span> <span data-ttu-id="ad2fa-108">"Azure AD" šaltinio sistemoje turi būti galiojantis keitimas, kad būtų galima aptikti keitimą ir srautą į "Active Directory".</span><span class="sxs-lookup"><span data-stu-id="ad2fa-108">There has to be a valid change in the source system for Azure AD to detect the change and flow it into Active Directory.</span></span>
- <span data-ttu-id="ad2fa-109">Parengimo tarnyba vertino vartotoją ir nustatė, kad jis neturėtų būti konfigūruojamas:</span><span class="sxs-lookup"><span data-stu-id="ad2fa-109">Provisioning service evaluated the user and determined it should not be provisioned:</span></span>
  - <span data-ttu-id="ad2fa-110">Jei nustatėte atributą pagal aprėpties filtrą, įsitikinkite, kad vartotojas atitinka nurodytus kriterijus.</span><span class="sxs-lookup"><span data-stu-id="ad2fa-110">If you have set an attribute based scoping filter, ensure that the user meets the criteria that you have specified.</span></span>
  - <span data-ttu-id="ad2fa-111">Jei vartotojai jau yra tikslinėse sistemose ir vartotojo būsena šaltinio ir paskirties atitikmuo, mes nesiimsime jokių tolesnių veiksmų.</span><span class="sxs-lookup"><span data-stu-id="ad2fa-111">If users already exist in the target system and the state of the user in the source and target match, we won't take any further action.</span></span>
- <span data-ttu-id="ad2fa-112">Parengimo tarnyba bandė pateikti vartotojui ir nepavyko.</span><span class="sxs-lookup"><span data-stu-id="ad2fa-112">Provisioning service attempted to provision the user and it failed.</span></span> <span data-ttu-id="ad2fa-113">Šiuose scenarijuose Peržiūrėkite parengimo žurnalų skirtuką trikčių diagnostika ir rekomendacijos:</span><span class="sxs-lookup"><span data-stu-id="ad2fa-113">For these scenarios, review the troubleshooting and recommendations tab of the provisioning logs:</span></span>
  - <span data-ttu-id="ad2fa-114">Vartotojui būtinas atributas gali trūkti vietiniame "Active Directory" arba "Azure AD".</span><span class="sxs-lookup"><span data-stu-id="ad2fa-114">A required attribute on the user might be missing in on-premises Active Directory or Azure AD.</span></span> <span data-ttu-id="ad2fa-115">Pvz., "userPrincipalName" arba "Samaccountiname" generavimo taisyklės nesugeneruoja tinkamos reikšmės.</span><span class="sxs-lookup"><span data-stu-id="ad2fa-115">For example, the userPrincipalName or sAMAccountName generation rules are not generating the right value.</span></span>
  - <span data-ttu-id="ad2fa-116">Sutampantis atributas (paprastai darbuotojai) nėra skirtas unikaliam vartotojui vietinėje "Active Directory" arba "Azure AD".</span><span class="sxs-lookup"><span data-stu-id="ad2fa-116">The matching attribute (usually employeeId) is not resolving to a unique user in on-premises Active Directory or Azure AD.</span></span> <span data-ttu-id="ad2fa-117">Pvz., "AD" yra du vartotojai su tuo pačiu darbuotojai ir Tarnyba pateikia klaidos kodą, nurodantį to paties šaltinio įrašo dublikatus paskirties įrašus.</span><span class="sxs-lookup"><span data-stu-id="ad2fa-117">For example, there are two users with the same employeeId in AD and the service returns an error code indicate duplicate target entries for the same source entry.</span></span>

<span data-ttu-id="ad2fa-118">Norėdami peržiūrėti vieno vartotojo ir grupių žurnalus, peržiūrėkite [konkretaus vartotojo problemų parengimo žurnalus](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-provisioning-logs).</span><span class="sxs-lookup"><span data-stu-id="ad2fa-118">To review logs for single user and groups, see [Review the provisioning logs for an issue with a specific user](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-provisioning-logs).</span></span>
