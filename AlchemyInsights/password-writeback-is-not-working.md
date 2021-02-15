---
title: Neveikia slaptažodis write
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
- "9004595"
- "8210"
ms.openlocfilehash: d7766f908f025b5db8299aa45d01dc5389b321ec
ms.sourcegitcommit: 2f39850ac0fba9fbeba9b8b7939ae79b505d3b67
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 02/12/2021
ms.locfileid: "50243516"
---
# <a name="password-writeback-is-not-working"></a><span data-ttu-id="e8c07-102">Neveikia slaptažodis write</span><span class="sxs-lookup"><span data-stu-id="e8c07-102">Password Writeback is not working</span></span>

<span data-ttu-id="e8c07-103">**Kilo problemų konfigūruojant slaptažodžius**</span><span class="sxs-lookup"><span data-stu-id="e8c07-103">**I'm having problems configuring password writeback**</span></span>

- <span data-ttu-id="e8c07-104">Slaptažodis write-back yra priemoka funkcija.</span><span class="sxs-lookup"><span data-stu-id="e8c07-104">Password writeback is a premium feature.</span></span>
- <span data-ttu-id="e8c07-105">Įsitikinkite, kad suprantate licencijavimo reikalavimus:</span><span class="sxs-lookup"><span data-stu-id="e8c07-105">Make sure that you understand the licensing requirements:</span></span>
  - <span data-ttu-id="e8c07-106">Turite turėti bent vieną licenciją, priskirtą jūsų organizacijoje</span><span class="sxs-lookup"><span data-stu-id="e8c07-106">You must have at least one license assigned in your organization</span></span>
  - <span data-ttu-id="e8c07-107">**Tik debesies vartotojai** – bet kuris "Office 365" (O365) sumokėtas SKU arba "Azure AD Basic"</span><span class="sxs-lookup"><span data-stu-id="e8c07-107">**Cloud only users** - Any Office 365 (O365) paid SKU, or Azure AD Basic</span></span>
  - <span data-ttu-id="e8c07-108">**Debesies ir (arba) vietiniai vartotojai – "** Azure AD Premium" P1 arba P2, įmonės mobilumas + sauga (EPS) arba saugi gamybinė įmonė (SPE)</span><span class="sxs-lookup"><span data-stu-id="e8c07-108">**Cloud and/or on-premises users** - Azure AD Premium P1 or P2, Enterprise Mobility + Security (EMS), or Secure Productive Enterprise (SPE)</span></span>
    - <span data-ttu-id="e8c07-109">Norėdami sužinoti daugiau apie licencijavimo reikalavimus, skaitykite " [AZURE AD" savitarnos slaptažodžio nustatymo iš naujo licencijavimo reikalavimai](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing)</span><span class="sxs-lookup"><span data-stu-id="e8c07-109">To learn more about licensing requirements, see [Licensing requirements for Azure AD self-service password reset](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing)</span></span>
- <span data-ttu-id="e8c07-110">Turite bent vieną administratoriaus paskyrą ir vieną bandomosios vartotojo paskyrą su viena iš atitinkamos licencijos.</span><span class="sxs-lookup"><span data-stu-id="e8c07-110">You have at least one administrator account and one test user account with one of the appropriate license.</span></span>
- <span data-ttu-id="e8c07-111">Turite prijungti "Azure AD Connect" prie pirminio domeno valdiklio emuliatorius, kad veiktų slaptažodis.</span><span class="sxs-lookup"><span data-stu-id="e8c07-111">You must connect Azure AD Connect to the Primary Domain Controller Emulator for password writeback to work.</span></span> <span data-ttu-id="e8c07-112">Galite sukonfigūruoti "Azure AD Connect" naudoti pirminį domeno valdiklį dešiniuoju pelės mygtuku spustelėdami "Active Directory" sinchronizavimo jungties **ypatybes** , tada pasirinkite **Konfigūruoti katalogų skaidinius**.</span><span class="sxs-lookup"><span data-stu-id="e8c07-112">You can configure Azure AD Connect to use a Primary Domain Controller by right clicking on the **properties** of the Active Directory synchronization connector, then selecting **configure directory partitions**.</span></span> <span data-ttu-id="e8c07-113">Čia ieškokite skyriaus **domeno valdiklio ryšių parametrai** ir pažymėkite žymės langelį **naudoti tik pageidaujamus domenų valdiklius**.</span><span class="sxs-lookup"><span data-stu-id="e8c07-113">From there, look for the **domain controller connection settings** section and check the box titled **only use preferred domain controllers**.</span></span>
  > [!NOTE]
  > <span data-ttu-id="e8c07-114">Jei pageidaujamas DC nėra PDC emuliatorius, "Azure AD Connect" vis tiek pasieks slaptažodžių įrašymo PDC.</span><span class="sxs-lookup"><span data-stu-id="e8c07-114">If the preferred DC is not a PDC emulator, Azure AD Connect will still reach out to the PDC for password writeback.</span></span>
