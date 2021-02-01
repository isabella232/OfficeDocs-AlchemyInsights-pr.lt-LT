---
title: Problemos su kredencialais
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
- "9004330"
- "7723"
ms.openlocfilehash: e463e8181123277f3509c0b0bb6f871a1a09bed1
ms.sourcegitcommit: c3574f574afe5a40a6ea2c6e399c58977d18bb73
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 01/29/2021
ms.locfileid: "50063681"
---
# <a name="issues-with-credentials"></a><span data-ttu-id="a1bb8-102">Problemos su kredencialais</span><span class="sxs-lookup"><span data-stu-id="a1bb8-102">Issues with credentials</span></span>

<span data-ttu-id="a1bb8-103">["Microsoft" tapatybės platforma ir "OAuth" 2,0 kliento kredencialų srautas](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow) aprašo, kaip programa tiesiogiai atitinka "oauth 2,0" kliento kredencialų suteikimo srautą.</span><span class="sxs-lookup"><span data-stu-id="a1bb8-103">[Microsoft identity platform and the OAuth 2.0 client credentials flow](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow) describes how to program directly against the OAuth 2.0 client credentials grant flow.</span></span>

<span data-ttu-id="a1bb8-104">**Kaip valdyti taikomosios programos slaptažodį arba sertifikato kredencialus?**</span><span class="sxs-lookup"><span data-stu-id="a1bb8-104">**How do I manage an application's password or certificate credentials?**</span></span>

