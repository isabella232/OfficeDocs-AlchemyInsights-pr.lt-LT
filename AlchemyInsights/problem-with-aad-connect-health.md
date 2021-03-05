---
title: "\"AAD Connect Health\" problema"
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004649"
- "8427"
ms.openlocfilehash: f5624069a2e96fde8aed08965ca6b753f3aad1e8
ms.sourcegitcommit: 5763fedfd5dd459249c81cdbb4af34181a757bd5
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 03/04/2021
ms.locfileid: "50482071"
---
# <a name="problem-with-aad-connect-health"></a><span data-ttu-id="47aab-102">"AAD Connect Health" problema</span><span class="sxs-lookup"><span data-stu-id="47aab-102">Problem with AAD Connect Health</span></span>

- <span data-ttu-id="47aab-103">Įsitikinkite, kad turite teisę atlikti veiksmą.</span><span class="sxs-lookup"><span data-stu-id="47aab-103">Ensure you are authorized to perform the operation.</span></span> <span data-ttu-id="47aab-104">Visuotiniai administratoriai turi prieigą pagal numatytuosius numatytuosius.</span><span class="sxs-lookup"><span data-stu-id="47aab-104">Global Admins have access by default.</span></span> <span data-ttu-id="47aab-105">Be to, galite naudoti [vaidmenimis pagrįstą prieigos valdymą](https://docs.microsoft.com/azure/active-directory/connect-health/active-directory-aadconnect-health-operations) , kad galėtumėte perduoti registravimo teisę bendraautoriui.</span><span class="sxs-lookup"><span data-stu-id="47aab-105">Additionally, you can use [Role Based Access Control](https://docs.microsoft.com/azure/active-directory/connect-health/active-directory-aadconnect-health-operations) to delegate registration permission to Contributor.</span></span>
- <span data-ttu-id="47aab-106">Užtikrinkite, kad būtini galiniai punktai yra įgalinti ir Neblokuojami dėl užkardos.</span><span class="sxs-lookup"><span data-stu-id="47aab-106">Ensure the required endpoints are enabled, and not blocked due to firewall.</span></span> <span data-ttu-id="47aab-107">Išsamesnės informacijos ieškokite [reikalavimai](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-agent-install).</span><span class="sxs-lookup"><span data-stu-id="47aab-107">For details, see [requirements](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-agent-install).</span></span>
- <span data-ttu-id="47aab-108">Registracija gali nepavykti dėl išeinančio ryšio su tinklo lygiu atliekama SSL patikra.</span><span class="sxs-lookup"><span data-stu-id="47aab-108">Registration can fail due to outbound communication being subjected to SSL inspection by the network layer.</span></span>
- <span data-ttu-id="47aab-109">Įsitikinkite, kad patikrinote "Azure AD Connect Health" pranešimų parametrus.</span><span class="sxs-lookup"><span data-stu-id="47aab-109">Make sure you have verified the notification settings for Azure AD Connect Health.</span></span> <span data-ttu-id="47aab-110">Peržiūrėkite savo parametrą.</span><span class="sxs-lookup"><span data-stu-id="47aab-110">Please review your setting.</span></span> <span data-ttu-id="47aab-111">Šis [vadovas](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-operations) gali padėti suprasti, kaip konfigūruoti pranešimų parametrus "Azure AD Connect Health" pranešimuose.</span><span class="sxs-lookup"><span data-stu-id="47aab-111">This [guide](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-operations) can help you understand how to configure the notification settings for Azure AD Connect health notifications.</span></span>
- <span data-ttu-id="47aab-112">Norėdami sužinoti daugiau apie "AAD Connect Health" sinchronizavimo ataskaitą ir kaip ją atsisiųsti, žiūrėkite [objekto lygio sinchronizavimo ataskaita](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-sync).</span><span class="sxs-lookup"><span data-stu-id="47aab-112">To learn more about the AAD Connect Health sync report and how to download it, see [Object level synchronization report](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-sync).</span></span>

<span data-ttu-id="47aab-113">Norėdami pašalinti "AAD Connect Health" įspėjimus, vadovaukitės [trikčių diagnostikos vadovu, kad galėtumėte susisiekti su sveikatos duomenų šviežumo įspėjimais](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-data-freshness) ir dažniausiai užduodamais klausimais, skaitykite [bendrosios "AAD Connect Health" klausimai](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-health-faq).</span><span class="sxs-lookup"><span data-stu-id="47aab-113">To troubleshoot AAD Connect Health alerts, follow [the troubleshooting guide for AAD Connect Health data freshness alerts](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-data-freshness) and for commonly asked questions, see [Common AAD Connect Health installation questions](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-health-faq).</span></span>
