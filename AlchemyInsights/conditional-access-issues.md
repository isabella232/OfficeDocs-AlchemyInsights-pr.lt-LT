---
title: Sąlyginės prieigos problemos
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004349"
- "7768"
ms.openlocfilehash: 7c20b26e3a038dc4392684ca410eba97cec2df30
ms.sourcegitcommit: eb685eea3ab312d404d55bfd5594a5d6d68811d1
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 01/27/2021
ms.locfileid: "50014886"
---
# <a name="conditional-access-issues"></a><span data-ttu-id="10af9-102">Sąlyginės prieigos problemos</span><span class="sxs-lookup"><span data-stu-id="10af9-102">Conditional access issues</span></span>

<span data-ttu-id="10af9-103">**Išspręskite prisijungimo diagnostikos problemas**</span><span class="sxs-lookup"><span data-stu-id="10af9-103">**Resolve problems with the Sign-in Diagnostic**</span></span>

<span data-ttu-id="10af9-104">Naudodami [prisijungimo diagnostiką](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom)galite greitai sužinoti, kas nutiko arba diagnozuoti problemas, susijusias su vartotojų prisijungtu:</span><span class="sxs-lookup"><span data-stu-id="10af9-104">You can quickly find out what happened or diagnose problems related to user sign-in by using the [Sign-in Diagnostic](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom):</span></span>

1. <span data-ttu-id="10af9-105">Paleidžia prisijungimo diagnostiką.</span><span class="sxs-lookup"><span data-stu-id="10af9-105">Launch the Sign-in Diagnostic.</span></span>
1. <span data-ttu-id="10af9-106">Raskite įvykį, kurį norite analizuoti, įvesdami informaciją apie vartotoją, taikomąją programą, prisijungimo laiką, užklausos ID arba koreliacijos ID.</span><span class="sxs-lookup"><span data-stu-id="10af9-106">Find the event to analyze by entering in the details you have about the user, application, time of sign-in, request Id, or correlation Id.</span></span>
1. <span data-ttu-id="10af9-107">Peržiūrėkite diagnostikos rezultatus, kuriuose pateikiama išsami informacija apie tai, kas nutiko ir kokių veiksmų galite imtis, kad keistumėte (jei reikia kokių nors pasikeitimų).</span><span class="sxs-lookup"><span data-stu-id="10af9-107">Review the diagnostic results showing the details of what happened and what actions you can take to make changes (if any changes are needed).</span></span>

<span data-ttu-id="10af9-108">**Prisijungimo trikčių šalinimo veiksmai**</span><span class="sxs-lookup"><span data-stu-id="10af9-108">**Steps to Troubleshoot a Sign-In**</span></span> 

1. <span data-ttu-id="10af9-109">Pereikite į "Azure AD" prisijungimo puslapį.</span><span class="sxs-lookup"><span data-stu-id="10af9-109">Navigate to the Azure AD Sign-in page.</span></span>
1. <span data-ttu-id="10af9-110">Filtruokite prisijungimo pagal vartotoją, laiko intervalą, taikomąją programą, būseną, kliento programą ir kt.</span><span class="sxs-lookup"><span data-stu-id="10af9-110">Filter sign-ins by user, time range, application, status, client app, and so on.</span></span>
1. <span data-ttu-id="10af9-111">Pasirinkite prisijungimo įvykį ir peržiūrėkite skirtuką sąlyginė prieiga, kad pamatytumėte, kurios strategijos buvo įvertintos.</span><span class="sxs-lookup"><span data-stu-id="10af9-111">Select a sign-in event and view the Conditional Access tab to see which policies were evaluated.</span></span>
1. <span data-ttu-id="10af9-112">Spustelėkite strategijos eilutę, kad peržiūrėtumėte išsamią informaciją apie strategiją ir suprastumėte, kodėl ji pritaikyta.</span><span class="sxs-lookup"><span data-stu-id="10af9-112">Click on the row of a policy to view the policy details and understand why it applied.</span></span>

<span data-ttu-id="10af9-113">**"Sąlyginės prieigos strategijos" įrankių šalinimas**</span><span class="sxs-lookup"><span data-stu-id="10af9-113">**Tools to troubleshoot a Conditional Access policy**</span></span>

- <span data-ttu-id="10af9-114">Tik ataskaitos režimas leidžia įvertinti strategiją netrukdant vartotojams.</span><span class="sxs-lookup"><span data-stu-id="10af9-114">Report-only mode lets you evaluate a policy without impacting users.</span></span>
- <span data-ttu-id="10af9-115">"If" įrankis leidžia imituoti prisijungimo įvykius ir peržiūrėti, kurios strategijos taikomos.</span><span class="sxs-lookup"><span data-stu-id="10af9-115">What-if tool lets you simulate sign-in events and see which policies apply.</span></span>
- <span data-ttu-id="10af9-116">Įžvalga ir ataskaitos darbaknygė rodo kiekvienos strategijos poveikį realiuoju laiku.</span><span class="sxs-lookup"><span data-stu-id="10af9-116">Insights and reporting workbook displays real-time impact of each policy.</span></span>

<span data-ttu-id="10af9-117">**Pradinės apsaugos strategijos**</span><span class="sxs-lookup"><span data-stu-id="10af9-117">**Baseline Protection Policies**</span></span>

<span data-ttu-id="10af9-118">Bazinės apsaugos strategijos pasenusios.</span><span class="sxs-lookup"><span data-stu-id="10af9-118">Baseline Protection policies have been deprecated.</span></span> <span data-ttu-id="10af9-119">Jie nebėra vykdomi ir netrukus bus pašalinti iš "Azure" portalo.</span><span class="sxs-lookup"><span data-stu-id="10af9-119">They are no longer being enforced and will soon be removed from Azure portal.</span></span> <span data-ttu-id="10af9-120">Rekomenduojame įgalinti [saugos numatytąsias reikšmes](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults).</span><span class="sxs-lookup"><span data-stu-id="10af9-120">We recommend enabling [security defaults](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults).</span></span>

<span data-ttu-id="10af9-121">Daugiau informacijos apie sąlyginę prieigą rasite:</span><span class="sxs-lookup"><span data-stu-id="10af9-121">For more information on Conditional Access see:</span></span>

<span data-ttu-id="10af9-122">[Geriausios "Azure Active Directory](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices)  
 " sąlyginės prieigos praktikos [Sąlyginės prieigos sąlygos](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices)  
 " [Sąlyginės prieigos](https://docs.microsoft.com/azure/active-directory/conditional-access/controls)  
 " valdikliai [Vietos sąlygine prieiga](https://docs.microsoft.com/azure/active-directory/conditional-access/location-condition)</span><span class="sxs-lookup"><span data-stu-id="10af9-122">[Best practices for conditional access in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices) 
[Conditions in Conditional Access](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices) 
[Controls in Conditional Access](https://docs.microsoft.com/azure/active-directory/conditional-access/controls) 
[Locations in Conditional Access ](https://docs.microsoft.com/azure/active-directory/conditional-access/location-condition)</span></span>
