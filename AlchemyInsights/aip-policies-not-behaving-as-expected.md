---
title: 'AIP: politika neelgiasi taip, kaip tikėtasi'
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002266"
- "4780"
ms.openlocfilehash: 0dfaae776ec551fe12919e8a8e69f2e7a58d67d0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47663197"
---
# <a name="aip-policies-not-behaving-as-expected"></a><span data-ttu-id="d1903-102">AIP: politika neelgiasi taip, kaip tikėtasi</span><span class="sxs-lookup"><span data-stu-id="d1903-102">AIP: Policies not behaving as expected</span></span>

<span data-ttu-id="d1903-103">"Azure" informacijos apsauga: strategijos, kurios nėra, kaip tikėtasi, ieškokite šioje rekomenduojamų rekomendacijų įvairiose politikos srityse:</span><span class="sxs-lookup"><span data-stu-id="d1903-103">Azure Information Protection: Policies not behaving as expected, see the following for recommended guidelines for various policy issues:</span></span>

1. <span data-ttu-id="d1903-104">Jei turite problemų su vaizdiniais ženklais, peržiūrėkite, [kai taikomi vizualiniai ženklai](https://docs.microsoft.com/azure/information-protection/configure-policy-markings#when-visual-markings-are-applied).</span><span class="sxs-lookup"><span data-stu-id="d1903-104">If you are having issues with visual markings, please review [When visual markings are applied](https://docs.microsoft.com/azure/information-protection/configure-policy-markings#when-visual-markings-are-applied).</span></span>
2. <span data-ttu-id="d1903-105">Jei kyla problemų dėl automatinio žymėjimo, peržiūrėkite, [kaip konfigūruoti automatines ir rekomenduojamas "Azure" informacijos apsaugos sąlygas](https://docs.microsoft.com/azure/information-protection/configure-policy-classification) ir [kokie atrodo slaptos informacijos tipai](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).</span><span class="sxs-lookup"><span data-stu-id="d1903-105">If you are having issues with automatic labeling, please review [How to configure conditions for automatic and recommended classification for Azure Information Protection](https://docs.microsoft.com/azure/information-protection/configure-policy-classification) and [What the sensitive information types look for](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).</span></span>
3. <span data-ttu-id="d1903-106">Jei kyla problemų su prigimtine/Pfile apsauga, peržiūrėkite [failų API konfigūraciją](https://docs.microsoft.com/azure/information-protection/develop/file-api-configuration).</span><span class="sxs-lookup"><span data-stu-id="d1903-106">If you are having issues with Native/Pfile protection, please review [File API configuration](https://docs.microsoft.com/azure/information-protection/develop/file-api-configuration).</span></span>
4. <span data-ttu-id="d1903-107">Patikrinkite, ar naudojate aprėpties strategijas, kurios netinkamai sukonfigūruotos: [kaip konfigūruoti "Azure" informacijos apsaugos strategiją konkretiems vartotojams naudojant aprėpties strategijas](https://docs.microsoft.com/azure/information-protection/configure-policy-scope).</span><span class="sxs-lookup"><span data-stu-id="d1903-107">Check if you are using scoped policies that aren't configured properly: [How to configure the Azure Information Protection policy for specific users by using scoped policies](https://docs.microsoft.com/azure/information-protection/configure-policy-scope).</span></span>
5. <span data-ttu-id="d1903-108">Jei prijungus pažymėtą dokumentą "Outlook" neveikia Automatinis žymėjimas, patikrinkite, ar "DRMEncryptProperty" neapibrėžta kaip aprašyta čia: [IRM registro parametrai, skirti saugos](https://docs.microsoft.com/deployoffice/security/protect-sensitive-messages-and-documents-by-using-irm-in-office#office-2016-irm-registry-key-options).</span><span class="sxs-lookup"><span data-stu-id="d1903-108">If automatic labeling isn't working for Outlook when attaching a labeled document, verify that DRMEncryptProperty isn't defined as described here: [IRM registry settings for security](https://docs.microsoft.com/deployoffice/security/protect-sensitive-messages-and-documents-by-using-irm-in-office#office-2016-irm-registry-key-options).</span></span>

<span data-ttu-id="d1903-109">Jei vis dar kyla problemų, surinkite "Azure" informacijos apsaugos kliento žurnalus ir pridėkite eksportuotus žurnalus su šiuo bilietu.</span><span class="sxs-lookup"><span data-stu-id="d1903-109">If you still are experiencing issues, please collect Azure Information Protection client logs and attach the exported logs to this ticket.</span></span>

1. <span data-ttu-id="d1903-110">Atidarykite "Office" dokumentą arba sukurkite naują laišką programoje "Outlook".</span><span class="sxs-lookup"><span data-stu-id="d1903-110">Open an Office document or create a new email in Outlook.</span></span>
2. <span data-ttu-id="d1903-111">Spustelėkite **apsaugoti/jautrumo**  >  **žinyną ir atsiliepimą**.</span><span class="sxs-lookup"><span data-stu-id="d1903-111">Click **Protect/Sensitivity** > **Help and feedback**.</span></span>
3. <span data-ttu-id="d1903-112">Spustelėkite **eksportuoti žurnalus**.</span><span class="sxs-lookup"><span data-stu-id="d1903-112">Click **Export Logs**.</span></span>
4. <span data-ttu-id="d1903-113">Įrašykite žurnalus į savo vietos pasirinkimą ir pridėkite juos prie šios paslaugos užklausos.</span><span class="sxs-lookup"><span data-stu-id="d1903-113">Save the logs to your choice of location, and attach them to this service request.</span></span>

<span data-ttu-id="d1903-114">Papildomi ištekliai:</span><span class="sxs-lookup"><span data-stu-id="d1903-114">Additional resources:</span></span>

- [<span data-ttu-id="d1903-115">Kaip sukonfigūruoti "Azure" informacijos apsaugos vaizdinio žymėjimo žymę</span><span class="sxs-lookup"><span data-stu-id="d1903-115">How to configure a label for visual markings for Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/configure-policy-markings)
- [<span data-ttu-id="d1903-116">"Azure" informacijos apsaugos dokumentų peržiūra</span><span class="sxs-lookup"><span data-stu-id="d1903-116">Review Azure Information Protection documentation</span></span>](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [<span data-ttu-id="d1903-117">"Microsoft 365" programėlių jautrumo žymių naudojimas</span><span class="sxs-lookup"><span data-stu-id="d1903-117">Use sensitivity labels in Microsoft 365 apps</span></span>](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels-office-apps)

