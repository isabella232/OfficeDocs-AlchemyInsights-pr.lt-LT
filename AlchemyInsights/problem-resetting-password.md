---
title: Problemos nustatymo iš naujo slaptažodis
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/09/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003259"
- "9360"
ms.openlocfilehash: aa1eba1efef6a4c28aa6b9229071304093395922
ms.sourcegitcommit: 9a00005546c2fe473e3cea2b06e38c27eada88c4
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 03/09/2021
ms.locfileid: "50696284"
---
# <a name="problems-resetting-password"></a><span data-ttu-id="02034-102">Problemos iš naujo nustatyti slaptažodį</span><span class="sxs-lookup"><span data-stu-id="02034-102">Problems resetting password</span></span>

<span data-ttu-id="02034-103">Toliau pateikiami keli klausimai, su kuriais galite susidurti iš naujo nustatę slaptažodį ir galimus sprendimo būdus:</span><span class="sxs-lookup"><span data-stu-id="02034-103">Following are some of the issues that you might face when resetting password and the possible solutions:</span></span>

<span data-ttu-id="02034-104">**Iškilo problema dėl slaptažodžio nustatymo iš naujo, neįtrauktos į kitas kategorijas**</span><span class="sxs-lookup"><span data-stu-id="02034-104">**I'm having an issue with password reset not covered in the other categories**</span></span>

