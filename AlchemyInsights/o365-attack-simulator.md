---
title: 2681 atakos simuliatorius programoje "Microsoft 365"
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
ms.openlocfilehash: dec96238c8438dcf9df176e3e3f20bd8a985b2cc
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47759227"
---
# <a name="attack-simulator-in-microsoft-365"></a><span data-ttu-id="af510-102">"Microsoft 365" atakos simuliatorius</span><span class="sxs-lookup"><span data-stu-id="af510-102">Attack Simulator in Microsoft 365</span></span>

- <span data-ttu-id="af510-103">Ar trūksta atakos treniruoklio?</span><span class="sxs-lookup"><span data-stu-id="af510-103">Are you missing Attack Simulator?</span></span> <span data-ttu-id="af510-104">Atakos treniruokliui reikia " **office 365" išplėstinės grėsmės apsaugos plano 2 (ATP planas 2)** arba " **Office 365 Enterprise E5**".</span><span class="sxs-lookup"><span data-stu-id="af510-104">Attack Simulator requires **Office 365 Advanced Threat Protection Plan 2 (ATP Plan 2)** or **Office 365 Enterprise E5**.</span></span> <span data-ttu-id="af510-105">Atakos simuliatorius **nėra** įtrauktas į "Office 365" išplėstinės grėsmės apsaugos planą 1 (ATP planas 1), "Office 365 Enterprise E3" arba bet kurias "Microsoft 365" taikomąsias programas verslui prenumeratos.</span><span class="sxs-lookup"><span data-stu-id="af510-105">Attack Simulator is **not** included in Office 365 Advanced Threat Protection Plan 1 (ATP Plan 1), Office 365 Enterprise E3, or any Microsoft 365 Apps for business subscriptions.</span></span>

- <span data-ttu-id="af510-106">Paskyrai, kurią naudojate norėdami inicijuoti modeliuojamoms atakoms, reikia visuotinių administratoriaus ar saugos administratoriaus teisių ir kelių dalių autentifikavimo (MFA).</span><span class="sxs-lookup"><span data-stu-id="af510-106">The account you use to launch simulated attacks requires global administrator or security administrator permissions and multi-factor authentication (MFA).</span></span> <span data-ttu-id="af510-107">Daugiau informacijos apie atakos imitatoriaus reikalavimus rasite [šioje temoje](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator).</span><span class="sxs-lookup"><span data-stu-id="af510-107">For more information about Attack Simulator requirements, see [this topic](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator).</span></span>

- <span data-ttu-id="af510-108">Svarbūs dalykai, kuriuos reikia žinoti apie **brute force slaptažodžio** atakos modeliavimą:</span><span class="sxs-lookup"><span data-stu-id="af510-108">Important things to know about **Brute Force Password** attack simulations:</span></span>

  - <span data-ttu-id="af510-109">Jei paskirties paskyroje įgalinta MFA ir slaptažodis buvo tinkamai atspėtas, paskyra nebus rodoma kaip pažeista (antrasis autentifikavimo faktorius bus neišsamus).</span><span class="sxs-lookup"><span data-stu-id="af510-109">If the target account has MFA enabled and the password was guessed correctly, the account will not show as compromised (the second authentication factor will be incomplete).</span></span>

  - <span data-ttu-id="af510-110">Slaptažodžio failas negali būti didesnis nei 10 MB.</span><span class="sxs-lookup"><span data-stu-id="af510-110">The password file can't be larger than 10 MB.</span></span> <span data-ttu-id="af510-111">Naudokite vieną slaptažodį eilutėje ir įtraukite tuščią eilutę (grįžties mygtuką) po paskutinio slaptažodžio sąraše.</span><span class="sxs-lookup"><span data-stu-id="af510-111">Use one password per line, and include a blank line (carriage return) after the last password in the list.</span></span>

- <span data-ttu-id="af510-112">Svarbūs dalykai, kuriuos reikia žinoti apie " **Spear phishing** " pridėti modeliavimų:</span><span class="sxs-lookup"><span data-stu-id="af510-112">Important things to know about **Spear Phishing** attach simulations:</span></span>

  - <span data-ttu-id="af510-113">Pagal dizainą negalite pateikti " **phishing" prisijungimo serverio URL**pasirinktinio reikšmės.</span><span class="sxs-lookup"><span data-stu-id="af510-113">By design, you can't provide a custom value for **Phishing login server URL**.</span></span>

  - <span data-ttu-id="af510-114">Jei gavėjas naudoja [ataskaitos pranešimo priedą įgalinti](https://docs.microsoft.com/microsoft-365/security/office-365-security/enable-the-report-message-add-in) , kad pranešimas būtų praneštas kaip sukčiavimas apsimetant, galite negauti pranešimo įspėjimų (nes tai sumodeliuotas išpuolis).</span><span class="sxs-lookup"><span data-stu-id="af510-114">If a recipient uses the [Enable the Report Message add-in](https://docs.microsoft.com/microsoft-365/security/office-365-security/enable-the-report-message-add-in) to report the message as phishing, you might not receive alerts for the message (because this is a simulated attack).</span></span>

- <span data-ttu-id="af510-115">Ataskaitos: po modeliuojamos atakos, galite spustelėti **atakuoti informaciją** , kad matytumėte ataskaitą.</span><span class="sxs-lookup"><span data-stu-id="af510-115">Reports: After the simulated attack is complete, you can click **Attack Details** to see the report.</span></span>

- <span data-ttu-id="af510-116">Išsamių instrukcijų ir naujų funkcijų atakos simuliatoriuje ieškokite ["Microsoft 365" atakos simuliatorius](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator).</span><span class="sxs-lookup"><span data-stu-id="af510-116">For detailed instructions and new features in Attack Simulator, see [Attack Simulator in Microsoft 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator).</span></span>
