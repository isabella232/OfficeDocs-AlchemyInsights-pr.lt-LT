---
title: Slaptažodžių sinchronizavimas
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/24/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004595"
- "8619"
ms.openlocfilehash: 601649f6e5212ca03df5fcc32cd1d02c133e9170
ms.sourcegitcommit: 6741a997fff871d263f92d3ff7fb61e7755956a9
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 03/04/2021
ms.locfileid: "50482039"
---
# <a name="password-synchronization"></a><span data-ttu-id="a40c2-102">Slaptažodžių sinchronizavimas</span><span class="sxs-lookup"><span data-stu-id="a40c2-102">Password synchronization</span></span>

<span data-ttu-id="a40c2-103">**Slaptažodžių maišos sinchronizavimas neveiks**</span><span class="sxs-lookup"><span data-stu-id="a40c2-103">**Password Hash Synchronization does not work at all**</span></span>

<span data-ttu-id="a40c2-104">Kai kurios Dažniausios problemos, su kuriomis susiduria Klientai, kai neveikia slaptažodžių maišos sinchronizavimas:</span><span class="sxs-lookup"><span data-stu-id="a40c2-104">Some common issues customers encounter when Password Hash Synchronization does not work are:</span></span>

- <span data-ttu-id="a40c2-105">"Azure AD Connect" naudojamos "Active Directory" paskyros ryšį su vietinio "Active Directory" nesuteiktas **lygiagretusis** katalogas ir **replikuoti katalogo pakeičiami visi** teisės, kurios reikalingos slaptažodžių sinchronizavimui – reikia tai pataisyti suteikiant šias teises "Active Directory" abonementui.</span><span class="sxs-lookup"><span data-stu-id="a40c2-105">The Active Directory account used by Azure AD Connect to communicate with on-premises Active Directory is not granted **Replicate Directory Changes** and **Replicate Directory Changes All** permissions, which are required for password synchronization - You need to fix this by granting these permissions to the Active Directory account.</span></span>
- <span data-ttu-id="a40c2-106">Slaptažodžių maišos sinchronizavimas yra išjungtas, kai administratorius pakeitė vartotojo Sign-In metodą iš **Slaptažodžių sinchronizavimo** į kitą parinktį, pvz., **susiejimo su AD FS** "Azure AD Connect" vediklyje – galite tai pataisyti iš naujo įgalindami **slaptažodžių maišos sinchronizavimo** funkciją "Azure AD Connect" vediklyje.</span><span class="sxs-lookup"><span data-stu-id="a40c2-106">Password hash synchronization is disabled after an administrator changed the User Sign-In method from **Password Synchronization** to another option such as **Federation with AD FS** in the Azure AD Connect wizard - You can fix this by re-enabling the **password hash synchronization** feature in the Azure AD Connect wizard.</span></span>
- <span data-ttu-id="a40c2-107">Ryšio problema su vietinio "Active Directory".</span><span class="sxs-lookup"><span data-stu-id="a40c2-107">Connectivity issue with on-premises Active Directory.</span></span> <span data-ttu-id="a40c2-108">Pvz., kai kurie domeno valdikliai nepasiekiami naudojant "Azure AD Connect" arba [būtini prievadai](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-ports) yra blokuojami užkardos – reikia tai pataisyti užtikrindami, kad ryšys tarp "Azure AD Connect" serverio ir vietinio "Active Directory" veikia tinkamai.</span><span class="sxs-lookup"><span data-stu-id="a40c2-108">For example, some domain controllers are not accessible by Azure AD Connect, or the [ports required](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-ports) are blocked by Firewall - You need to fix this by ensuring that the connectivity between the Azure AD Connect server and the on-premises Active Directory works correctly.</span></span>
- <span data-ttu-id="a40c2-109">"Azure AD Connect" serveris šiuo metu yra sustojimo režimu, dėl kurio serveris negalės naudoti slaptažodžių, kad išspręstumėte problemą, atlikite veiksmus, aprašytus skyriuje " [AZURE AD Connect Sync" slaptažodžių Sinchronizavimo trikčių šalinimas – nesinchronizuojami jokie slaptažodžiai](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization).</span><span class="sxs-lookup"><span data-stu-id="a40c2-109">Azure AD Connect server currently being in staging mode, which will result the server not being able to the password hashes - To troubleshoot the issue, follow the steps described in section [Troubleshoot password synchronization with Azure AD Connect sync - No passwords are synchronized](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization).</span></span>

<span data-ttu-id="a40c2-110">**Slaptažodžių maišos sinchronizavimas neveikia kai kuriems vartotojams**</span><span class="sxs-lookup"><span data-stu-id="a40c2-110">**Password Hash Synchronization does not work for some of my users**</span></span>

