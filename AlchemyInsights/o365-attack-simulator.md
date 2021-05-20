---
title: 2681 attack Simulator in Microsoft 365
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "2681"
ms.assetid: ''
ms.openlocfilehash: e7d71fdb77b4a047c1998e9aba75cdd469a936a8
ms.sourcegitcommit: f4866e94918c7b591ad0cd3b58169d340bcc7f00
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 05/19/2021
ms.locfileid: "52545734"
---
# <a name="attack-simulator-in-microsoft-365"></a><span data-ttu-id="e6027-102">Attack Simulator in Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="e6027-102">Attack Simulator in Microsoft 365</span></span>

- <span data-ttu-id="e6027-103">Ar jums trūksta atakos simuliatoriaus?</span><span class="sxs-lookup"><span data-stu-id="e6027-103">Are you missing Attack Simulator?</span></span> <span data-ttu-id="e6027-104">"Attack Simulator" **reikia "Microsoft" sargybos Office 365 2 arba** **Office 365 Enterprise E5.**</span><span class="sxs-lookup"><span data-stu-id="e6027-104">Attack Simulator requires **Microsoft Defender for Office 365 Plan 2** or **Office 365 Enterprise E5**.</span></span> <span data-ttu-id="e6027-105">Atakos **simuliatorius** neįtrauktas į "Microsoft" sargybą, Office 365 1 planą, "Office 365 Enterprise E3" arba "Microsoft 365" programos verslui prenumeratas.</span><span class="sxs-lookup"><span data-stu-id="e6027-105">Attack Simulator is **not** included in Microsoft Defender for Office 365 Plan 1, Office 365 Enterprise E3, or any Microsoft 365 Apps for business subscriptions.</span></span>

- <span data-ttu-id="e6027-106">Paskyrai, kurią naudojate imituoties atakoms paleisti, reikia visuotinio administratoriaus arba saugos administratoriaus teisių ir kelių dalių autentifikavimo (MFA).</span><span class="sxs-lookup"><span data-stu-id="e6027-106">The account you use to launch simulated attacks requires global administrator or security administrator permissions and multi-factor authentication (MFA).</span></span> <span data-ttu-id="e6027-107">Daugiau informacijos apie atakos simuliatoriaus reikalavimus žr. [šioje temoje](/microsoft-365/security/office-365-security/attack-simulator).</span><span class="sxs-lookup"><span data-stu-id="e6027-107">For more information about Attack Simulator requirements, see [this topic](/microsoft-365/security/office-365-security/attack-simulator).</span></span>

- <span data-ttu-id="e6027-108">Svarbūs dalykai, kuriuos reikia žinoti apie **"Brute Force Password"** atakos modeliavimą:</span><span class="sxs-lookup"><span data-stu-id="e6027-108">Important things to know about **Brute Force Password** attack simulations:</span></span>

  - <span data-ttu-id="e6027-109">Jei paskirties paskyroje įgalintas MFA ir slaptažodis buvo atspėjamas tinkamai, paskyra nebus rodoma kaip pažeista (antrasis autentifikavimo koeficientas bus neišsamus).</span><span class="sxs-lookup"><span data-stu-id="e6027-109">If the target account has MFA enabled and the password was guessed correctly, the account will not show as compromised (the second authentication factor will be incomplete).</span></span>

  - <span data-ttu-id="e6027-110">Slaptažodžio failas negali būti didesnis nei 10 MB.</span><span class="sxs-lookup"><span data-stu-id="e6027-110">The password file can't be larger than 10 MB.</span></span> <span data-ttu-id="e6027-111">Naudokite vieną slaptažodį vienoje eilutėje ir įtraukite tuščią eilutę (gabenimo grąžinimą) po paskutinio sąrašo slaptažodžio.</span><span class="sxs-lookup"><span data-stu-id="e6027-111">Use one password per line, and include a blank line (carriage return) after the last password in the list.</span></span>

- <span data-ttu-id="e6027-112">Svarbūs dalykai, kuriuos reikia žinoti apie **sukčiavimo apsimetant pridėjimo** modeliavimą:</span><span class="sxs-lookup"><span data-stu-id="e6027-112">Important things to know about **Spear Phishing** attach simulations:</span></span>

  - <span data-ttu-id="e6027-113">Pagal dizainą negalite pateikti pasirinktinės reikšmės apsimestinių duomenų **registravimosi serverio URL.**</span><span class="sxs-lookup"><span data-stu-id="e6027-113">By design, you can't provide a custom value for **Phishing login server URL**.</span></span>

  - <span data-ttu-id="e6027-114">Jei gavėjas [](/microsoft-365/security/office-365-security/enable-the-report-message-add-in) naudoja ataskaitos pranešimo papildinyje įgalinti pranešimą kaip sukčiavimą apsimetant, galite negauti įspėjimų apie pranešimą (nes tai yra imituota ataka).</span><span class="sxs-lookup"><span data-stu-id="e6027-114">If a recipient uses the [Enable the Report Message add-in](/microsoft-365/security/office-365-security/enable-the-report-message-add-in) to report the message as phishing, you might not receive alerts for the message (because this is a simulated attack).</span></span>

- <span data-ttu-id="e6027-115">Ataskaitos: kai imituota ataka bus baigta, galite spustelėti **Atakos išsami informacija,** kad pamatytumėte ataskaitą.</span><span class="sxs-lookup"><span data-stu-id="e6027-115">Reports: After the simulated attack is complete, you can click **Attack Details** to see the report.</span></span>

- <span data-ttu-id="e6027-116">Išsamias instrukcijas ir naujas "Attack Simulator" funkcijas žr. [Atakos simuliatorius Microsoft 365](/microsoft-365/security/office-365-security/attack-simulator).</span><span class="sxs-lookup"><span data-stu-id="e6027-116">For detailed instructions and new features in Attack Simulator, see [Attack Simulator in Microsoft 365](/microsoft-365/security/office-365-security/attack-simulator).</span></span>
