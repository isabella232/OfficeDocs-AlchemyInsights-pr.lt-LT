---
title: Tarnybos jungties taško (SCP) konfigūravimas
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/17/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9732"
- "9003244"
ms.openlocfilehash: 9d733a1a0a3b8d92bdd5477a8978b6fbeede9653
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 03/19/2021
ms.locfileid: "51036146"
---
# <a name="configure-service-connection-point-scp"></a><span data-ttu-id="9101e-102">Tarnybos jungties taško (SCP) konfigūravimas</span><span class="sxs-lookup"><span data-stu-id="9101e-102">Configure Service connection Point (SCP)</span></span>

<span data-ttu-id="9101e-103">**DSREG_AUTOJOIN_ADCONFIG_READ_FAILED (0x801c001d/-2145648611)**</span><span class="sxs-lookup"><span data-stu-id="9101e-103">**DSREG_AUTOJOIN_ADCONFIG_READ_FAILED (0x801c001d/-2145648611)**</span></span>

- <span data-ttu-id="9101e-104">**Priežastis**: nepavyko perskaityti SCP objekto ir gauti "Azure AD" nuomotojo informaciją</span><span class="sxs-lookup"><span data-stu-id="9101e-104">**Reason**: Unable to read the SCP object and get the Azure AD tenant information</span></span>
- <span data-ttu-id="9101e-105">**Skiriamoji geba**: ieškokite skyriaus [tarnybos kreipties taško konfigūravimas](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-federated-domains#configure-hybrid-azure-ad-join)</span><span class="sxs-lookup"><span data-stu-id="9101e-105">**Resolution**: Refer to the section [Configure a Service Connection Point](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-federated-domains#configure-hybrid-azure-ad-join)</span></span>


<span data-ttu-id="9101e-106">**Veiksmų planas**</span><span class="sxs-lookup"><span data-stu-id="9101e-106">**Action plan**</span></span>

- <span data-ttu-id="9101e-107">Patikrinkite, ar įrenginys gavo GPO, skirtą valdomam patvirtinimui.</span><span class="sxs-lookup"><span data-stu-id="9101e-107">Check whether the device has received the GPO for the controlled validation.</span></span>
- <span data-ttu-id="9101e-108">Įsitikinkite, kad GPO sukūrė registro raktus.</span><span class="sxs-lookup"><span data-stu-id="9101e-108">Ensure that the GPO has created the registry keys.</span></span>
- <span data-ttu-id="9101e-109">Įsitikinkite, kad turite 2 raktus, sukurtus naudojant katalogo ID ir "onmicrosoft domain".</span><span class="sxs-lookup"><span data-stu-id="9101e-109">Ensure that you have 2 keys created with your Directory ID and onmicrosoft domain.</span></span>

<span data-ttu-id="9101e-110">**Konfigūruoti kliento pusės registro parametrą, skirtą "SCP"**</span><span class="sxs-lookup"><span data-stu-id="9101e-110">**Configure client-side registry setting for SCP**</span></span>

<span data-ttu-id="9101e-111">Naudokite toliau pateiktą pavyzdį, kad sukurtumėte grupės strategijos objektą (GPO), kad galėtumėte įdiegti registro parametrą, kuris konfigūruoja SCP įrašą jūsų įrenginių registre.</span><span class="sxs-lookup"><span data-stu-id="9101e-111">Use the following example to create a Group Policy Object (GPO) to deploy a registry setting that configures an SCP entry in the registry of your devices.</span></span>

1. <span data-ttu-id="9101e-112">Atidarykite grupės strategijos valdymo konsolę ir sukurkite naują GPO savo domene.</span><span class="sxs-lookup"><span data-stu-id="9101e-112">Open a Group Policy Management console and create a new GPO in your domain.</span></span>
     - <span data-ttu-id="9101e-113">Pateikite naujai sukurtą GPO vardą (pvz., ClientSideSCP)</span><span class="sxs-lookup"><span data-stu-id="9101e-113">Provide your newly created GPO a name (for example, ClientSideSCP)</span></span>

2. <span data-ttu-id="9101e-114">Redaguoti GPO ir rasti šį kelią: **kompiuterio konfigūracija > nuostatos > "Windows" parametrų > registrą**.</span><span class="sxs-lookup"><span data-stu-id="9101e-114">Edit the GPO and locate the following path: **Computer Configuration > Preferences > Windows Settings > Registry**.</span></span>

3. <span data-ttu-id="9101e-115">Dešiniuoju pelės mygtuku spustelėkite **registrą** ir pasirinkite **naujas > registro elementą**.</span><span class="sxs-lookup"><span data-stu-id="9101e-115">Right-click on **Registry** and select **New > Registry Item**.</span></span>

4. <span data-ttu-id="9101e-116">Skirtuke **Bendrasis** Konfigūruokite šiuos dalykus:</span><span class="sxs-lookup"><span data-stu-id="9101e-116">On the **General** tab, configure the following:</span></span>
  
- <span data-ttu-id="9101e-117">**Veiksmas**: naujinimas</span><span class="sxs-lookup"><span data-stu-id="9101e-117">**Action**: Update</span></span>
    
- <span data-ttu-id="9101e-118">**Avilys**: HKEY_LOCAL_MACHINE</span><span class="sxs-lookup"><span data-stu-id="9101e-118">**Hive**: HKEY_LOCAL_MACHINE</span></span>
    
- <span data-ttu-id="9101e-119">**Rakto Path**: Software\microsoft\windows\currentversion\cdj\aad</span><span class="sxs-lookup"><span data-stu-id="9101e-119">**Key Path**: SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD</span></span>
    
- <span data-ttu-id="9101e-120">**Reikšmės pavadinimas**: tenantid</span><span class="sxs-lookup"><span data-stu-id="9101e-120">**Value name**: TenantId</span></span>
    
- <span data-ttu-id="9101e-121">**Reikšmės tipas**: REG_SZ</span><span class="sxs-lookup"><span data-stu-id="9101e-121">**Value type**: REG_SZ</span></span>
    
- <span data-ttu-id="9101e-122">**Reikšmės duomenys**: "Azure AD" egzemplioriaus GUID arba katalogo ID (šią reikšmę galima rasti "Azure" **portale > "Azure Active Directory" > ypatybių > katalogo ID**)</span><span class="sxs-lookup"><span data-stu-id="9101e-122">**Value data**: The GUID or Directory ID of your Azure AD instance (This value can be found in **Azure portal > Azure Active Directory > Properties > Directory ID**)</span></span>
 
- <span data-ttu-id="9101e-123">Spustelėkite **Gerai**.</span><span class="sxs-lookup"><span data-stu-id="9101e-123">Click **OK**.</span></span>
 
5. <span data-ttu-id="9101e-124">Dešiniuoju pelės mygtuku spustelėkite **registrą** ir pasirinkite **naujas > registro elementą**.</span><span class="sxs-lookup"><span data-stu-id="9101e-124">Right-click on **Registry** and select **New > Registry Item**.</span></span>

6. <span data-ttu-id="9101e-125">Skirtuke **Bendrasis** Konfigūruokite šiuos dalykus:</span><span class="sxs-lookup"><span data-stu-id="9101e-125">On the **General** tab, configure the following:</span></span>
  
- <span data-ttu-id="9101e-126">**Veiksmas**: naujinimas</span><span class="sxs-lookup"><span data-stu-id="9101e-126">**Action**: Update</span></span>
    
- <span data-ttu-id="9101e-127">**Avilys**: HKEY_LOCAL_MACHINE</span><span class="sxs-lookup"><span data-stu-id="9101e-127">**Hive**: HKEY_LOCAL_MACHINE</span></span>
    
- <span data-ttu-id="9101e-128">**Rakto Path**: Software\microsoft\windows\currentversion\cdj\aad</span><span class="sxs-lookup"><span data-stu-id="9101e-128">**Key Path**: SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD</span></span>
    
- <span data-ttu-id="9101e-129">**Reikšmės pavadinimas**: tenantname</span><span class="sxs-lookup"><span data-stu-id="9101e-129">**Value name**: TenantName</span></span>
    
- <span data-ttu-id="9101e-130">**Reikšmės tipas**: REG_SZ</span><span class="sxs-lookup"><span data-stu-id="9101e-130">**Value type**: REG_SZ</span></span>
    
- <span data-ttu-id="9101e-131">**Reikšmės duomenys**: jūsų patvirtintas domeno vardas, jei naudojate bendrą aplinką, pvz., AD FS.</span><span class="sxs-lookup"><span data-stu-id="9101e-131">**Value data**: Your verified domain name if you are using federated environment such as AD FS.</span></span> <span data-ttu-id="9101e-132">Jūsų patvirtintas domeno vardas arba onmicrosoft.com domeno vardas (pvz., contoso. onmicrosoft). com, jei naudojate valdomą aplinką</span><span class="sxs-lookup"><span data-stu-id="9101e-132">Your verified domain name or your onmicrosoft.com domain name (for example, contoso.onmicrosoft).com if you are using managed environment</span></span>

- <span data-ttu-id="9101e-133">Spustelėkite **Gerai**.</span><span class="sxs-lookup"><span data-stu-id="9101e-133">Click **OK**.</span></span>

7. <span data-ttu-id="9101e-134">Uždarykite naujai sukurto GPO rengyklę.</span><span class="sxs-lookup"><span data-stu-id="9101e-134">Close the editor for the newly created GPO.</span></span>

8. <span data-ttu-id="9101e-135">Susiekite naujai sukurtą GPO su pageidaujamu OU, kuriame yra domeno sujungti kompiuteriai, priklausantys jūsų kontroliuojamam "rida" populiacijai.</span><span class="sxs-lookup"><span data-stu-id="9101e-135">Link the newly created GPO to the desired OU containing domain-joined computers that belong to your controlled rollout population.</span></span>

<span data-ttu-id="9101e-136">Daugiau informacijos ieškokite " [hibridinio" AZURE ad Join-AZURE AD "kontroliuojamo tikrinimo tikrinimas | "Microsoft" dokumentai](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control) ir  [trikčių diagnostikos hibridiniai "Azure Active Directory" sujungti įrenginiai | "Microsoft" dokumentai](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-hybrid-join-windows-current).</span><span class="sxs-lookup"><span data-stu-id="9101e-136">For more information, see [Controlled validation of hybrid Azure AD join - Azure AD | Microsoft Docs](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control) and  [Troubleshooting hybrid Azure Active Directory joined devices | Microsoft Docs](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-hybrid-join-windows-current).</span></span>









