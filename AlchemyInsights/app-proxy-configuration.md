---
title: Taikomosios programos tarpinio serverio konfigūracija
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004356"
- "7800"
ms.openlocfilehash: 0b782705afa8eab338687590baff90de4e17ccb9
ms.sourcegitcommit: 83fe2a8d060794fdf58445b469b30a3294b7a9b6
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 01/15/2021
ms.locfileid: "49885521"
---
# <a name="app-proxy-configuration"></a><span data-ttu-id="251d4-102">Taikomosios programos tarpinio serverio konfigūracija</span><span class="sxs-lookup"><span data-stu-id="251d4-102">App Proxy Configuration</span></span>

1. <span data-ttu-id="251d4-103">Norėdami sužinoti, kaip konfigūruoti taikomosios programos tarpinio serverio taikomąją programą "Azure AD", kad savo vietines taikomąsias programas būtų galima atskleisti debesyje, Sužinokite, [kaip sukonfigūruoti taikomosios programos tarpinio serverio taikomąją programą](https://docs.microsoft.com/azure/active-directory/application-proxy-config-how-to).</span><span class="sxs-lookup"><span data-stu-id="251d4-103">To understand how to configure an Application Proxy application within Azure AD to expose your on-premises applications to the cloud, see [How to configure an Application Proxy application](https://docs.microsoft.com/azure/active-directory/application-proxy-config-how-to).</span></span>
2. <span data-ttu-id="251d4-104">Bendroji autentifikacija (SSO) leidžia vartotojams pasiekti taikomąją programą neautentifikuojant kelių kartų.</span><span class="sxs-lookup"><span data-stu-id="251d4-104">Single sign-on (SSO) allows your users to access an application without authenticating multiple times.</span></span> <span data-ttu-id="251d4-105">Jis leidžia vienam autentifikavimui įvykti debesyje, prieš "Azure Active Directory", ir leidžia tarnybai arba jungčiai apsimokite vartotoju, kad būtų galima atlikti papildomas autentifikavimo problemas iš taikomosios programos.</span><span class="sxs-lookup"><span data-stu-id="251d4-105">It allows the single authentication to occur in the cloud, against Azure Active Directory, and allows the service or Connector to impersonate the user to complete any additional authentication challenges from the application.</span></span> <span data-ttu-id="251d4-106">Norėdami sužinoti daugiau, Sužinokite, [kaip konfigūruoti bendrąją autentifikacija taikomosios programos tarpinio serverio taikomajai programai](https://docs.microsoft.com/azure/active-directory/application-proxy-config-sso-how-to).</span><span class="sxs-lookup"><span data-stu-id="251d4-106">To learn more, see [How to configure single sign-on to an Application Proxy application](https://docs.microsoft.com/azure/active-directory/application-proxy-config-sso-how-to).</span></span>
3. <span data-ttu-id="251d4-107">Naudokite [šį straipsnį](https://docs.microsoft.com/azure/active-directory/application-proxy-config-problem) , kad išspręstumėte įprastas problemas, su kuriomis susiduria žmonės kurdami naują taikomosios programos tarpinio serverio taikomąją programą.</span><span class="sxs-lookup"><span data-stu-id="251d4-107">Use [this article](https://docs.microsoft.com/azure/active-directory/application-proxy-config-problem) to troubleshoot common issues people face when creating a new application proxy application.</span></span>
4. <span data-ttu-id="251d4-108">Jei kyla problemų nustatant back-end autentifikavimą taikomojoje programoje, gali reikėti [Šalinti tarpinio serverio "Kerberos" įgaliojimų perdavimo konfigūracijas](https://docs.microsoft.com/azure/active-directory/application-proxy-back-end-kerberos-constrained-delegation-how-to) arba stebėti [taikomosios programos konfigūravimą su "pingaccess](https://docs.microsoft.com/azure/active-directory/application-proxy-back-end-ping-access-how-to) ", kad išspręstumėte problemą.</span><span class="sxs-lookup"><span data-stu-id="251d4-108">If you are having a problem setting up back-end authentication to your application you may need to [Troubleshoot Kerberos constrained delegation configurations for Application Proxy](https://docs.microsoft.com/azure/active-directory/application-proxy-back-end-kerberos-constrained-delegation-how-to) or follow guidance on [configuring application with PingAccess](https://docs.microsoft.com/azure/active-directory/application-proxy-back-end-ping-access-how-to) to resolve your issue.</span></span>
