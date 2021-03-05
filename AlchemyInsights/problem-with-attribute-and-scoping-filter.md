---
title: Problema su atributo ir aprėpties filtru
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
- "8470"
- "9004687"
ms.openlocfilehash: 78df24c0d8a670d678e26879cf81476f1ae9b92d
ms.sourcegitcommit: 379e132c4d21ecf703d5506484ec96a767fdda39
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 03/04/2021
ms.locfileid: "50481895"
---
# <a name="problem-with-attribute-and-scoping-filter"></a><span data-ttu-id="1b924-102">Problema su atributo ir aprėpties filtru</span><span class="sxs-lookup"><span data-stu-id="1b924-102">Problem with attribute and scoping filter</span></span>

<span data-ttu-id="1b924-103">**Problema dėl nesuderinamų UPN reikšmių**</span><span class="sxs-lookup"><span data-stu-id="1b924-103">**Issue with conflicting UPN values**</span></span>

<span data-ttu-id="1b924-104">Darbo dienos iki skelbimo vartotojo parengimo darbo dienos iki skelbimo vartotojo parengimo rodomas klaidos pranešimas **Hybridsynchronizationactivedirectoryuserprincipalnamenotunique**.</span><span class="sxs-lookup"><span data-stu-id="1b924-104">The Workday to AD User Provisioning Workday to AD User Provisioning shows error message **HybridSynchronizationActiveDirectoryUserPrincipalNameNotUnique**.</span></span> <span data-ttu-id="1b924-105">Operacija nepavyko dėl to, kad į sudėties/Modifikacijos reikšmė nėra unikali.</span><span class="sxs-lookup"><span data-stu-id="1b924-105">The operation failed because UPN value provided for addition/modification is not unique forest-wide.</span></span> <span data-ttu-id="1b924-106">Išsami klaidos informacija: **CONSTRAINT_ATT_TYPE-userPrincipalName**.</span><span class="sxs-lookup"><span data-stu-id="1b924-106">Error Details: **CONSTRAINT_ATT_TYPE - userPrincipalName**.</span></span>

<span data-ttu-id="1b924-107">" **UserPrincipalName** " reikšmė, kurią bando nustatyti, kai kuriamas skelbimo vartotojo abonementas jau yra paskirties skelbimų srityje.</span><span class="sxs-lookup"><span data-stu-id="1b924-107">The **userPrincipalName** value that Workday connector is trying to set when creating the AD user account already exists in the target AD domain.</span></span> <span data-ttu-id="1b924-108">Tai reiškia, kad (1) vartotojas jau yra ir atitikimo ID žymės nepavyko vartotojui arba (2) UPN generavimo taisyklė sugeneravo nesuderinamą reikšmę.</span><span class="sxs-lookup"><span data-stu-id="1b924-108">This implies that either (1) the user already exists and the matching ID check failed for the user or (2) the UPN generation rule generated a conflicting value.</span></span>

<span data-ttu-id="1b924-109">Pateikiame siūlomus sprendimo veiksmus:</span><span class="sxs-lookup"><span data-stu-id="1b924-109">Here are the suggested resolution steps:</span></span>

<span data-ttu-id="1b924-110">Jei vartotojas jau yra, o atitikimo ID patikra nepavyko susieti darbo dienos paskyros su "Active Directory" paskyra, tada patikrinkite, ar atitikimo ID atributas (paprastai **darbuotojai**) tiek darbo dieną, tiek AD turi tikslią atitiktį.</span><span class="sxs-lookup"><span data-stu-id="1b924-110">If the user already exists and the matching ID check failed to link the Workday account to Active Directory account, then check if the matching ID attribute (typically **employeeID**) in both Workday and AD have an exact match.</span></span> <span data-ttu-id="1b924-111">Jei jie neturi atitikmens, tai yra duomenų problema, kurią reikia išspręsti.</span><span class="sxs-lookup"><span data-stu-id="1b924-111">If they don't have a match, it is a data issue that needs to be fixed.</span></span> <span data-ttu-id="1b924-112">Pavyzdžiui, jei "darbuotojai" yra "001052" ir skelbime ji yra 1052, tada parengimo modulis nepavyks susieti dviejų paskyrų ir bandys sukurti jau esamą vartotoją.</span><span class="sxs-lookup"><span data-stu-id="1b924-112">For example, if the EmployeeID in Workday is 001052 and in AD it is 1052, then the provisioning engine will fail to link the two accounts and will try to create a user that already exists.</span></span> <span data-ttu-id="1b924-113">Šiuo atveju sprendimas yra pakeisti **darbuotojai** reikšmę skelbime, kad būtų įtraukti nuliai, kad jis 001052.</span><span class="sxs-lookup"><span data-stu-id="1b924-113">The solution in this case is to change the **EmployeeID** value in AD to include the leading zeros to make it 001052.</span></span>
<span data-ttu-id="1b924-114">Jei "UPN" generuojama išraiška nesugeneruoja unikalios reikšmės, **Apsvarstykite galimybę naudoti funkciją de** -dubliavimo, kad kiekvieną kartą sukurtumėte unikalią reikšmę.</span><span class="sxs-lookup"><span data-stu-id="1b924-114">If the UPN-generating expression is not generating a unique value, consider using the de-duplication function **SelectUniqueValue** to generate a unique value each time.</span></span>

