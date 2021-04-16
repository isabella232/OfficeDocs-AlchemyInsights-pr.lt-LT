---
title: Norite pažymėti domeną arba el. pašto siuntėją saugiai?
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002921"
- "5673"
ms.openlocfilehash: a1c4c4d2fadaf75eda9b5b322aca35c32dfee8ea
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 04/15/2021
ms.locfileid: "51792140"
---
# <a name="need-to-mark-a-domain-or-email-sender-safe"></a><span data-ttu-id="eb6fe-102">Norite pažymėti domeną arba el. pašto siuntėją saugiai?</span><span class="sxs-lookup"><span data-stu-id="eb6fe-102">Need to mark a domain or email sender safe?</span></span>

- <span data-ttu-id="eb6fe-103">Patikimų **siuntėjų sąrašų naudoti nerekomenduojama,** nes ji atveria jūsų organizacijai pašto šiukšlių, sukčiavimo apsimetant ir apsimetimo atakomis.</span><span class="sxs-lookup"><span data-stu-id="eb6fe-103">Use of **safe sender lists is not recommended** since it opens up your organization to spam, phish, and spoofing attacks.</span></span>
- <span data-ttu-id="eb6fe-104">Tačiau, jei yra verslo reikalavimas, rekomenduojame **šiam atvejui** **[naudoti pašto](https://docs.microsoft.com/microsoft-365/security/office-365-security/create-safe-sender-lists-in-office-365?view=o365-worldwide#recommended-use-mail-flow-rules)** srauto taisykles.</span><span class="sxs-lookup"><span data-stu-id="eb6fe-104">However, if there is a business requirement, we **recommend** using **[Mail Flow Rules](https://docs.microsoft.com/microsoft-365/security/office-365-security/create-safe-sender-lists-in-office-365?view=o365-worldwide#recommended-use-mail-flow-rules)** for this.</span></span> <span data-ttu-id="eb6fe-105">Mūsų rekomendacijos užtikrina siuntėjo autentifikavimą (patikrina, ar siuntimo domenas nėra apgaulių).</span><span class="sxs-lookup"><span data-stu-id="eb6fe-105">Our guidance ensures sender authentication (verifies sending domain is not being spoofed).</span></span> <span data-ttu-id="eb6fe-106">**Pastaba:** nerekomenduojame valdyti klaidingų teigiamų rezultatų naudojant patikimų siuntėjų sąrašus, nes pašto šiukšlių filtravimo išimtys gali atidaryti jūsų organizaciją saugos atakoms.</span><span class="sxs-lookup"><span data-stu-id="eb6fe-106">**Note**: We don't recommend managing false positives by using safe sender lists, because exceptions to spam filtering can open your organization to security attacks.</span></span> <span data-ttu-id="eb6fe-107">Jei jūsų vartotojas (-ai) gauna laiškus, netinkamai pažymėtus kaip pašto šiukšlės arba nepageidaujamas el. paštas, **[praneškite apie pranešimus ir failus "Microsoft".](https://protection.office.com/reportsubmission)**</span><span class="sxs-lookup"><span data-stu-id="eb6fe-107">If your user(s) receive messages incorrectly marked as spam or junk email, please **[Report messages and files to Microsoft](https://protection.office.com/reportsubmission)**.</span></span>
- <span data-ttu-id="eb6fe-108">Patikimų siuntėjų programoje "Outlook", Leidžiamų siuntėjų sąraše  arba leidžiamų domenų sąraše apsaugos nuo pašto šiukšlių strategijose reikėtų vengti, nes siuntėjai apeina visus pašto šiukšles, apsimetimo apsimetant ir siuntėjų autentifikavimą (SPF, DKIM, DMARC).</span><span class="sxs-lookup"><span data-stu-id="eb6fe-108">Safe Senders in Outlook, Allowed sender list, or allowed domain list in anti-spam policies **should be avoided** because senders bypass all spam, spoof, and phish protection, and sender authentication (SPF, DKIM, DMARC).</span></span> <span data-ttu-id="eb6fe-109">Šis metodas geriausiai naudojamas tik laikinajam testavimui.</span><span class="sxs-lookup"><span data-stu-id="eb6fe-109">This method is best used for temporary testing only.</span></span>
