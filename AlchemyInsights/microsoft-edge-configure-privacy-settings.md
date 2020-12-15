---
title: "\"Microsoft Edge\" Konfigūruokite privatumo parametrus"
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003843"
- "6892"
ms.openlocfilehash: dcd1d91dcde1f585caf0e1e3af30946513a0f26c
ms.sourcegitcommit: 94036315916fbc79dca2a692c2e9bc1139dd28f6
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 12/08/2020
ms.locfileid: "49677796"
---
# <a name="microsoft-edge-configure-privacy-settings"></a><span data-ttu-id="90b17-102">"Microsoft Edge" Konfigūruokite privatumo parametrus</span><span class="sxs-lookup"><span data-stu-id="90b17-102">Microsoft Edge configure privacy settings</span></span>

<span data-ttu-id="90b17-103">Pagal numatytuosius, jei "Microsoft Edge" įdiegta ne "Windows" platformose, diagnostikos duomenys ir svetainės informacija nesiunčiami "Microsoft".</span><span class="sxs-lookup"><span data-stu-id="90b17-103">By default, if Microsoft Edge is deployed on non-Windows platforms, diagnostic data and site information are not sent to Microsoft.</span></span> <span data-ttu-id="90b17-104">Tačiau jei "Microsoft Edge" įdiegta "Windows 10", diagnostikos duomenys ir svetainės informacija siunčiami pagal vartotojų " [Windows" diagnostikos duomenų parametrus](https://docs.microsoft.com/windows/privacy/configure-windows-diagnostic-data-in-your-organization).</span><span class="sxs-lookup"><span data-stu-id="90b17-104">However, if Microsoft Edge is deployed on Windows 10, diagnostic data and site information are sent according to users' [Windows Diagnostic data settings](https://docs.microsoft.com/windows/privacy/configure-windows-diagnostic-data-in-your-organization).</span></span>

<span data-ttu-id="90b17-105">Norėdami konfigūruoti, kaip "Microsoft Edge" apdoroja jūsų organizacijos duomenų rinkimą, naudokite šias grupių strategijas:</span><span class="sxs-lookup"><span data-stu-id="90b17-105">To configure how Microsoft Edge handles data collection for your organization, use the following group policies:</span></span>
- <span data-ttu-id="90b17-106">[Metricsreportingenabled](https://docs.microsoft.com/DeployEdge/microsoft-edge-policies#metricsreportingenabled): Ši strategija įgalina ataskaitų apie naudojimą ir su gedimais susijusius duomenis.</span><span class="sxs-lookup"><span data-stu-id="90b17-106">[MetricsReportingEnabled](https://docs.microsoft.com/DeployEdge/microsoft-edge-policies#metricsreportingenabled): This policy enables reporting of usage and crash-related data.</span></span>
- <span data-ttu-id="90b17-107">[Sendsiteinfotoimproveserspaustuvai](https://docs.microsoft.com/DeployEdge/microsoft-edge-policies#sendsiteinfotoimproveservices): Ši strategija siunčia svetainės informaciją, kuri naudojama "Microsoft" paslaugoms tobulinti.</span><span class="sxs-lookup"><span data-stu-id="90b17-107">[SendSiteInfoToImproveServices](https://docs.microsoft.com/DeployEdge/microsoft-edge-policies#sendsiteinfotoimproveservices): This policy sends site information that is used to improve Microsoft services.</span></span>

<span data-ttu-id="90b17-108">Norėdami sužinoti daugiau, peržiūrėkite [strategijos parametrų konfigūravimas](https://docs.microsoft.com/deployedge/microsoft-edge-enterprise-privacy-settings#configure-policy-settings).</span><span class="sxs-lookup"><span data-stu-id="90b17-108">To learn more, see [Configure policy settings](https://docs.microsoft.com/deployedge/microsoft-edge-enterprise-privacy-settings#configure-policy-settings).</span></span>