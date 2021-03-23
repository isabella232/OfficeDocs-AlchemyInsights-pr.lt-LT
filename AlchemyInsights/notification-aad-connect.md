---
title: Pranešimas "AAD Connect"
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
- "9003245"
- "9326"
ms.openlocfilehash: 832c9dd587cb023b5b1d87e905acb123df34237f
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 03/19/2021
ms.locfileid: "51036107"
---
# <a name="notification-aad-connect"></a><span data-ttu-id="df574-102">Pranešimas "AAD Connect"</span><span class="sxs-lookup"><span data-stu-id="df574-102">Notification AAD Connect</span></span>

- <span data-ttu-id="df574-103">Įsitikinkite, kad turite teisę atlikti veiksmą.</span><span class="sxs-lookup"><span data-stu-id="df574-103">Ensure you are authorized to perform the operation.</span></span> <span data-ttu-id="df574-104">Visuotiniai administratoriai turi prieigą pagal numatytuosius numatytuosius.</span><span class="sxs-lookup"><span data-stu-id="df574-104">Global Admins have access by default.</span></span> <span data-ttu-id="df574-105">Be to, galite naudoti [vaidmenimis pagrįstą prieigos valdymą](https://docs.microsoft.com/azure/active-directory/connect-health/active-directory-aadconnect-health-operations) , kad galėtumėte perduoti registravimo teisę bendraautoriui.</span><span class="sxs-lookup"><span data-stu-id="df574-105">Additionally, you can use [Role Based Access Control](https://docs.microsoft.com/azure/active-directory/connect-health/active-directory-aadconnect-health-operations) to delegate registration permission to Contributor.</span></span>
- <span data-ttu-id="df574-106">Užtikrinkite, kad būtini galiniai punktai yra įgalinti ir Neblokuojami dėl užkardos.</span><span class="sxs-lookup"><span data-stu-id="df574-106">Ensure the required endpoints are enabled, and not blocked due to firewall.</span></span> <span data-ttu-id="df574-107">Išsamesnės informacijos ieškokite [reikalavimai](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-agent-install).</span><span class="sxs-lookup"><span data-stu-id="df574-107">For details, see [requirements](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-agent-install).</span></span>
- <span data-ttu-id="df574-108">Registracija gali nepavykti dėl išeinančio ryšio su tinklo lygiu atliekama SSL patikra.</span><span class="sxs-lookup"><span data-stu-id="df574-108">Registration can fail due to outbound communication being subjected to SSL inspection by the network layer.</span></span>
- <span data-ttu-id="df574-109">Įsitikinkite, kad patikrinote "Azure AD Connect Health" pranešimų parametrus ir peržiūrite savo parametrą.</span><span class="sxs-lookup"><span data-stu-id="df574-109">Make sure you have verified the notification settings for Azure AD Connect Health and review your setting.</span></span> <span data-ttu-id="df574-110">Norėdami sužinoti, kaip konfigūruoti pranešimų parametrus, skirtus "Azure AD Connect Health" pranešimams, Peržiūrėkite šį [vadovą](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-operations).</span><span class="sxs-lookup"><span data-stu-id="df574-110">To understand how to configure the notification settings for Azure AD Connect Health notifications, see this [guide](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-operations).</span></span>
- <span data-ttu-id="df574-111">Norėdami sužinoti daugiau apie "AAD Connect Health" sinchronizavimo ataskaitą ir kaip ją atsisiųsti, žiūrėkite [objekto lygio sinchronizavimo ataskaita](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-sync).</span><span class="sxs-lookup"><span data-stu-id="df574-111">To learn more about the AAD Connect Health sync report and how to download it, see [Object level synchronization report](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-sync).</span></span>

<span data-ttu-id="df574-112">Norėdami pašalinti "AAD Connect Health" įspėjimus, vadovaukitės [trikčių diagnostikos vadovu, kad galėtumėte susisiekti su sveikatos duomenų šviežumo įspėjimais](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-data-freshness) ir dažnai užduodamais klausimais, skaitykite [bendrosios "AAD Connect Health" klausimai](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-health-faq).</span><span class="sxs-lookup"><span data-stu-id="df574-112">To troubleshoot AAD Connect Health Alerts follow [the troubleshooting guide for AAD Connect Health data freshness alerts](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-data-freshness) and for commonly asked questions, see [Common AAD Connect Health installation questions](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-health-faq).</span></span>