1. <span data-ttu-id="a40c2-111">Jei pastebėjote, kad vartotojo slaptažodžio maiša nėra sinchronizuojamas, naudokite "Azure AD Connect" užduotį **Šalinti triktis** , kad sužinotumėte ir išspręstumėte problemą.</span><span class="sxs-lookup"><span data-stu-id="a40c2-111">If you noticed that password hash is not syncing for a user, use the **troubleshoot** task in the Azure AD Connect to investigate and resolve the issue.</span></span> <span data-ttu-id="a40c2-112">Atlikite šias užduotis:</span><span class="sxs-lookup"><span data-stu-id="a40c2-112">Perform the following tasks:</span></span>

    <span data-ttu-id="a40c2-113">a.</span><span class="sxs-lookup"><span data-stu-id="a40c2-113">a.</span></span> [<span data-ttu-id="a40c2-114">Paleiskite trikčių diagnostikos užduotį vediklyje</span><span class="sxs-lookup"><span data-stu-id="a40c2-114">Run the troubleshooting task in the wizard</span></span>](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-objectsync)

    <span data-ttu-id="a40c2-115">b.</span><span class="sxs-lookup"><span data-stu-id="a40c2-115">b.</span></span> [<span data-ttu-id="a40c2-116">Naudokite trikčių diagnostikos "cmdlet", kad ištirtumėte konkretaus naudojimo slaptažodžių maišos sinchronizavimo problemą</span><span class="sxs-lookup"><span data-stu-id="a40c2-116">Use the troubleshooting cmdlet to investigate the password hash syncing issue for a specific use</span></span>](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization)

2. <span data-ttu-id="a40c2-117">Vietinis "Active Directory" vartotojo objektas įgalintas **vartotojui turi pasikeisti slaptažodį kitu registravimosi** parinktimi.</span><span class="sxs-lookup"><span data-stu-id="a40c2-117">The on-premises Active Directory User object is enabled for **User must change password at next logon** option.</span></span> <span data-ttu-id="a40c2-118">Kai ši parinktis įgalinta, vartotojui priskiriamas laikinas slaptažodis ir būsite paraginti pakeisti slaptažodį kitame registravime.</span><span class="sxs-lookup"><span data-stu-id="a40c2-118">When this option is enabled, the user is assigned a temporary password and will be prompted to change the password on the next logon.</span></span> <span data-ttu-id="a40c2-119">"Azure AD Connect" nesinchronizuoja laikinųjų slaptažodžių "Azure AD".</span><span class="sxs-lookup"><span data-stu-id="a40c2-119">Azure AD Connect does not synchronize temporary passwords to Azure AD.</span></span>

<span data-ttu-id="a40c2-120">Norėdami išspręsti šią problemą, atlikite vieną iš šių užduočių:</span><span class="sxs-lookup"><span data-stu-id="a40c2-120">To resolve the above issue, perform either of the following tasks:</span></span>

- <span data-ttu-id="a40c2-121">Paprašykite vartotojo prisijungti prie vietinio programos (pvz., "Windows" darbalaukio) ir pakeiskite slaptažodį.</span><span class="sxs-lookup"><span data-stu-id="a40c2-121">Ask the user to sign in to on-premises application (for example, Windows Desktop) and change the password.</span></span> <span data-ttu-id="a40c2-122">Naujasis slaptažodis bus sinchronizuojamas su "Azure AD".</span><span class="sxs-lookup"><span data-stu-id="a40c2-122">The new password will be synchronized to Azure AD.</span></span>
- <span data-ttu-id="a40c2-123">Administratorius turi atnaujinti vartotojo slaptažodį neįjungus parinkties **vartotojas turi pakeisti slaptažodį kitu prisijungimo metu** ir bendrinti naują slaptažodį su vartotoju.</span><span class="sxs-lookup"><span data-stu-id="a40c2-123">Have an administrator update the user's password without enabling the option **User must change password at next logon**, and share the new password with the user.</span></span>

3. <span data-ttu-id="a40c2-124">Vietinio "Active Directory" vartotojo objektas **netinkamai sukonfigūruotas** objekto sinchronizacijai arba slaptažodžių sinchronizacijai.</span><span class="sxs-lookup"><span data-stu-id="a40c2-124">The on-premises Active Directory User object is **not correctly configured** for object synchronization or password synchronization.</span></span> <span data-ttu-id="a40c2-125">Norėdami pašalinti šią problemą, atlikite veiksmus, aprašytus skyriuje [slaptažodžių maišos Sinchronizavimo trikčių šalinimas naudojant "AZURE AD Connect Sync](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization)".</span><span class="sxs-lookup"><span data-stu-id="a40c2-125">To troubleshoot this issue, follow the steps described in the [Troubleshoot password hash synchronization with Azure AD Connect sync](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization).</span></span>