- <span data-ttu-id="e8c07-115">Slaptažodžio nustatymas iš naujo sukonfigūruotas ir įgalintas jūsų nuomotojuje.</span><span class="sxs-lookup"><span data-stu-id="e8c07-115">Password reset has been configured and enabled in your tenant.</span></span> <span data-ttu-id="e8c07-116">Daugiau informacijos ieškokite [vartotojų įgalinimas iš naujo nustatyti "AZURE AD" slaptažodžius](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-getting-started).</span><span class="sxs-lookup"><span data-stu-id="e8c07-116">For more information, see [Enable users to reset their Azure AD passwords](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-getting-started).</span></span>
- <span data-ttu-id="e8c07-117">Įsitikinkite, kad administratoriaus abonementas, naudojamas slaptažodžiui write, yra debesies administratoriaus abonementas (sukurtas "Azure AD" ne vietiniame skelbime)</span><span class="sxs-lookup"><span data-stu-id="e8c07-117">Make sure that the administrator account being used to enable Password Writeback is a cloud administrator account (created in Azure AD not on-premises AD)</span></span>
- <span data-ttu-id="e8c07-118">Turite vieną arba kelių miškų skelbimą vietiniame diegime, kuriame veikia "Windows Server" 2008 R2, "Windows Server 2012" arba "Windows Server 2012 R2" su įdiegtais naujausiais pakeitimų paketais</span><span class="sxs-lookup"><span data-stu-id="e8c07-118">You have a single or multi-forest AD on-premises deployment running Windows Server 2008 R2, Windows Server 2012, or Windows Server 2012 R2 with the latest service packs installed</span></span>
- <span data-ttu-id="e8c07-119">Įdiegtas "Azure AD Connect" įrankis ir jūs paruošėte skelbimo aplinką, skirtą sinchronizuoti debesyje.</span><span class="sxs-lookup"><span data-stu-id="e8c07-119">You have the Azure AD Connect tool installed and you have prepared your AD environment for synchronization to the cloud.</span></span> <span data-ttu-id="e8c07-120">Prieš išbandydami slaptažodį write, įsitikinkite, kad pirmą kartą atliekate visą importavimą ir visišką sinchronizavimą iš AD ir Azure AD "Azure AD Connect".</span><span class="sxs-lookup"><span data-stu-id="e8c07-120">Before testing password writeback, make sure that you first complete a full import and full sync from both AD and Azure AD in Azure AD Connect.</span></span>
- <span data-ttu-id="e8c07-121">Norėdami sužinoti daugiau, Sužinokite, kaip atlikti [visas sinchronizavimo ir visas importavimas naudojant "AZURE AD Connect](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-operations) "</span><span class="sxs-lookup"><span data-stu-id="e8c07-121">To learn more, see how to do a [full sync and full import in Azure AD Connect](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-operations)</span></span>

<span data-ttu-id="e8c07-122">**Iškilo problema dėl slaptažodžio įrašymo atgal ryšio**</span><span class="sxs-lookup"><span data-stu-id="e8c07-122">**I'm having a problem with password writeback connectivity**</span></span>

1. <span data-ttu-id="e8c07-123">Naujausios " [AZURE AD Connect](https://www.microsoft.com/download/details.aspx?id=47594) " versijos atsisiuntimas ir įjungimas</span><span class="sxs-lookup"><span data-stu-id="e8c07-123">Download and enable the latest version of [Azure AD Connect](https://www.microsoft.com/download/details.aspx?id=47594)</span></span>
2. <span data-ttu-id="e8c07-124">Užkardos konfigūracija: "Azure AD Connect" įrankyje (1.1.443 ir anksčiau) reikės **siuntimo https** prieigos:</span><span class="sxs-lookup"><span data-stu-id="e8c07-124">Firewall configuration: The Azure AD Connect tool (1.1.443 and above) will need **outbound HTTPS** access to:</span></span>
    - <span data-ttu-id="e8c07-125">passwordreset.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="e8c07-125">passwordreset.microsoftonline.com</span></span>
    - <span data-ttu-id="e8c07-126">servicebus. Windows. Networks</span><span class="sxs-lookup"><span data-stu-id="e8c07-126">servicebus.windows.networks</span></span>
3. <span data-ttu-id="e8c07-127">Leisti naudoti tuščiosios eigos ryšius bent 2-3 min.</span><span class="sxs-lookup"><span data-stu-id="e8c07-127">Allow idle connections to persist for at least 2-3 minutes</span></span>

<span data-ttu-id="e8c07-128">**Vis dar kyla problemų dėl slaptažodžio įrašymo**</span><span class="sxs-lookup"><span data-stu-id="e8c07-128">**I'm still having problems with password writeback**</span></span>

- <span data-ttu-id="e8c07-129">Jei vis tiek kyla problemų, bandykite išjungti ir iš naujo įgalinti slaptažodžio įrašymo paslaugą "Azure AD Connect" įrankyje</span><span class="sxs-lookup"><span data-stu-id="e8c07-129">If you are still having difficulty, try disabling and re-enabling the password writeback service in the Azure AD Connect tool</span></span>
- <span data-ttu-id="e8c07-130">Norėdami sužinoti daugiau, Sužinokite, kaip [išjungti ir iš naujo įjungti slaptažodį write-back](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-troubleshoot)</span><span class="sxs-lookup"><span data-stu-id="e8c07-130">To learn more, see how to [disable and re-enable password writeback](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-troubleshoot)</span></span>
