---
title: Prisijungimas prie "Windows 10" nenaudojant slaptažodžio
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001690"
- "3766"
ms.openlocfilehash: 1c03f00f7b41ea16d3106b19b998edeea6114603
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 04/15/2021
ms.locfileid: "51830554"
---
# <a name="sign-in-to-windows-10-without-using-a-password"></a><span data-ttu-id="f125c-102">Prisijungimas prie "Windows 10" nenaudojant slaptažodžio</span><span class="sxs-lookup"><span data-stu-id="f125c-102">Sign-in to Windows 10 without using a password</span></span>

<span data-ttu-id="f125c-103">Kad nereikėtų įvesti slaptažodžio "Windows" paleisties metu, rekomenduojame naudoti vieną iš "Windows Hello" saugaus prisijungimo parinkčių, pvz., PIN, veido atpažinimo arba pirštų atspaudo, jei yra.</span><span class="sxs-lookup"><span data-stu-id="f125c-103">To avoid having to type a password at Windows startup, we recommend you use one of the Windows Hello secure sign-in options, like a PIN, face recognition, or fingerprint, if available.</span></span> <span data-ttu-id="f125c-104">Jei tikrai norite išjungti saugų prisijungimą, žr. toliau pateiktas instrukcijas "Automatinis prisijungimas prie "Windows 10".</span><span class="sxs-lookup"><span data-stu-id="f125c-104">If you really want to disable secure sign-in, see the "Automatically sign in to Windows 10" instructions below.</span></span>

<span data-ttu-id="f125c-105">**Apsaugokite "Windows Hello" paskyros slaptažodžio alternatyvas**</span><span class="sxs-lookup"><span data-stu-id="f125c-105">**Secure Windows Hello alternatives to the account password**</span></span>

<span data-ttu-id="f125c-106">Eikite **į Parametrai > Paskyros > prisijungimo parinktys** (arba spustelėkite [čia](ms-settings:signinoptions?activationSource=GetHelp)).</span><span class="sxs-lookup"><span data-stu-id="f125c-106">Go to **Settings  > Accounts > Sign-in options** (or click [here](ms-settings:signinoptions?activationSource=GetHelp)).</span></span> <span data-ttu-id="f125c-107">Bus išvardytos galimos prisijungimo parinktys.</span><span class="sxs-lookup"><span data-stu-id="f125c-107">Available sign-in options will be listed.</span></span> <span data-ttu-id="f125c-108">Toliau pateikiami pavyzdžiai.</span><span class="sxs-lookup"><span data-stu-id="f125c-108">For example:</span></span>

![Prisijungimo parinktys.](media/sign-in-options.png)

<span data-ttu-id="f125c-110">Spustelėkite arba bakstelėkite vieną iš parinkčių, kad jį sukonfigūruotų.</span><span class="sxs-lookup"><span data-stu-id="f125c-110">Click or tap one of the options to configure it.</span></span> <span data-ttu-id="f125c-111">Kai kitą kartą pradėsite arba atrakinsite "Windows", galėsite naudoti naują parinktį, o ne slaptažodį.</span><span class="sxs-lookup"><span data-stu-id="f125c-111">Next time you start or unlock Windows, you will be able to use the new option instead of a password.</span></span> 

<span data-ttu-id="f125c-112">**Automatinis prisijungimas prie "Windows 10"**</span><span class="sxs-lookup"><span data-stu-id="f125c-112">**Automatically sign-in to Windows 10**</span></span>

<span data-ttu-id="f125c-113">**Pastaba:** automatinis prisijungimas yra patogus, tačiau kelia pavojų saugai, ypač jei jūsų kompiuterį gali pasiekti keli žmonės.</span><span class="sxs-lookup"><span data-stu-id="f125c-113">**Note**: Automatic sign-in is convenient, but introduces a security risk, especially if your PC is accessible by multiple people.</span></span> 

1. <span data-ttu-id="f125c-114">Užduočių juostoje **spustelėkite arba** bakstelėkite mygtuką Pradžia.</span><span class="sxs-lookup"><span data-stu-id="f125c-114">Click or tap the **Start** button in the Taskbar.</span></span>

2. <span data-ttu-id="f125c-115">Įveskite **netplwiz ir** paspauskite klavišą Enter, kad atidarytumėte langą Vartotojų paskyros.</span><span class="sxs-lookup"><span data-stu-id="f125c-115">Type **netplwiz** and hit the Enter key to open the User Accounts window.</span></span>

3. <span data-ttu-id="f125c-116">Vartotojų **paskyrose** spustelėkite paskyrą, prie kurios norite automatiškai prisijungti, kai paleidžiama "Windows".</span><span class="sxs-lookup"><span data-stu-id="f125c-116">In **User Accounts**, click the account you want to automatically sign in to when Windows starts.</span></span>

4. <span data-ttu-id="f125c-117">Panaikinkite žymės langelio "Vartotojai turi įvesti vartotojo vardą ir slaptažodį, kad galėtų naudoti šį kompiuterį" žymėjimą.</span><span class="sxs-lookup"><span data-stu-id="f125c-117">Uncheck the "Users must enter a user name and password to use this computer" checkbox.</span></span>

    ![Vartotojai turi įvesti vartotojo vardo ir slaptažodžio parinktį.](media/users-must-enter-username.png)

5. <span data-ttu-id="f125c-119">Spustelėkite **Gerai**.</span><span class="sxs-lookup"><span data-stu-id="f125c-119">Click **OK**.</span></span> <span data-ttu-id="f125c-120">Jūsų bus paprašyta įvesti ir patvirtinti pasirinktos paskyros slaptažodį.</span><span class="sxs-lookup"><span data-stu-id="f125c-120">You will be asked to enter and confirm the password for the account you selected.</span></span> <span data-ttu-id="f125c-121">Spustelėkite **Gerai,** kad baigtumėte.</span><span class="sxs-lookup"><span data-stu-id="f125c-121">Click **OK** to finish.</span></span> <span data-ttu-id="f125c-122">Kai kitą kartą paleidžiama "Windows 10", ji automatiškai prisijungsite prie pasirinktos paskyros.</span><span class="sxs-lookup"><span data-stu-id="f125c-122">Next time Windows 10 starts, it will automatically sign in to the account you selected.</span></span>
