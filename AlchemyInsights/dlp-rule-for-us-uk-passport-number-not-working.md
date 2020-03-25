---
title: Neveikia JAV / JUNGTINĖS Karalystės paso numerio DLP taisyklė
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1319"
- "3200001"
ms.assetid: fc178b8b-943b-4346-a2bd-a75c6af6f80f
ms.openlocfilehash: c63e814059c897531109aa78725e9811b311fb27
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 03/24/2020
ms.locfileid: "42931270"
---
# <a name="problems-with-dlp---usuk-passport-numbers"></a><span data-ttu-id="31d5e-102">Problemos su DLP - JAV / JK pasų numeriai</span><span class="sxs-lookup"><span data-stu-id="31d5e-102">Problems with DLP - US/UK passport numbers</span></span>

<span data-ttu-id="31d5e-103">**Svarbu:** daugelis "SharePoint Online" ir "OneDrive" klientų vykdo verslui svarbias taikomąsias programas pagal fone vykdomą tarnybą.</span><span class="sxs-lookup"><span data-stu-id="31d5e-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="31d5e-104">Tai apima turinio perkėlimą, duomenų praradimo prevenciją (DLP) ir atsarginių kopijų kūrimo sprendimus.</span><span class="sxs-lookup"><span data-stu-id="31d5e-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="31d5e-105">Šiais precedento neturinčiais laikais imamės veiksmų, kad užtikrintume, jog "SharePoint Online" ir "OneDrive" paslaugos būtų labai prieinamos ir patikimos jūsų vartotojams, kurie labiau nei bet kada priklauso nuo paslaugos nuotoliniuose darbo scenarijuose.</span><span class="sxs-lookup"><span data-stu-id="31d5e-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="31d5e-106">Siekdami šio tikslo, darbo dienos valandomis įdiegėme griežtesnius buferizavimo apribojimus fonines programas (migraciją, DLP ir atsarginius sprendimus).</span><span class="sxs-lookup"><span data-stu-id="31d5e-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="31d5e-107">Turėtumėte tikėtis, kad šios programos pasieks labai ribotą pralaidumą šiais laikais.</span><span class="sxs-lookup"><span data-stu-id="31d5e-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="31d5e-108">Tačiau regiono vakaro ir savaitgalio valandomis paslauga bus paruošta apdoroti žymiai didesnį užklausų iš foninių programų apimtį.</span><span class="sxs-lookup"><span data-stu-id="31d5e-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="31d5e-109">**DLP problemos su JAV / JK pasų numeriais**</span><span class="sxs-lookup"><span data-stu-id="31d5e-109">**DLP issues with US/UK passport numbers**</span></span>

<span data-ttu-id="31d5e-110">Ar turite problemų su **duomenų praradimo prevencija (DLP)** neveikia turinio, kuriame yra **JAV / JK paso numerį,** kai naudojate DLP slaptos informacijos tipą O365?</span><span class="sxs-lookup"><span data-stu-id="31d5e-110">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **US/UK passport number** when using a DLP sensitive information type in O365?</span></span> <span data-ttu-id="31d5e-111">Jei taip, įsitikinkite, kad jūsų turinyje yra reikiama informacija, kurios ieškote, kai ji vertinama.</span><span class="sxs-lookup"><span data-stu-id="31d5e-111">If so, make sure your content contains the needed information for what the DLP policy is looking for when it is evaluated.</span></span>
  
<span data-ttu-id="31d5e-112">Pvz., **JAV ir Jungtinės Karalystės paso numerio** strategija, sukonfigūruota 75 % patikimumo lygiu, įvertinami toliau nurodyti duomenys, kuriuos reikia aptikti, kad taisyklė būtų suaktyvinta</span><span class="sxs-lookup"><span data-stu-id="31d5e-112">For example, for a **US/UK passport number** policy configured with a confidence level of 75%, the following are evaluated and must be detected for the rule to trigger</span></span>
  
- <span data-ttu-id="31d5e-113">**[Formatas:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** Devyni skaitmenys</span><span class="sxs-lookup"><span data-stu-id="31d5e-113">**[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** Nine digits</span></span>

- <span data-ttu-id="31d5e-114">**[Raštas:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** Devyni skaitmenys iš eilės</span><span class="sxs-lookup"><span data-stu-id="31d5e-114">**[Pattern:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** Nine consecutive digits</span></span>

- <span data-ttu-id="31d5e-115">**[Kontrolinė suma:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** Ne, nėra kontrolinės sumos</span><span class="sxs-lookup"><span data-stu-id="31d5e-115">**[Checksum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** No, there is no Checksum</span></span>

- <span data-ttu-id="31d5e-116">**[Apibrėžimas:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-77)** DLP strategija yra 75% įsitikinusi, kad ji aptiko tokio tipo slaptą informaciją, jei 300 simbolių atstumu:</span><span class="sxs-lookup"><span data-stu-id="31d5e-116">**[Definition:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-77)** A DLP policy is 75% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span>

  - <span data-ttu-id="31d5e-117">Funkcija Func_usa_uk_passport randa šabloną atitinkantį turinį.</span><span class="sxs-lookup"><span data-stu-id="31d5e-117">The function Func_usa_uk_passport finds content that matches the pattern.</span></span>

  - <span data-ttu-id="31d5e-118">Rastas raktinis žodis iš Keyword_passport.</span><span class="sxs-lookup"><span data-stu-id="31d5e-118">A keyword from Keyword_passport is found.</span></span>

    <span data-ttu-id="31d5e-119">Pvz., šis pavyzdys būtų sukelti **JAV ir Jungtinės Karalystės paso numerio** politika: JAV paso numeris 123456789</span><span class="sxs-lookup"><span data-stu-id="31d5e-119">For example, the following sample would trigger for the **US/UK passport number** policy: U.S. Passport number 123456789</span></span>

<span data-ttu-id="31d5e-120">Daugiau informacijos apie tai, ko reikia, kad jūsų turiniui būtų aptiktas JAV/ JUNGTINĖS Karalystės paso numeris, ieškokite šiame šio straipsnio skyriuje: [Kas slaptos informacijos tipai ieško JAV / JUNGTINĖS Karalystės paso numerio](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us--uk-passport-number)</span><span class="sxs-lookup"><span data-stu-id="31d5e-120">For more information on what is required for a US/UK Passport Number to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for US/UK Passport Number](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us--uk-passport-number)</span></span>
  
<span data-ttu-id="31d5e-121">Naudodami kitą įtaisytąjį slaptą informacijos tipą, informacijos apie tai, ko reikia kitiems tipams: [ko ieško slaptos informacijos tipai, ieškokite](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for) šiame straipsnyje</span><span class="sxs-lookup"><span data-stu-id="31d5e-121">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span></span>
  