<span data-ttu-id="1b924-115">**Darbo dienos į skelbimų vartotojo parengimas nenustatė vadovo atributo reikšmė, skirta skelbimų vartotojo abonementui**</span><span class="sxs-lookup"><span data-stu-id="1b924-115">**Workday to AD User Provisioning does not set manager attribute value for AD user account**</span></span>

<span data-ttu-id="1b924-116">"WORKDAY to AD" vartotojo parengimo užduotis nėra parametro **vadovo** atributo reikšmė.</span><span class="sxs-lookup"><span data-stu-id="1b924-116">The Workday to AD User Provisioning job is not setting the **manager** attribute value for AD user accounts.</span></span> <span data-ttu-id="1b924-117">Yra du galimi scenarijai, kai šis elgesys yra matomas:</span><span class="sxs-lookup"><span data-stu-id="1b924-117">There are two possible scenarios when this behavior is seen:</span></span>

1. <span data-ttu-id="1b924-118">Darbo dienos tvarkytuvas negali būti išspręstas atitinkamam skelbimo vartotojo abonementui, nes vadovo nėra aprėpties.</span><span class="sxs-lookup"><span data-stu-id="1b924-118">The manager in Workday cannot be resolved to a corresponding AD User account because the manager is not in scope.</span></span>
2. <span data-ttu-id="1b924-119">**Kelių skelbimų domenų** scenarijuje, darbo dienos tvarkytuvas nėra tame pačiame domene kaip vartotojas.</span><span class="sxs-lookup"><span data-stu-id="1b924-119">In a **multiple AD domains** scenario, the manager in Workday is not present in the same domain as the user.</span></span>

<span data-ttu-id="1b924-120">Išbandykite šiuos veiksmus, kad išspręstumėte problemą:</span><span class="sxs-lookup"><span data-stu-id="1b924-120">Try these steps to resolve the issue:</span></span>

1. <span data-ttu-id="1b924-121">Jei nustatėte aprėpties filtrus, pirmiausia patikrinkite, ar tvarkytuvas yra aprėpties ir ar jis atitinka sąlygą aprėpties.</span><span class="sxs-lookup"><span data-stu-id="1b924-121">If you have defined scoping filters, first check if the manager is in scope and that it satisfies the scoping clause.</span></span> <span data-ttu-id="1b924-122">Jei vadovas neatitinka aprėpties filtro, pakeiskite filtrą taip, kad vadovas taip pat aprėptų parengimo operaciją.</span><span class="sxs-lookup"><span data-stu-id="1b924-122">If the manager does not satisfy the scoping filter, change the filter so that the manager is also in scope of the provisioning operation.</span></span>
2. <span data-ttu-id="1b924-123">Jei turite kelis skelbimų domenus, tada jungiamoji dalis turi žinomą nesugebėjimo išspręsti kelių domenų vadovo nuorodas apribojimą.</span><span class="sxs-lookup"><span data-stu-id="1b924-123">If you have multiple AD domains, then the connector has a known limitation of inability to resolve cross-domain manager references.</span></span>

<span data-ttu-id="1b924-124">Išsamesnės informacijos apie darbo dienos konfigūravimą automatiniam parengimas ieškokite straipsnyje [Susipažinkite: darbo dienos konfigūravimas automatiniam vartotojų parengimas](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial).</span><span class="sxs-lookup"><span data-stu-id="1b924-124">For more details on configuring workday for automated provisioning, see [Tutorial: Configure Workday for automatic user provisioning](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial).</span></span>













