---
title: Norite, kad domenas arba pašto siuntėjas būtų saugūs?
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
- "9002921"
- "5673"
ms.openlocfilehash: 0ea089b95ad7de25e77017196fb2db895d4d0178
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 09/15/2020
ms.locfileid: "47803253"
---
# <a name="need-to-mark-a-domain-or-email-sender-safe"></a><span data-ttu-id="6598c-102">Norite, kad domenas arba pašto siuntėjas būtų saugūs?</span><span class="sxs-lookup"><span data-stu-id="6598c-102">Need to mark a domain or email sender safe?</span></span>

- <span data-ttu-id="6598c-103">**Saugių siuntėjų sąrašų naudojimas nerekomenduojamas** , nes jis atveria jūsų organizacijai pašto šiukšlių, apsimetimo ir imitavimo atakų.</span><span class="sxs-lookup"><span data-stu-id="6598c-103">Use of **safe sender lists is not recommended** since it opens up your organization to spam, phish, and spoofing attacks.</span></span>
- <span data-ttu-id="6598c-104">Tačiau, jei yra verslo reikalavimas, **rekomenduojame** naudoti " **[mail Flow" taisykles](https://docs.microsoft.com/microsoft-365/security/office-365-security/create-safe-sender-lists-in-office-365?view=o365-worldwide#recommended-use-mail-flow-rules)** .</span><span class="sxs-lookup"><span data-stu-id="6598c-104">However, if there is a business requirement, we **recommend** using **[Mail Flow Rules](https://docs.microsoft.com/microsoft-365/security/office-365-security/create-safe-sender-lists-in-office-365?view=o365-worldwide#recommended-use-mail-flow-rules)** for this.</span></span> <span data-ttu-id="6598c-105">Mūsų rekomendacijos užtikrina siuntėjo autentifikavimą (tikrina, ar siuntimo domenas nėra apsimetimo).</span><span class="sxs-lookup"><span data-stu-id="6598c-105">Our guidance ensures sender authentication (verifies sending domain is not being spoofed).</span></span> <span data-ttu-id="6598c-106">**Pastaba**: nerekomenduojame naudoti neteisingus teigiamus rezultatus naudojant patikimų siuntėjų sąrašus, nes išimtys pašto šiukšlių filtrui gali atidaryti jūsų organizaciją į saugos atakas.</span><span class="sxs-lookup"><span data-stu-id="6598c-106">**Note**: We don't recommend managing false positives by using safe sender lists, because exceptions to spam filtering can open your organization to security attacks.</span></span> <span data-ttu-id="6598c-107">Jei jūsų vartotojas (-iai) gauna laiškus, netinkamai pažymėtus kaip pašto šiukšles arba nepageidaujamą paštą, praneškite **[apie laiškus ir failus "Microsoft"](https://protection.office.com/reportsubmission)**.</span><span class="sxs-lookup"><span data-stu-id="6598c-107">If your user(s) receive messages incorrectly marked as spam or junk email, please **[Report messages and files to Microsoft](https://protection.office.com/reportsubmission)**.</span></span>
- <span data-ttu-id="6598c-108">**Reikia vengti** patikimų siuntėjų programoje "Outlook", leidžiančio siuntėjų sąrašo arba leidžiamo domenų sąrašo apsaugos nuo pašto šiukšlių politikoje, nes siuntėjai apeina visus pašto šiukšlių, apgaulingas ir pašto apsaugos bei siuntėjo autentifikavimo (SPF, DKIM, DMARC).</span><span class="sxs-lookup"><span data-stu-id="6598c-108">Safe Senders in Outlook, Allowed sender list, or allowed domain list in anti-spam policies **should be avoided** because senders bypass all spam, spoof, and phish protection, and sender authentication (SPF, DKIM, DMARC).</span></span> <span data-ttu-id="6598c-109">Šis metodas geriausiai tinka tik laikiniesiems bandymams.</span><span class="sxs-lookup"><span data-stu-id="6598c-109">This method is best used for temporary testing only.</span></span>
