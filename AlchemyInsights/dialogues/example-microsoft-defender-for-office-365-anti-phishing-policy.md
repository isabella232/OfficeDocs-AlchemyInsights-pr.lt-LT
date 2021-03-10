---
title: "\"Microsoft Defender\", skirtas \"Office 365\" apsaugos nuo sukčiavimo apsimetant strategijai"
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: eabff70c22b641627d3ab6c0b2f8846a0be2f49e
ms.sourcegitcommit: 60c504f3ac187eaf1141b3ba701d9e0633bdd968
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 03/08/2021
ms.locfileid: "50695635"
---
# <a name="example-microsoft-defender-for-office-365-anti-phishing-policy"></a><span data-ttu-id="f4910-102">"Microsoft Defender", skirtas "Office 365" apsaugos nuo sukčiavimo apsimetant strategijai</span><span class="sxs-lookup"><span data-stu-id="f4910-102">Example Microsoft Defender for Office 365 anti-phishing policy</span></span>

<span data-ttu-id="f4910-103">Šie parametrai įgalina strategiją, vadinamą *domenu ir generaliniu direktoriumi*.</span><span class="sxs-lookup"><span data-stu-id="f4910-103">These settings enable a policy called *Domain and CEO*.</span></span> <span data-ttu-id="f4910-104">Ši strategija suteikia ir vartotojo, ir domeno apsaugą nuo apsimetimas ir tada taiko strategiją visiems pašto vartotojams, kuriuos gavo domenas.</span><span class="sxs-lookup"><span data-stu-id="f4910-104">This policy provides both user and domain protection from impersonation and then applies the policy to all email received by users within the domain.</span></span> <span data-ttu-id="f4910-105">Pirmiausia įtraukite šią informaciją, kad sukurtumėte strategiją:</span><span class="sxs-lookup"><span data-stu-id="f4910-105">First, add the following information to create the policy:</span></span>

- <span data-ttu-id="f4910-106">**Pavadinimas**: domain ir CEO **Description**: užtikrina, kad generalinis direktorius ir jūsų domenas nebus apsimečiami.</span><span class="sxs-lookup"><span data-stu-id="f4910-106">**Name**: Domain and CEO **Description**: Ensures that the CEO and your domain are not being impersonated.</span></span>
  <span data-ttu-id="f4910-107">**Pritaikyta**: pasirinkite **gavėjo domeną**.</span><span class="sxs-lookup"><span data-stu-id="f4910-107">**Applied to**: Select **The recipient domain is**.</span></span> <span data-ttu-id="f4910-108">Dalyje **bet kurį iš šių** pasirinkite **pasirinkti**, tada pasirinkite domeną.</span><span class="sxs-lookup"><span data-stu-id="f4910-108">Under **Any of these**, select **Choose**, and then select a domain.</span></span> <span data-ttu-id="f4910-109">Pasirinkite **+ įtraukti**.</span><span class="sxs-lookup"><span data-stu-id="f4910-109">Select **+ Add**.</span></span> <span data-ttu-id="f4910-110">Pažymėkite žymės langelį, esantį prie domeno vardo sąraše (pvz., *contoso.com*), tada pasirinkite **įtraukti**.</span><span class="sxs-lookup"><span data-stu-id="f4910-110">Select the check box next to the name of the domain in the list (for example, *contoso.com*), and then select **Add**.</span></span> <span data-ttu-id="f4910-111">Pasirinkite **atlikta**.</span><span class="sxs-lookup"><span data-stu-id="f4910-111">Select **Done**.</span></span>
- <span data-ttu-id="f4910-112">Kai strategija bus sukurta, galite pakoreguoti strategiją naudodami šias parinktis:</span><span class="sxs-lookup"><span data-stu-id="f4910-112">After the policy is created, you can fine-tune the policy by using the following options:</span></span>
  - <span data-ttu-id="f4910-113">**Vartotojų įtraukimas į apsaugą:** Šiame pavyzdyje, bent minimaliai įtraukite generalinio direktoriaus elektroninio pašto adresą.</span><span class="sxs-lookup"><span data-stu-id="f4910-113">**Add users to protect:** For this example, add the CEO's email address, at a minimum.</span></span>
  - <span data-ttu-id="f4910-114">**Įtraukite domenus, kad apsaugotumėte**: įtraukite organizacijos domeną, kuriame yra generalinio direktoriaus biuras.</span><span class="sxs-lookup"><span data-stu-id="f4910-114">**Add domains to protect**: Add the organizational domain that includes the office of the CEO.</span></span>
  - <span data-ttu-id="f4910-115">**Pasirinkite veiksmai**: **Jei laišką siunčia apsimestas vartotojas**, pasirinkite **Peradresuoti pranešimą į kitą elektroninio pašto adresą**, tada įveskite saugos administratoriaus el. pašto adresą (pvz., *securityadmin@contoso.com*).</span><span class="sxs-lookup"><span data-stu-id="f4910-115">**Choose actions**: For **If email is sent by an impersonated user**, select **Redirect message to another email address**, and then enter the email address of the security administrator (for example, *securityadmin@contoso.com*).</span></span> <span data-ttu-id="f4910-116">**Jei el. laišką siunčia apsimestas domenas**, pasirinkite **sulaikyti pranešimą**.</span><span class="sxs-lookup"><span data-stu-id="f4910-116">For **If email is sent by an impersonated domain**, select **Quarantine the message**.</span></span>
  - <span data-ttu-id="f4910-117">**Pašto dėžutės informacijos**: pagal numatytuosius nustatymą Ši parinktis pažymėta, kai kuriate naują apsaugos nuo sukčiavimo apsimetant strategiją.</span><span class="sxs-lookup"><span data-stu-id="f4910-117">**Mailbox intelligence**: By default, this option is selected when you create a new anti-phishing policy.</span></span> <span data-ttu-id="f4910-118">Palikite **šį parametrą,** kad būtų pasiekti Geriausi rezultatai.</span><span class="sxs-lookup"><span data-stu-id="f4910-118">Leave this setting **On** for best results.</span></span>
  - <span data-ttu-id="f4910-119">**Patikimų siuntėjų ir domenų įtraukimas:** Šiame pavyzdyje negalima apibrėžti jokių perrašymų.</span><span class="sxs-lookup"><span data-stu-id="f4910-119">**Add trusted senders and domains:** For this example, don't define any overrides.</span></span>
- <span data-ttu-id="f4910-120">Peržiūrėjus parametrus, pasirinkite **Kurti šią strategiją** arba **įrašyti**, jei reikia.</span><span class="sxs-lookup"><span data-stu-id="f4910-120">Once you've reviewed your settings, select **Create this policy** or **Save**, as appropriate.</span></span>

<span data-ttu-id="f4910-121">Norėdami sužinoti daugiau, peržiūrėkite [apsaugos nuo sukčiavimo apsimetant strategijas programoje "Microsoft 365"](https://go.microsoft.com/fwlink/?linkid=2092235).</span><span class="sxs-lookup"><span data-stu-id="f4910-121">To learn more, see [Anti-phishing policies in Microsoft 365](https://go.microsoft.com/fwlink/?linkid=2092235).</span></span>