- <span data-ttu-id="02034-105">Įsitikinkite, kad turite teisę iš naujo nustatyti slaptažodžius.</span><span class="sxs-lookup"><span data-stu-id="02034-105">Ensure you are authorized to reset passwords.</span></span> <span data-ttu-id="02034-106">Tik visuotinis, slaptažodis ir vartotojų administratoriai gali iš naujo nustatyti vartotojų slaptažodžius.</span><span class="sxs-lookup"><span data-stu-id="02034-106">Only global, password, and user administrators can reset user passwords.</span></span> <span data-ttu-id="02034-107">Visuotiniai administratoriai taip pat gali iš naujo nustatyti kitų privilegijuotų administratoriaus slaptažodžius.</span><span class="sxs-lookup"><span data-stu-id="02034-107">Global administrators can also reset other privileged administrator's passwords.</span></span>
- <span data-ttu-id="02034-108">Įsitikinkite, kad suprantate licencijavimo reikalavimus:</span><span class="sxs-lookup"><span data-stu-id="02034-108">Ensure that you understand the licensing requirements:</span></span>
    - <span data-ttu-id="02034-109">Turite turėti bent vieną licenciją, priskirtą jūsų organizacijoje</span><span class="sxs-lookup"><span data-stu-id="02034-109">You must have at least one license assigned in your organization</span></span>
        - <span data-ttu-id="02034-110">Tik debesies vartotojai – bet kuris "Office 365" (O365) sumokėtas SKU arba "Azure AD Basic"</span><span class="sxs-lookup"><span data-stu-id="02034-110">Cloud only users - Any Office 365 (O365) paid SKU, or Azure AD Basic</span></span>
        - <span data-ttu-id="02034-111">Debesies ir (arba) vietiniai vartotojai – "Azure AD Premium" P1 arba P2, įmonės mobilumas + sauga (EPS) arba saugi gamybinė įmonė (SPE)</span><span class="sxs-lookup"><span data-stu-id="02034-111">Cloud and/or on-premises users - Azure AD Premium P1 or P2, Enterprise Mobility + Security (EMS), or Secure Productive Enterprise (SPE)</span></span>
        - <span data-ttu-id="02034-112">Norėdami sužinoti daugiau apie licencijavimo reikalavimus, peržiūrėkite straipsnį [licencijavimo reikalavimai, skirti "AZURE AD" savitarnos slaptažodžio nustatymo iš naujo](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing?WT.mc_id=Portal-Microsoft_Azure_Support).</span><span class="sxs-lookup"><span data-stu-id="02034-112">To read more about licensing requirements see the article [Licensing requirements for Azure AD self-service password reset](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>

<span data-ttu-id="02034-113">**Kilo problemų tikrinant slaptažodžio nustatymo iš naujo strategiją, kurią nustatėte**</span><span class="sxs-lookup"><span data-stu-id="02034-113">**I'm having problems testing the password reset policy I set**</span></span>

- <span data-ttu-id="02034-114">Neseniai taikytos strategijos gali užtrukti kelias minutes, kad būtų galima replikuoti visus duomenų centrus ir galutinius taškus.</span><span class="sxs-lookup"><span data-stu-id="02034-114">Recently applied policies can take several minutes to replicate across all data centers and end-points.</span></span> <span data-ttu-id="02034-115">Fiziniai atstumai iš duomenų centro taip pat turės įtakos, kaip greitai keičiami keitimai.</span><span class="sxs-lookup"><span data-stu-id="02034-115">Physical distance from the data center will also affect how quickly changes are applied.</span></span>
- <span data-ttu-id="02034-116">Išbandykite su galutinio vartotojo, o ne administratoriumi ir pilotu su nedideliu vartotojų rinkiniu.</span><span class="sxs-lookup"><span data-stu-id="02034-116">Test with an end user, not an administrator, and pilot with a small set of users.</span></span> <span data-ttu-id="02034-117">Strategijos, sukonfigūruotos "Azure" portale, taikomos tik galutiniams vartotojams, o ne administratoriams.</span><span class="sxs-lookup"><span data-stu-id="02034-117">The policies configured in the Azure portal ONLY apply to end-users, not administrators.</span></span> <span data-ttu-id="02034-118">"Microsoft" užtikrina, kad "Azure" administratoriaus vaidmuo būtų stipri numatytoji dviejų vartų slaptažodžio nustatymo iš naujo strategija (pvz.: visuotinis administratorius, pagalbos administratorius, slaptažodžių administratorius ir kt.)</span><span class="sxs-lookup"><span data-stu-id="02034-118">Microsoft enforces a strong default two-gate password reset policy for any Azure administrator role (Example: Global Administrator, Helpdesk Administrator, Password Administrator, etc.)</span></span>
    - <span data-ttu-id="02034-119">Sužinokite daugiau apie [administratorių strategijas](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-policy?WT.mc_id=Portal-Microsoft_Azure_Support#administrator-password-policy-differences).</span><span class="sxs-lookup"><span data-stu-id="02034-119">Learn more about [policies for administrators](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-policy?WT.mc_id=Portal-Microsoft_Azure_Support#administrator-password-policy-differences).</span></span>

<span data-ttu-id="02034-120">**Noriu įdiegti slaptažodį iš naujo, bet nenoriu, kad mano vartotojai užregistruotų papildomą saugos informaciją**</span><span class="sxs-lookup"><span data-stu-id="02034-120">**I want to deploy password reset but I don't want to make my users register additional security info**</span></span>

<span data-ttu-id="02034-121">Iš anksto užpildyti jūsų vartotojų duomenis, kad jie neturėtų!</span><span class="sxs-lookup"><span data-stu-id="02034-121">Pre-populate data for your users so they don't have to!</span></span> <span data-ttu-id="02034-122">-Kaip administratorius galite nustatyti savo vartotojams telefono ir elektroninio pašto ypatybes prieš atkurdami slaptažodį iš naujo savo organizacijai.</span><span class="sxs-lookup"><span data-stu-id="02034-122">- As an administrator you can set phone and email properties for your users before rolling out password reset to your organization.</span></span> <span data-ttu-id="02034-123">Tai galite padaryti naudodami API, "PowerShell" arba "Azure AD Connect".</span><span class="sxs-lookup"><span data-stu-id="02034-123">You can do this using an API, PowerShell, or Azure AD Connect.</span></span> <span data-ttu-id="02034-124">Daugiau informacijos rasite čia:</span><span class="sxs-lookup"><span data-stu-id="02034-124">More information here:</span></span>
- [<span data-ttu-id="02034-125">Slaptažodžio nustatymo iš naujo diegimas nereikalaujant vartotojų registruotis</span><span class="sxs-lookup"><span data-stu-id="02034-125">Deploying password reset without requiring users to register</span></span>](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-policy?WT.mc_id=Portal-Microsoft_Azure_Support#administrator-password-policy-differences)
- [<span data-ttu-id="02034-126">Kokius duomenis naudoja slaptažodžio nustatymas iš naujo</span><span class="sxs-lookup"><span data-stu-id="02034-126">What data is used by password reset</span></span>](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support)

<span data-ttu-id="02034-127">**Slaptažodžio nustatymo iš naujo mygtukas yra pilkas**</span><span class="sxs-lookup"><span data-stu-id="02034-127">**The password reset button is greyed-out**</span></span>

<span data-ttu-id="02034-128">Jūs neturite teisę iš naujo nustatyti šio vartotojo slaptažodžių.</span><span class="sxs-lookup"><span data-stu-id="02034-128">You are not authorized to reset this user's passwords.</span></span> <span data-ttu-id="02034-129">Tik visuotinis, slaptažodis ir vartotojų administratoriai gali iš naujo nustatyti vartotojų slaptažodžius.</span><span class="sxs-lookup"><span data-stu-id="02034-129">Only global, password, and user administrators can reset user passwords.</span></span> <span data-ttu-id="02034-130">Visuotiniai administratoriai taip pat gali iš naujo nustatyti kitų privilegijuotų administratoriaus slaptažodžius.</span><span class="sxs-lookup"><span data-stu-id="02034-130">Global administrators can also reset other privileged administrator's passwords.</span></span>

<span data-ttu-id="02034-131">**Nematau slaptažodžio nustatymo iš naujo ašmenų**</span><span class="sxs-lookup"><span data-stu-id="02034-131">**I don't see the password reset blade**</span></span>

<span data-ttu-id="02034-132">Jūs nesate įgalioti iš naujo nustatyti slaptažodžius.</span><span class="sxs-lookup"><span data-stu-id="02034-132">You are not authorized to reset passwords.</span></span> <span data-ttu-id="02034-133">Tik visuotinis, slaptažodis ir vartotojų administratoriai gali iš naujo nustatyti vartotojų slaptažodžius.</span><span class="sxs-lookup"><span data-stu-id="02034-133">Only global, password, and user administrators can reset user passwords.</span></span> <span data-ttu-id="02034-134">Visuotiniai administratoriai taip pat gali iš naujo nustatyti kitų privilegijuotų administratoriaus slaptažodžius.</span><span class="sxs-lookup"><span data-stu-id="02034-134">Global administrators can also reset other privileged administrator's passwords.</span></span>

<span data-ttu-id="02034-135">**Nematau vietinio integravimo peilio slaptažodžio nustatymo iš naujo**</span><span class="sxs-lookup"><span data-stu-id="02034-135">**I don't see the on-premises integration blade in password reset**</span></span>

- <span data-ttu-id="02034-136">Vietinis integravimo peilis rodomas tik hibridinėse aplinkose – tai reiškia, kad naudojate slaptažodį write, kad galėtumėte manipuliuoti vietinio vartotojo slaptažodžiais.</span><span class="sxs-lookup"><span data-stu-id="02034-136">The on-premises integration blade only appears in hybrid environments - meaning you are using password writeback to manipulate on-premises user's passwords.</span></span>
- <span data-ttu-id="02034-137">Nematote šio disko, jei:</span><span class="sxs-lookup"><span data-stu-id="02034-137">You do not see this blade if:</span></span>
    - <span data-ttu-id="02034-138">Nenaudojate slaptažodžio įrašymo atgal</span><span class="sxs-lookup"><span data-stu-id="02034-138">You are not using password writeback</span></span>
    - <span data-ttu-id="02034-139">Iškilo problema dėl slaptažodžio įrašymo ir diegimo ryšio</span><span class="sxs-lookup"><span data-stu-id="02034-139">There is a problem with your installation/connectivity of password writeback</span></span>
    - <span data-ttu-id="02034-140">Iškilo "Azure AD Connect" diegimo/ryšio problema</span><span class="sxs-lookup"><span data-stu-id="02034-140">There is a problem with your installation/connectivity of Azure AD Connect</span></span>
    - <span data-ttu-id="02034-141">Jei reikia daugiau trikčių šalinimo veiksmų problemoms su slaptažodžiais write, žr skyriuje [slaptažodžio įrašymo trikčių šalinimas](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support)</span><span class="sxs-lookup"><span data-stu-id="02034-141">For more troubleshooting steps for issues with password writeback, see the section [Troubleshoot password writeback](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support)</span></span>

<span data-ttu-id="02034-142">**Nežinau, kaip iš naujo nustatyti vartotojo slaptažodį**</span><span class="sxs-lookup"><span data-stu-id="02034-142">**I don't know how to reset a user's password**</span></span>

1. <span data-ttu-id="02034-143">Prisijunkite prie "Azure" portalo kaip tinkamo administratoriaus.</span><span class="sxs-lookup"><span data-stu-id="02034-143">Sign in to the Azure portal as an appropriate admin.</span></span>
1. <span data-ttu-id="02034-144">Eikite į diską vartotojai ir grupės, pasirinkite **visi vartotojai**.</span><span class="sxs-lookup"><span data-stu-id="02034-144">Go to the Users and groups blade, select **All Users**.</span></span>
1. <span data-ttu-id="02034-145">Pasirinkite vartotoją iš sąrašo.</span><span class="sxs-lookup"><span data-stu-id="02034-145">Select a user from the list.</span></span>
1. <span data-ttu-id="02034-146">Pasirinktam vartotojui pasirinkite **apžvalga**, tada komandų juostoje spustelėkite **iš naujo nustatyti slaptažodį**.</span><span class="sxs-lookup"><span data-stu-id="02034-146">For the selected user, select **Overview**, and then in the command bar, click **Reset password**.</span></span>
1. <span data-ttu-id="02034-147">Vadovaukitės ekrane pateikiamomis instrukcijomis.</span><span class="sxs-lookup"><span data-stu-id="02034-147">Follow the instructions on the screen.</span></span>
    - <span data-ttu-id="02034-148">Tik iš naujo vykdomas "Azure" portalo palaikymo slaptažodžio įrašymo metu.</span><span class="sxs-lookup"><span data-stu-id="02034-148">Only resets performed through the Azure portal support password writeback.</span></span>

<span data-ttu-id="02034-149">**Iš naujo nustatyti vietinio vartotojo slaptažodį iš "Office 365" administravimo portalo arba "Office 365 Mobile" taikomosios programos, tačiau vartotojas vis tiek negali prisijungti**</span><span class="sxs-lookup"><span data-stu-id="02034-149">**I reset an on-premises user's password from the Office 365 Admin portal or Office 365 mobile application but the user is still not able to sign in**</span></span>

<span data-ttu-id="02034-150">Slaptažodžio write-back nepalaiko šiame portale.</span><span class="sxs-lookup"><span data-stu-id="02034-150">Password Writeback is not supported in this portal.</span></span> <span data-ttu-id="02034-151">Iš naujo nustatyti vartotojo slaptažodį dar kartą "Azure" portale – portal.azure.com</span><span class="sxs-lookup"><span data-stu-id="02034-151">Reset the user's password again in the Azure portal - portal.azure.com</span></span>

