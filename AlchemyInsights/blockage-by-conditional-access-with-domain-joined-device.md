---
title: Gaunu blokuojamą sąlyginę prieigą su domeno sujungtu įrenginiu
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/20/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9834"
- "9003257"
ms.openlocfilehash: 052311ffe71bcb65de2b5c2a964932b1fb99c373
ms.sourcegitcommit: c34ba92e19419dcb2d251b8a1afe4d180a939617
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 03/20/2021
ms.locfileid: "51036702"
---
# <a name="im-getting-blocked-by-conditional-access-with-domain-joined-device"></a><span data-ttu-id="e051e-102">Gaunu blokuojamą sąlyginę prieigą su domeno sujungtu įrenginiu</span><span class="sxs-lookup"><span data-stu-id="e051e-102">I’m getting blocked by Conditional Access with domain joined device</span></span>

<span data-ttu-id="e051e-103">**Labai Rekomenduojami įrankiai**</span><span class="sxs-lookup"><span data-stu-id="e051e-103">**Highly Recommended Tools**</span></span>

<span data-ttu-id="e051e-104">[Įrenginių registravimo trikčių diagnostikos priemonė](https://docs.microsoft.com/samples/azure-samples/dsregtool/dsregtool/) – įrankis, padedantis pašalinti dažniausiai pasitaikančių įrenginių registravimo triktis.</span><span class="sxs-lookup"><span data-stu-id="e051e-104">[Device Registration Troubleshooter Tool](https://docs.microsoft.com/samples/azure-samples/dsregtool/dsregtool/) - The tool that helps in troubleshooting the most common device registration issues.</span></span>

<span data-ttu-id="e051e-105">[Patikrinkite įrenginio registracijos ryšio scenarijų](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/) – scenarijų, kuris padeda užtikrinti, kad įrenginys galėtų pasiekti įrenginio registracijos pabaigos taškus po sistemos abonementu.</span><span class="sxs-lookup"><span data-stu-id="e051e-105">[Test Device Registration Connectivity script](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/) - The script that helps ensuring that a device can access Device Registration endpoints under the system account.</span></span>

<span data-ttu-id="e051e-106">" [Azure AD" įrenginio valymo scenarijus](https://github.com/mzmaili/AzureADDeviceCleanup) – scenarijus, leidžiantis ieškoti ir valdyti "pasenusių apsikeitimo" įrenginius savo aplinkoje.</span><span class="sxs-lookup"><span data-stu-id="e051e-106">[Azure AD Device Cleanup Script](https://github.com/mzmaili/AzureADDeviceCleanup) - The script that enables you to seek and manage stale devices in your environment.</span></span>

<span data-ttu-id="e051e-107">Štai kelios dažniausios priežastys, kodėl sąlyginiai "Access" gali būti nepavykę įrenginio, kuris prisijungė prie domeno (hibridinio "Azure AD").</span><span class="sxs-lookup"><span data-stu-id="e051e-107">Here are some common reasons why conditional access may be failing a device that has joined a domain (Hybrid Azure AD).</span></span>

1. <span data-ttu-id="e051e-108">**Įrenginyje nėra "AZURE ad PRT"** – reikia įsitikinti, kad įrenginyje yra "Azure AD" pirminis atnaujinimo atpažinimo ženklas (PRT).</span><span class="sxs-lookup"><span data-stu-id="e051e-108">**There’s no Azure AD PRT on the device** - You need to ensure that the device has Azure AD Primary Refresh Token (PRT).</span></span> <span data-ttu-id="e051e-109">Daugiau informacijos apie PRT ieškokite šiame [dokumente](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token).</span><span class="sxs-lookup"><span data-stu-id="e051e-109">For more information about PRT, see this [document](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token).</span></span>

<span data-ttu-id="e051e-110">Norėdami patikrinti, ar turite "Azure AD PRT", galite vykdyti `dsregcmd/status` įrenginio komandą ir patikrinti, ar "AzureAdPrt" yra lygu "Yes".</span><span class="sxs-lookup"><span data-stu-id="e051e-110">To verify if you have Azure AD PRT, you can run `dsregcmd/status` command on the device and verify if “AzureAdPrt” equals “YES”.</span></span>

<span data-ttu-id="e051e-111">Jei "AzureAdPrt" yra "ne", patikrinkite šiuos dalykus:</span><span class="sxs-lookup"><span data-stu-id="e051e-111">If "AzureAdPrt" is "NO", check the following:</span></span>

- <span data-ttu-id="e051e-112">**Nesvarbu, ar turite išorinės aplinkos su AD FS ir yra nepasiekiamas iš vartotojų namų tinklo**: šiuo atveju įsitikinkite, kad jūsų "usernamemixed" pabaigos taškai pasiekiami iš ekstraneto.</span><span class="sxs-lookup"><span data-stu-id="e051e-112">**Whether you have a federated environment with AD FS, and it’s unreachable from your users’ home networks**: In this case, ensure that your "usernamemixed" endpoints are accessible from the extranet.</span></span> <span data-ttu-id="e051e-113">Jei AD FS yra už VPN, pasirūpinkite, kad vartotojai prisijungtų prie VPN ir iš naujo prisijungtų prie įrenginio.</span><span class="sxs-lookup"><span data-stu-id="e051e-113">If your AD FS is behind a VPN, ensure that the users connect to the VPN and re-login to the device.</span></span> <span data-ttu-id="e051e-114">Daugiau informacijos ieškokite šiame [dokumente](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-federated-domains).</span><span class="sxs-lookup"><span data-stu-id="e051e-114">For more information, see this [document](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-federated-domains).</span></span>

- <span data-ttu-id="e051e-115">**Ar įrenginio TPM yra klaidingas ir todėl negali autentifikuoti įrenginio**: pažymėkite "TPM. msc", kad pamatytumėte, ar TPM būsena yra "paruošta".</span><span class="sxs-lookup"><span data-stu-id="e051e-115">**Whether the device’s TPM is faulty and thus cannot authenticate the device**: Check "tpm.msc" to see if the state of TPM is "Ready".</span></span> <span data-ttu-id="e051e-116">Jei ne, paleiskite `dsregcmd/leave` ir paleiskite įrenginį iš naujo prisijungti prie "AZURE AD".</span><span class="sxs-lookup"><span data-stu-id="e051e-116">If not, run `dsregcmd/leave` and let the device re-join to Azure AD.</span></span> <span data-ttu-id="e051e-117">Tada bandykite dar kartą.</span><span class="sxs-lookup"><span data-stu-id="e051e-117">Then, try again.</span></span> <span data-ttu-id="e051e-118">Daugiau informacijos ieškokite šiame [dokumente](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state).</span><span class="sxs-lookup"><span data-stu-id="e051e-118">For more information, see this [document](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state).</span></span>

- <span data-ttu-id="e051e-119">Naudojate **trečiosios šalies tapatybės teikėją, nepalaikantį WS-Trust protokolo**.</span><span class="sxs-lookup"><span data-stu-id="e051e-119">**You’re using a 3rd party identity provider, which does not support WS-Trust protocol**.</span></span> <span data-ttu-id="e051e-120">Kaip aprašyta mūsų dokumentuose, hibridiniai "Azure AD" įrenginiai šiuo atveju neveikia.</span><span class="sxs-lookup"><span data-stu-id="e051e-120">As described in our docs, hybrid Azure AD-joined devices cannot work in this case.</span></span> <span data-ttu-id="e051e-121">Susisiekite su savo tapatybės teikėju.</span><span class="sxs-lookup"><span data-stu-id="e051e-121">Please work with your Identity provider for support.</span></span>

2. <span data-ttu-id="e051e-122">**Vartotojai naudoja "Chrome" naršyklę be "Windows 10" paskyrų** arba " **Office" plėtinio "Chrome" automatiškai nenaudoja "pag" ar "Hybrid-AAD" įrenginių. "Windows"**, kuri yra su įrenginiu susietos sąlyginės prieigos strategijos, rodomas klaidos pranešimas "neregistruotasis įrenginys".</span><span class="sxs-lookup"><span data-stu-id="e051e-122">**Users are using Chrome browser without the Windows 10 Accounts** or **Office extension Chrome does not automatically use the PRT on AAD-joined or hybrid-AAD-joined devices**: This leads to failure of any device-based Conditional Access policies, with “Unregistered device” error message displayed.</span></span> <span data-ttu-id="e051e-123">Jei norite tinkamai naudoti "Chrome" naršyklę, turite įdiegti "Windows 10" paskyras arba "Office" plėtinį vartotojų "Chrome" naršyklėje per SCCM arba Intune.</span><span class="sxs-lookup"><span data-stu-id="e051e-123">To use Chrome browser correctly, you must install the “Windows 10 Accounts” or "Office extension to the users’ Chrome browser" via SCCM or Intune.</span></span> <span data-ttu-id="e051e-124">Daugiau informacijos ieškokite šiame [dokumente](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-conditions#chrome-support).</span><span class="sxs-lookup"><span data-stu-id="e051e-124">For more information, see this [document](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-conditions#chrome-support).</span></span>

<span data-ttu-id="e051e-125">Jei negalima išplėsti plėtinio nuotoliniu būdu, praneškite vartotojams rankiniu būdu įdiegti vieną iš aukščiau nurodytų plėtinių, kad būtų galima pasiekti taikomąsias programas už įrenginių pagrindu veikiančią sąlyginę prieigą.</span><span class="sxs-lookup"><span data-stu-id="e051e-125">If it’s not possible to push the extension remotely, notify users to manually install one of the above extensions to access applications behind device-based Conditional Access.</span></span> <span data-ttu-id="e051e-126">Daugiau informacijos ieškokite šiame [dokumente](https://docs.microsoft.com/azure/active-directory/conditional-access/require-managed-devices#prerequisites).</span><span class="sxs-lookup"><span data-stu-id="e051e-126">For more information, see this [document](https://docs.microsoft.com/azure/active-directory/conditional-access/require-managed-devices#prerequisites).</span></span>

3. <span data-ttu-id="e051e-127">**Įrenginys buvo tinkamai hibridinio "AZURE AD", bet jis buvo netyčia panaikintas arba išjungtas dėl sinchronizavimo pasikeitimų "AZURE AD Connect" arba "Azure" portale**: jei taip nutinka, įrenginio objektas nebėra atpažįstamas kaip visiškai sujungtas įrenginys, nors "Azureadsujungtos" ir "PRT" būsena rodoma kaip tinkama įrenginyje.</span><span class="sxs-lookup"><span data-stu-id="e051e-127">**The device was correctly hybrid Azure AD joined, but it was inadvertently deleted or disabled, either due to sync changes in Azure AD Connect or from the Azure portal**: If this happens, the device object is no longer recognized as a fully joined device even though the "AzureAdJoined" and "PRT" status show up as valid on the device.</span></span>

<span data-ttu-id="e051e-128">Norėdami išspręsti šią problemą, paleiskite `dsregcmd/leave` paveiktus įrenginius ir leisti jiems vėl prisijungti prie "AZURE AD".</span><span class="sxs-lookup"><span data-stu-id="e051e-128">To fix this issue, run `dsregcmd/leave` on the affected devices and let them rejoin Azure AD.</span></span> <span data-ttu-id="e051e-129">Daugiau informacijos ieškokite šiame [dokumente](https://docs.microsoft.com/azure/active-directory/devices/faq#q-why-do-my-users-see-an-error-message-saying-your-organization-has-deleted-the-device-or-your-organization-has-disabled-the-device-on-their-windows-10-devices).</span><span class="sxs-lookup"><span data-stu-id="e051e-129">For more information, see this [document](https://docs.microsoft.com/azure/active-directory/devices/faq#q-why-do-my-users-see-an-error-message-saying-your-organization-has-deleted-the-device-or-your-organization-has-disabled-the-device-on-their-windows-10-devices).</span></span>

> [!NOTE]
> <span data-ttu-id="e051e-130">Jei jūsų įrenginiai yra "Windows 10", "1809" naujinime, naudodami VPN/debesies tarpinį serverį ir matysite problemas "AzureAdPrt" arba bet kurią taikomąją programą su SSO problema ("Outlook" nesusijungia su pašto dėžute, net jei turėjote "PRT"), įsitikinkite, kad turite šį pataisos [KB4554354](https://support.microsoft.com/topic/march-30-2020-kb4554354-os-build-17763-1132-deaba49b-4b29-55b9-caee-3e2d87dd75a2) arba balandžio kaupiamojo naujinimo [KB4549949](https://support.microsoft.com/topic/april-14-2020-kb4549949-os-build-17763-1158-76d9a3af-b20b-8996-bd4d-7b50c505fda6) , kad išvengtumėte šių mašinų PRT gedimų</span><span class="sxs-lookup"><span data-stu-id="e051e-130">If your devices are on Windows 10, 1809 update, with VPN/Cloud Proxy and see issues with "AzureAdPrt" state or any app with SSO problem (outlook not connecting to mailbox even though you had PRT), ensure you have this patch [KB4554354](https://support.microsoft.com/topic/march-30-2020-kb4554354-os-build-17763-1132-deaba49b-4b29-55b9-caee-3e2d87dd75a2) or April cumulative update [KB4549949](https://support.microsoft.com/topic/april-14-2020-kb4549949-os-build-17763-1158-76d9a3af-b20b-8996-bd4d-7b50c505fda6) to prevent PRT failures on those machines.</span></span>

