<span data-ttu-id="a1bb8-105">"Azure CLI" galite naudoti [AZ ad taikomosios programos](https://docs.microsoft.com/cli/azure/ad/app/credential) kredencialus, kad panaikintumėte, sąraše arba iš naujo nustatytumėte taikomosios programos slaptažodį arba sertifikato kredencialus.</span><span class="sxs-lookup"><span data-stu-id="a1bb8-105">In the Azure CLI, you can use [az ad app credential](https://docs.microsoft.com/cli/azure/ad/app/credential) to delete, list, or reset an application's password or certificate credentials.</span></span>

<span data-ttu-id="a1bb8-106">**Kaip iš naujo nustatyti vartotojų slaptažodžius?**</span><span class="sxs-lookup"><span data-stu-id="a1bb8-106">**How do my users reset their passwords?**</span></span>

<span data-ttu-id="a1bb8-107">Vartotojai turi [registruotis savitarnos slaptažodžio nustatymo iš naujo,](https://docs.microsoft.com/azure/active-directory/user-help/active-directory-passwords-reset-register) kad galėtų iš naujo nustatyti savo slaptažodžius.</span><span class="sxs-lookup"><span data-stu-id="a1bb8-107">Users need to [register for self-service password reset](https://docs.microsoft.com/azure/active-directory/user-help/active-directory-passwords-reset-register) before they can reset their passwords.</span></span> <span data-ttu-id="a1bb8-108">Užregistravus vartotoją, jie gali vadovautis šiame straipsnyje pateiktomis instrukcijomis, kad iš naujo nustatytumėte slaptažodį: [darbo arba mokymo įstaigos slaptažodžio nustatymas iš naujo](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#how-to-reset-or-unlock-your-password-for-a-work-or-school-account).</span><span class="sxs-lookup"><span data-stu-id="a1bb8-108">Once a user has registered, they can follow the instructions in this article to reset their password: [Reset your work or school password](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#how-to-reset-or-unlock-your-password-for-a-work-or-school-account).</span></span>

<span data-ttu-id="a1bb8-109">**Kaip mano vartotojai keičia savo slaptažodžius?**</span><span class="sxs-lookup"><span data-stu-id="a1bb8-109">**How do my users change their passwords?**</span></span>

<span data-ttu-id="a1bb8-110">Vartotojai gali atlikti šiame straipsnyje nurodytus veiksmus, kad pakeistų slaptažodžius: [kaip pakeisti slaptažodį](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#how-to-change-your-password).</span><span class="sxs-lookup"><span data-stu-id="a1bb8-110">Users can follow the steps in this article to change their passwords: [How to change your password](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#how-to-change-your-password).</span></span>
<span data-ttu-id="a1bb8-111">Jie taip pat gali [valdyti taikomųjų programų slaptažodžius dviem veiksmais](https://docs.microsoft.com/azure/active-directory/user-help/multi-factor-authentication-end-user-app-passwords).</span><span class="sxs-lookup"><span data-stu-id="a1bb8-111">They can also [Manage app passwords for two-step verification](https://docs.microsoft.com/azure/active-directory/user-help/multi-factor-authentication-end-user-app-passwords).</span></span>

<span data-ttu-id="a1bb8-112">**Mano vartotojas gauna klaidą keičiant arba iš naujo nustatant slaptažodį**</span><span class="sxs-lookup"><span data-stu-id="a1bb8-112">**My user is getting an error when changing or resetting their password**</span></span>

<span data-ttu-id="a1bb8-113">Šis saitas pateiks informaciją apie įprastas problemas, kurios gali iškilti, kai vartotojas bando iš naujo nustatyti slaptažodį: [Dažniausios problemos ir jų sprendimai](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#common-problems-and-their-solutions)</span><span class="sxs-lookup"><span data-stu-id="a1bb8-113">This link will provide information on common problems that can arise when a user is trying to reset their password: [Common problems and their solutions](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#common-problems-and-their-solutions)</span></span>

<span data-ttu-id="a1bb8-114">**Iškilo problema iš naujo nustatant vartotojo slaptažodį**</span><span class="sxs-lookup"><span data-stu-id="a1bb8-114">**I'm having a problem resetting a user's password**</span></span>

- <span data-ttu-id="a1bb8-115">Įsitikinkite, kad turite teisę iš naujo nustatyti slaptažodžius.</span><span class="sxs-lookup"><span data-stu-id="a1bb8-115">Make sure you are authorized to reset passwords.</span></span> <span data-ttu-id="a1bb8-116">*Tik visuotinis, slaptažodis ir vartotojų administratoriai gali iš naujo nustatyti vartotojų slaptažodžius.*</span><span class="sxs-lookup"><span data-stu-id="a1bb8-116">*Only global, password, and user administrators can reset user passwords.*</span></span> <span data-ttu-id="a1bb8-117">Visuotiniai administratoriai taip pat gali iš naujo nustatyti kitų privilegijuotų administratoriaus slaptažodžius.</span><span class="sxs-lookup"><span data-stu-id="a1bb8-117">Global administrators can also reset other privileged administrator's passwords.</span></span>

- <span data-ttu-id="a1bb8-118">Įsitikinkite, kad suprantate licencijavimo reikalavimus:</span><span class="sxs-lookup"><span data-stu-id="a1bb8-118">Make sure you understand the licensing requirements:</span></span>

  - <span data-ttu-id="a1bb8-119">Turite turėti bent vieną licenciją, priskirtą jūsų organizacijoje:</span><span class="sxs-lookup"><span data-stu-id="a1bb8-119">You must have at least one license assigned in your organization:</span></span>
    - <span data-ttu-id="a1bb8-120">**Tik debesies vartotojai** – bet kuris "Office 365" (O365) sumokėtas SKU arba "Azure AD Basic"</span><span class="sxs-lookup"><span data-stu-id="a1bb8-120">**Cloud only users** - Any Office 365 (O365) paid SKU, or Azure AD Basic</span></span>
    - <span data-ttu-id="a1bb8-121">**Debesies ir (arba) vietiniai vartotojai – "** Azure AD Premium" P1 arba P2, įmonės mobilumas + sauga (EPS) arba saugi gamybinė įmonė (SPE)</span><span class="sxs-lookup"><span data-stu-id="a1bb8-121">**Cloud and/or on-premises users** - Azure AD Premium P1 or P2, Enterprise Mobility + Security (EMS), or Secure Productive Enterprise (SPE)</span></span>
    - <span data-ttu-id="a1bb8-122">Jei norite sužinoti daugiau apie licencijavimo reikalavimus, skaitykite " [AZURE AD" savitarnos slaptažodžio nustatymo iš naujo licencijavimo reikalavimus](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing).</span><span class="sxs-lookup"><span data-stu-id="a1bb8-122">To learn more about licensing requirements, see [Licensing requirements for Azure AD self-service password reset](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing).</span></span>
- <span data-ttu-id="a1bb8-123">Norėdami iš naujo nustatyti vartotojo slaptažodį, raskite vartotoją "Azure AD".</span><span class="sxs-lookup"><span data-stu-id="a1bb8-123">To reset a user's password, find the user in Azure AD.</span></span> <span data-ttu-id="a1bb8-124">Po to vartotojo Apžvalgos disku spustelėkite mygtuką iš naujo nustatyti slaptažodį.</span><span class="sxs-lookup"><span data-stu-id="a1bb8-124">Then, on the overview blade for that user, click the "reset password" button.</span></span>

<span data-ttu-id="a1bb8-125">**Slaptažodžio nustatymo iš naujo mygtukas yra pilkas**</span><span class="sxs-lookup"><span data-stu-id="a1bb8-125">**The password reset button is greyed-out**</span></span>

<span data-ttu-id="a1bb8-126">Jūs neturite teisę iš naujo nustatyti **šio** vartotojo slaptažodžių.</span><span class="sxs-lookup"><span data-stu-id="a1bb8-126">You are not authorized to reset **this** user's passwords.</span></span> <span data-ttu-id="a1bb8-127">*Tik visuotinis, slaptažodis ir vartotojų administratoriai gali iš naujo nustatyti vartotojų slaptažodžius.*</span><span class="sxs-lookup"><span data-stu-id="a1bb8-127">*Only global, password, and user administrators can reset user passwords.*</span></span> <span data-ttu-id="a1bb8-128">Visuotiniai administratoriai taip pat gali iš naujo nustatyti kitų privilegijuotų administratoriaus slaptažodžius.</span><span class="sxs-lookup"><span data-stu-id="a1bb8-128">Global administrators can also reset other privileged administrator's passwords.</span></span>

<span data-ttu-id="a1bb8-129">**Nematau slaptažodžio nustatymo iš naujo ašmenų**</span><span class="sxs-lookup"><span data-stu-id="a1bb8-129">**I don't see the password reset blade**</span></span>

<span data-ttu-id="a1bb8-130">Jūs nesate įgalioti iš naujo nustatyti slaptažodžius.</span><span class="sxs-lookup"><span data-stu-id="a1bb8-130">You are not authorized to reset passwords.</span></span> <span data-ttu-id="a1bb8-131">*Tik visuotinis, slaptažodis ir vartotojų administratoriai gali iš naujo nustatyti vartotojų slaptažodžius.*</span><span class="sxs-lookup"><span data-stu-id="a1bb8-131">*Only global, password, and user administrators can reset user passwords.*</span></span> <span data-ttu-id="a1bb8-132">Visuotiniai administratoriai taip pat gali iš naujo nustatyti kitų privilegijuotų administratoriaus slaptažodžius.</span><span class="sxs-lookup"><span data-stu-id="a1bb8-132">Global administrators can also reset other privileged administrator's passwords.</span></span>

<span data-ttu-id="a1bb8-133">**Nematau vietinio integravimo peilio slaptažodžio nustatymo iš naujo**</span><span class="sxs-lookup"><span data-stu-id="a1bb8-133">**I don't see the on-premises integration blade in password reset**</span></span>

- <span data-ttu-id="a1bb8-134">Vietinis integravimo peilis rodomas tik hibridinėse aplinkose – tai reiškia, kad naudojate slaptažodį write, kad galėtumėte manipuliuoti vietinio vartotojo slaptažodžiais.</span><span class="sxs-lookup"><span data-stu-id="a1bb8-134">The on-premises integration blade only appears in hybrid environments - meaning you are using password writeback to manipulate on-premises user's passwords.</span></span>

- <span data-ttu-id="a1bb8-135">Nematote šio disko, jei:</span><span class="sxs-lookup"><span data-stu-id="a1bb8-135">You do not see this blade if:</span></span>

  - <span data-ttu-id="a1bb8-136">Nenaudojate slaptažodžio įrašymo atgal</span><span class="sxs-lookup"><span data-stu-id="a1bb8-136">You are not using password writeback</span></span>
  - <span data-ttu-id="a1bb8-137">Iškilo problema dėl slaptažodžio įrašymo ir diegimo ryšio</span><span class="sxs-lookup"><span data-stu-id="a1bb8-137">There is a problem with your installation/connectivity of password writeback</span></span>
  - <span data-ttu-id="a1bb8-138">Iškilo "Azure AD Connect" diegimo/ryšio problema</span><span class="sxs-lookup"><span data-stu-id="a1bb8-138">There is a problem with your installation/connectivity of Azure AD Connect</span></span>
  - <span data-ttu-id="a1bb8-139">Jei reikia daugiau trikčių šalinimo veiksmų problemoms su slaptažodžiais write, žiūrėkite [slaptažodžio įrašymo trikčių šalinimas](https://docs.microsoft.com/azure/active-directory/authentication/troubleshoot-sspr-writeback)</span><span class="sxs-lookup"><span data-stu-id="a1bb8-139">For more troubleshooting steps for issues with password writeback, see [Troubleshoot password writeback](https://docs.microsoft.com/azure/active-directory/authentication/troubleshoot-sspr-writeback)</span></span>

<span data-ttu-id="a1bb8-140">**Nežinau, kaip iš naujo nustatyti vartotojo slaptažodį**</span><span class="sxs-lookup"><span data-stu-id="a1bb8-140">**I don't know how to reset a user's password**</span></span>

1. <span data-ttu-id="a1bb8-141">Prisijunkite prie "Azure" portalo kaip tinkamo administratoriaus.</span><span class="sxs-lookup"><span data-stu-id="a1bb8-141">Sign in to the Azure portal as an appropriate admin.</span></span>
2. <span data-ttu-id="a1bb8-142">Eikite į diską **vartotojai ir grupės** , pasirinkite **visi vartotojai**.</span><span class="sxs-lookup"><span data-stu-id="a1bb8-142">Go to the **Users and groups** blade, select **All Users**.</span></span>
3. <span data-ttu-id="a1bb8-143">Pasirinkite vartotoją iš sąrašo.</span><span class="sxs-lookup"><span data-stu-id="a1bb8-143">Select a user from the list.</span></span>
4. <span data-ttu-id="a1bb8-144">Pasirinktam vartotojui pasirinkite **apžvalga**, tada komandų juostoje pasirinkite **iš naujo nustatyti slaptažodį**.</span><span class="sxs-lookup"><span data-stu-id="a1bb8-144">For the selected user, select **Overview**, and then in the command bar, select **Reset password**.</span></span>
5. <span data-ttu-id="a1bb8-145">Pasirinkite mygtuką **iš naujo nustatyti slaptažodį** ir vadovaukitės ekrane pateikiamomis instrukcijomis.</span><span class="sxs-lookup"><span data-stu-id="a1bb8-145">Select the **Reset password** button and follow the instructions on the screen.</span></span>
    - <span data-ttu-id="a1bb8-146">Tik iš naujo vykdomas " **Azure" portalo** palaikymo slaptažodžio įrašymo metu.</span><span class="sxs-lookup"><span data-stu-id="a1bb8-146">Only resets performed through the **Azure portal** support password writeback.</span></span>

<span data-ttu-id="a1bb8-147">**Iš naujo nustatyti vietinio vartotojo slaptažodį iš "Office 365" administravimo portalo arba "Office 365 Mobile" taikomosios programos, tačiau vartotojas vis tiek negali prisijungti**</span><span class="sxs-lookup"><span data-stu-id="a1bb8-147">**I reset an on-premises user's password from the Office 365 Admin portal or Office 365 mobile application but the user is still not able to sign in**</span></span>

<span data-ttu-id="a1bb8-148">Slaptažodžio write-back nepalaiko šiame portale.</span><span class="sxs-lookup"><span data-stu-id="a1bb8-148">Password Writeback is not supported in this portal.</span></span> <span data-ttu-id="a1bb8-149">Iš naujo nustatyti vartotojo slaptažodį dar kartą "Azure" portale.</span><span class="sxs-lookup"><span data-stu-id="a1bb8-149">Reset the user's password again in the Azure portal.</span></span>
