---
title: MIM sinchronizavimo paslaugos konfigūravimas
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8472"
- "9004688"
ms.openlocfilehash: 48e9a0e8c26088b690092bfaedfba641841739f6
ms.sourcegitcommit: 379e132c4d21ecf703d5506484ec96a767fdda39
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 03/04/2021
ms.locfileid: "50481870"
---
# <a name="configure-mim-sync-service"></a><span data-ttu-id="85ea6-102">MIM sinchronizavimo paslaugos konfigūravimas</span><span class="sxs-lookup"><span data-stu-id="85ea6-102">Configure MIM Sync service</span></span>

<span data-ttu-id="85ea6-103">"Microsoft Identity Manager" (MIM) Sinchronizavimo tarnyba yra MIM komponentas.</span><span class="sxs-lookup"><span data-stu-id="85ea6-103">Microsoft Identity Manager (MIM) Synchronization Service is a component of MIM.</span></span> <span data-ttu-id="85ea6-104">Tai centralizuota vietinė tarnyba, kuri saugo ir sujungia informaciją apie organizacijas, kurios turi kelis vietinius katalogus ir duomenų bazes.</span><span class="sxs-lookup"><span data-stu-id="85ea6-104">It is a centralized on-premises service that stores and integrates information for organizations that have multiple on-premises directories and databases.</span></span> <span data-ttu-id="85ea6-105">Jums gali būti suteikta galimybė išspręsti problemą su MIM sinchronizavimu, jei problema buvo išspręsta naujausiame "MIM" naujinime arba yra viena iš kitų toliau nurodytų problemų.</span><span class="sxs-lookup"><span data-stu-id="85ea6-105">You may be able to resolve your problem with MIM Sync if the issue was addressed in a recent update to MIM or is one of the other issues mentioned in the below section.</span></span>

<span data-ttu-id="85ea6-106">**Rekomenduojami veiksmai**</span><span class="sxs-lookup"><span data-stu-id="85ea6-106">**Recommended steps**</span></span>

1. <span data-ttu-id="85ea6-107">Įsitikinkite, kad naudojate vėliausią MIM sinchronizavimo naujinimą ir patikrinkite [Mim sinchronizavimo leidimo pastabas](https://docs.microsoft.com/microsoft-identity-manager/reference/version-history) , kad nustatytumėte, ar problema buvo išspręsta naujinime.</span><span class="sxs-lookup"><span data-stu-id="85ea6-107">Ensure that you are using a recent update of MIM Sync and check the [MIM Sync release notes](https://docs.microsoft.com/microsoft-identity-manager/reference/version-history) to determine if the issue has been resolved in an update.</span></span>
2. <span data-ttu-id="85ea6-108">Jei problema yra bendra LDAP, Bendrasis SQL, Lotus Domino arba žiniatinklio tarnybų jungtis, įsitikinkite, kad naudojate naujausią [bendrųjų jungčių](https://docs.microsoft.com/microsoft-identity-manager/reference/microsoft-identity-manager-2016-connector-version-history)naujinimą.</span><span class="sxs-lookup"><span data-stu-id="85ea6-108">If the problem is with the Generic LDAP, Generic SQL, Lotus Domino or Web Services connector, ensure that you are using a recent update of the [generic connectors](https://docs.microsoft.com/microsoft-identity-manager/reference/microsoft-identity-manager-2016-connector-version-history).</span></span>
3. <span data-ttu-id="85ea6-109">Jei MIM sinchronizavimo vykdymas sustabdomas su klaida, skaitykite " [Run" klaidų kodų](https://docs.microsoft.com/microsoft-identity-manager/reference/maerrorcodes) , kad nustatytumėte galimas priežastis, lentelę.</span><span class="sxs-lookup"><span data-stu-id="85ea6-109">If an MIM Sync-run stops with an error, consult the table of [run error codes](https://docs.microsoft.com/microsoft-identity-manager/reference/maerrorcodes) to determine the potential causes.</span></span>
4. <span data-ttu-id="85ea6-110">Jei paleisti sustoja naudodami **plėtinį – dll – išimtis**, tada spustelėkite šiuos žodžius, kad atidarytumėte langą **jungties vietos objekto ypatybės** , ir spustelėkite **rietuvės sekimas...** , kad pamatytumėte daugiau informacijos apie PRIEŽASTĮ, kaip aprašyta [plėtinio – DLL – išimtis](https://social.technet.microsoft.com/wiki/contents/articles/7515.fim-troubleshooting-extension-dll-exception.aspx).</span><span class="sxs-lookup"><span data-stu-id="85ea6-110">If the run stops with **extension-dll-exception**, then click on those words to open the **Connector Space Object properties** window, and click on **Stack Trace...** to see more information on the underlying cause, as described in [Extension-DLL-Exception](https://social.technet.microsoft.com/wiki/contents/articles/7515.fim-troubleshooting-extension-dll-exception.aspx).</span></span>
5. <span data-ttu-id="85ea6-111">Jei slaptažodžio keitimo pranešimų tarnybos (PCNS) komponento ataskaitos **klaida 6025** įvykių rodinyje sinchronizuojant slaptažodžius, patikrinkite " [PCNS" ataskaitų klaidos 6025](https://social.technet.microsoft.com/wiki/contents/articles/4159.pcns-troubleshooting-event-id-6025.aspx).</span><span class="sxs-lookup"><span data-stu-id="85ea6-111">If the Password Change Notification Service (PCNS) component reports **error 6025** in the event log during password synchronization, check the guide for troubleshooting [PCNS reporting error 6025](https://social.technet.microsoft.com/wiki/contents/articles/4159.pcns-troubleshooting-event-id-6025.aspx).</span></span>
6. <span data-ttu-id="85ea6-112">Jei visas sinchronizavimas su FIM tarnybos valdymo agentu yra lėtas, pažymėkite **automatinio padidinimo** parametrą, skirtą tempdb, kaip aprašyta skyriuje [trikčių šalinimas lėtas arba kabinamas visas sinchronizavimas](https://social.technet.microsoft.com/wiki/contents/articles/14713.troubleshooting-fim-performance-slow-or-hanging-full-synchronization.aspx).</span><span class="sxs-lookup"><span data-stu-id="85ea6-112">If full synchronization with the FIM Service Management Agent is slow, check the **auto grow** setting for TempDB, as described in [Troubleshooting slow or hanging full synchronization](https://social.technet.microsoft.com/wiki/contents/articles/14713.troubleshooting-fim-performance-slow-or-hanging-full-synchronization.aspx).</span></span>
7. <span data-ttu-id="85ea6-113">Jei įvyksta klaida, kai sustojo serveris su nepavykusia kūrimo-Via-Web-Services, naudodami FIM tarnybos tvarkymo agentą, žiūrėkite [palaikymo-info: nepavyko – kūrimas – Via – Web – Services](https://docs.microsoft.com/archive/blogs/iamsupport/support-info-fimma-failed-creation-via-web-services) dėl priežasčių apžvalgos.</span><span class="sxs-lookup"><span data-stu-id="85ea6-113">If you are encountering an error of stopped-server with failed-creation-via-web-services using the FIM Service Management Agent, see [Support-Info: failed-creation-via-web-services](https://docs.microsoft.com/archive/blogs/iamsupport/support-info-fimma-failed-creation-via-web-services) for an overview of causes.</span></span>

