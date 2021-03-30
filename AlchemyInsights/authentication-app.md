---
title: Autentifikavimo programa
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
- "9003252"
- "9909"
ms.openlocfilehash: 67331a9661ee67c4a861feb1a4292255a4d37133
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 03/29/2021
ms.locfileid: "51405066"
---
# <a name="authentication-app"></a><span data-ttu-id="fe702-102">Autentifikavimo programa</span><span class="sxs-lookup"><span data-stu-id="fe702-102">Authentication app</span></span>

<span data-ttu-id="fe702-103">Jei esate visuotinis administratorius, naudodami prisijungimo diagnostiką galite greitai sužinoti, kas nutiko arba nustatyti problemas, susijusias [su vartotojo prisijungimu.](https://ms.portal.azure.com/microsoft.onmicrosoft.com?loginHint=shhada@microsoft.com#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom)</span><span class="sxs-lookup"><span data-stu-id="fe702-103">If you are a Global Admin, you can quickly find out what happened or diagnose problems related to user-sign in by using the [Sign-in Diagnostics](https://ms.portal.azure.com/microsoft.onmicrosoft.com?loginHint=shhada@microsoft.com#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom).</span></span>

1. <span data-ttu-id="fe702-104">Pradėkite diagnostiką spustelėdami mygtuką[Paleisti diagnostiką.](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom)</span><span class="sxs-lookup"><span data-stu-id="fe702-104">Start the diagnostics by clicking "[Launch Diagnostic](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom)" button.</span></span> 
1. <span data-ttu-id="fe702-105">Raskite analizuojamą įvykį įvesdami išsamią informaciją apie vartotoją, taikomąją programą, prisijungimo laiką, užklausos ID arba koreliacijos ID.</span><span class="sxs-lookup"><span data-stu-id="fe702-105">Find the event to analyze by entering in the details you have about the user, application, time of sign-in, request Id, or correlation Id.</span></span>
1. <span data-ttu-id="fe702-106">Peržiūrėkite diagnostikos rezultatus, kuriuose rodoma išsami informacija apie tai, kas nutiko ir kokius veiksmus galite atlikti, jei reikia atlikti keitimus.</span><span class="sxs-lookup"><span data-stu-id="fe702-106">Review the diagnostic results showing the details of what happened and what actions you can take to make changes, if any changes are needed.</span></span>

<span data-ttu-id="fe702-107">**Patikrinkite taikomą scenarijų:**</span><span class="sxs-lookup"><span data-stu-id="fe702-107">**Check the scenario that is applicable:**</span></span>

1. <span data-ttu-id="fe702-108">Jei vartotojas negaus "push" pranešimo "Microsoft Authenticator" programoje, patikrinkite, ar jie nerodomas pagal MFA užblokuotus vartotojus, kaip aprašyta skyriuje Vartotojų blokavimas ir [atblokavimas.](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom)</span><span class="sxs-lookup"><span data-stu-id="fe702-108">If a user is not getting a push notification in the Microsoft Authenticator app, verify they are not shown under the MFA blocked users as described in [Block and unblock users](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom).</span></span>
1. <span data-ttu-id="fe702-109">Jei vartotojas nėra užblokuotas naudoti MFA, bet negauna "push" pranešimo, jis gali atidaryti "Microsoft Authenticator" programą, kuri išims laukiančias patvirtinimo užklausas.</span><span class="sxs-lookup"><span data-stu-id="fe702-109">If the user is not blocked for MFA but does not receive a push notification, they can open the Microsoft Authenticator app, which will pull the pending approval requests.</span></span>
1. <span data-ttu-id="fe702-110">Kaip alternatyvus prisijungimo būdas, vartotojas taip pat gali spustelėti Prisijungti kitu būdu ir pasirinkti naudoti patvirtinimo kodą iš mano mobiliųjų įrenginių programėlės.</span><span class="sxs-lookup"><span data-stu-id="fe702-110">As an alternative sign-in method, the user can also click on Sign in another way and choose use a verification code from my mobile app.</span></span>
1. <span data-ttu-id="fe702-111">"Microsoft Authenticator" programa yra vienintelis būdas, kurį gali naudoti daugelis vartotojų.</span><span class="sxs-lookup"><span data-stu-id="fe702-111">The Microsoft Authenticator App is the only available method for many users.</span></span> <span data-ttu-id="fe702-112">[Sužinokite daugiau apie saugos numatytąsias reikšmes](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults), patikrinkite [Autentifikavimo programos DUK](https://docs.microsoft.com/azure/active-directory/user-help/user-help-auth-app-faq) apie dažnai užduodamus klausimus ir kaip juos išspręsti.</span><span class="sxs-lookup"><span data-stu-id="fe702-112">[Learn more about security defaults](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults), check [Authenticator App FAQ](https://docs.microsoft.com/azure/active-directory/user-help/user-help-auth-app-faq) for commonly asked questions and how to resolve them.</span></span>
 
<span data-ttu-id="fe702-113">**Rekomenduojami vaizdo įrašai**</span><span class="sxs-lookup"><span data-stu-id="fe702-113">**Recommended Videos**</span></span>

<span data-ttu-id="fe702-114">[Kaip nustatyti autentifikavimo programą naujame telefone (2min).](https://go.microsoft.com/fwlink/?linkid=2158163&clcid=0x409)</span><span class="sxs-lookup"><span data-stu-id="fe702-114">[How to set up Authenticator App on a new phone (2min)](https://go.microsoft.com/fwlink/?linkid=2158163&clcid=0x409).</span></span>
