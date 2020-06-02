---
title: 'AIP: Politika neveikia taip, kaip tikėtasi'
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002266"
- "4780"
ms.openlocfilehash: 7926ff9ebbd54969fb5b3ae5d909baffe96a4292
ms.sourcegitcommit: 2afad0b107d03cd8c4de0b85b5bee38a13a7960d
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 05/26/2020
ms.locfileid: "44493161"
---
# <a name="aip-policies-not-behaving-as-expected"></a><span data-ttu-id="82309-102">AIP: Politika neveikia taip, kaip tikėtasi</span><span class="sxs-lookup"><span data-stu-id="82309-102">AIP: Policies not behaving as expected</span></span>

<span data-ttu-id="82309-103">Azure informacijos apsauga: strategijos neveikia kaip tikėtasi, ieškokite rekomenduojamų gairių įvairių strategijos problemų:</span><span class="sxs-lookup"><span data-stu-id="82309-103">Azure Information Protection: Policies not behaving as expected, see the following for recommended guidelines for various policy issues:</span></span>

1. <span data-ttu-id="82309-104">Jei kyla problemų dėl vaizdinių ženklų, peržiūrėkite [Kai taikomi vaizdiniai ženklai](https://docs.microsoft.com/azure/information-protection/configure-policy-markings#when-visual-markings-are-applied).</span><span class="sxs-lookup"><span data-stu-id="82309-104">If you are having issues with visual markings, please review [When visual markings are applied](https://docs.microsoft.com/azure/information-protection/configure-policy-markings#when-visual-markings-are-applied).</span></span>
2. <span data-ttu-id="82309-105">Jei kyla problemų dėl automatinio ženklinimo, peržiūrėkite [Kaip konfigūruoti automatinio ir rekomenduojamo "Azure" informacijos apsaugos ir](https://docs.microsoft.com/azure/information-protection/configure-policy-classification) ["What the sensitive information types" klasifikavimo](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)sąlygas .</span><span class="sxs-lookup"><span data-stu-id="82309-105">If you are having issues with automatic labeling, please review [How to configure conditions for automatic and recommended classification for Azure Information Protection](https://docs.microsoft.com/azure/information-protection/configure-policy-classification) and [What the sensitive information types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for).</span></span>
3. <span data-ttu-id="82309-106">Jei kyla problemų dėl apsaugos nuo vietinio / Pfailo, peržiūrėkite [failo API konfigūraciją](https://docs.microsoft.com/azure/information-protection/develop/file-api-configuration).</span><span class="sxs-lookup"><span data-stu-id="82309-106">If you are having issues with Native/Pfile protection, please review [File API configuration](https://docs.microsoft.com/azure/information-protection/develop/file-api-configuration).</span></span>
4. <span data-ttu-id="82309-107">Patikrinkite, ar naudojate aprėpties strategijas, kurios nėra tinkamai sukonfigūruotos: [kaip konfigūruoti konkrečių vartotojų Azure informacijos apsaugos strategiją naudojant aprėpties strategijas](https://docs.microsoft.com/azure/information-protection/configure-policy-scope).</span><span class="sxs-lookup"><span data-stu-id="82309-107">Check if you are using scoped policies that aren't configured properly: [How to configure the Azure Information Protection policy for specific users by using scoped policies](https://docs.microsoft.com/azure/information-protection/configure-policy-scope).</span></span>
5. <span data-ttu-id="82309-108">Jei automatinis žymėjimas neveikia programoje "Outlook" pridedant pažymėtą dokumentą, patikrinkite, ar DRMEncryptProperty nėra apibrėžta kaip aprašyta čia: [IRM registro parametrus saugos](https://docs.microsoft.com/deployoffice/security/protect-sensitive-messages-and-documents-by-using-irm-in-office#office-2016-irm-registry-key-options).</span><span class="sxs-lookup"><span data-stu-id="82309-108">If automatic labeling isn't working for Outlook when attaching a labeled document, verify that DRMEncryptProperty isn't defined as described here: [IRM registry settings for security](https://docs.microsoft.com/deployoffice/security/protect-sensitive-messages-and-documents-by-using-irm-in-office#office-2016-irm-registry-key-options).</span></span>

<span data-ttu-id="82309-109">Jei vis tiek kyla problemų, rinkkite "Azure" informacijos apsaugos kliento žurnalus ir pridėkite eksportuotus žurnalus prie šio bilieto.</span><span class="sxs-lookup"><span data-stu-id="82309-109">If you still are experiencing issues, please collect Azure Information Protection client logs and attach the exported logs to this ticket.</span></span>

1. <span data-ttu-id="82309-110">Atidarykite "Office" dokumentą arba sukurkite naują el. laišką programoje "Outlook".</span><span class="sxs-lookup"><span data-stu-id="82309-110">Open an Office document or create a new email in Outlook.</span></span>
2. <span data-ttu-id="82309-111">Spustelėkite **Apsaugoti / jautrumas**  >  **Žinynas ir atsiliepimai**.</span><span class="sxs-lookup"><span data-stu-id="82309-111">Click **Protect/Sensitivity** > **Help and feedback**.</span></span>
3. <span data-ttu-id="82309-112">Spustelėkite **Eksportuoti žurnalus**.</span><span class="sxs-lookup"><span data-stu-id="82309-112">Click **Export Logs**.</span></span>
4. <span data-ttu-id="82309-113">Įrašykite žurnalus į savo vietą ir pridėkite juos prie šios tarnybos užklausos.</span><span class="sxs-lookup"><span data-stu-id="82309-113">Save the logs to your choice of location, and attach them to this service request.</span></span>

<span data-ttu-id="82309-114">Papildomi ištekliai:</span><span class="sxs-lookup"><span data-stu-id="82309-114">Additional resources:</span></span>

- [<span data-ttu-id="82309-115">Kaip sukonfigūruoti žymę visual pažymi Azure informacijos apsauga</span><span class="sxs-lookup"><span data-stu-id="82309-115">How to configure a label for visual markings for Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/configure-policy-markings)
- [<span data-ttu-id="82309-116">"Azure" informacijos apsaugos dokumentų peržiūra</span><span class="sxs-lookup"><span data-stu-id="82309-116">Review Azure Information Protection documentation</span></span>](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [<span data-ttu-id="82309-117">Jautrumo etikečių naudojimas "Office" programose</span><span class="sxs-lookup"><span data-stu-id="82309-117">Use sensitivity labels in Office apps</span></span>](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels-office-apps)

