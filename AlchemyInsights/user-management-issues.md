---
title: Vartotojų valdymo problemos
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9209"
- "9005371"
ms.openlocfilehash: 4b61686381de0cafa38857ca7a96b3a81aa191ec
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 03/19/2021
ms.locfileid: "51036286"
---
# <a name="user-management-issues"></a>Vartotojų valdymo problemos

**Kas nutinka dabartiniams priskirtiems vartotojams taikomajai programai, jei išjungsiu ypatybės "vartotojo priskyrimas būtinas" (nustatyti šią ypatybę kaip ne)?**

**Reikia išjungti vartotojo užduotį** , kuri neturi įtakos šiuo metu priskirtiems vartotojams. Išjungus šią ypatybę visi vartotojai galės pasiekti taikomąją programą. Visi nurodyti vartotojai ir vartotojai, priskirti programos grupėms, vis tiek bus galiojantys.

- Norėdami apriboti programą pagal konkretų vartotojų rinkinį, žiūrėkite – ["AZURE AD" taikomosios programos apribojimas vartotojų rinkiniu – "Microsoft" tapatybės platforma | "Microsoft" dokumentai](https://docs.microsoft.com/azure/active-directory/develop/howto-restrict-your-app-to-a-set-of-users#:~:text=Select%20the%20application%20you%20want%2cand%20set%20it%20to%20Yes.).
- Norėdami priskirti vartotojus ir grupes, įmonės taikomąsias programas "Azure Active Directory" ("Azure AD"), iš "Azure" portalo arba naudodami "PowerShell", ieškokite ["Azure Active Directory" taikomosios programos vartotojų priskyrimo valdymas](https://docs.microsoft.com/azure/active-directory/manage-apps/assign-user-or-group-access-portal).
- Jei norite perduoti taikomųjų programų kūrimo ir valdymo teises, žiūrėkite [atstovo taikomųjų programų valdymo administratoriaus teisės – "AZURE AD" | "Microsoft" dokumentai](https://docs.microsoft.com/azure/active-directory/roles/delegate-app-roles).
- **Konkrečių įmonės taikomųjų programų slėpimas iš vartotojų** – atlikite toliau nurodytus veiksmus, kad paslėptumėte visas "Microsoft" 365 taikomąsias programas iš " **myapps** " skydelio. Programos vis tiek bus matomos "Office 365" portale.

 1. Prisijungimas prie "Azure" portalo kaip visuotinis jūsų katalogo administratorius. 
 2. Pasirinkite " **Azure Active Directory**". 
 3. Pasirinkite **vartotojai**. 
 4. Pasirinkite **vartotojo parametrai**. 
 5. Dalyje **įmonės taikomosios programos** spustelėkite **valdyti, kaip galutiniai vartotojai paleidžia ir peržiūri jų taikomąsias programas**. 
 6. **Vartotojai gali matyti tik "office 365" taikomąsias programas "office 365" portale**, spustelėkite **taip**. 
 7. Spustelėkite **Įrašyti**. 
 8. Daugiau informacijos ieškokite "Enterprise" taikomosios programos, skirtos " [AZURE AD", vartotojo funkcijos slėpimas "Microsoft" dokumentai](https://docs.microsoft.com/azure/active-directory/manage-apps/hide-application-from-user-portal#:~:text=%20Hide%20an%20application%20from%20the%20end%20user,6%20Click%20Properties.%207%20Click%20Save.%20See%20More.)

- Jei programinę įrangą kaip paslaugą (SaaS) siūlote daugeliui organizacijų, galite sukonfigūruoti programą taip, kad ji priimtų prisijungimo programą iš bet kurio "Azure Active Directory" ("Azure AD") nuomotojo. Ši konfigūracija vadinasi "jūsų taikomosios programos kelių nuomotojų pateikimas". Visi "Azure AD" nuomotojo vartotojai galės prisijungti prie jūsų programos, gavę sutikimą naudoti savo paskyrą su jūsų programėle. Daugiau informacijos ieškokite ["AZURE AD" vartotojų prisijungimo programų kūrimas – "Microsoft" tapatybės platforma | "Microsoft" dokumentai](https://docs.microsoft.com/azure/active-directory/develop/howto-convert-app-to-be-multi-tenant).

- **Kaip galutinis vartotojas gali pasiekti taikomąją programą, kai jis/ji priskiriama taikomajai programai?**

Kiekviena "Enterprise" taikomosios programos disko programa turi saitą galutiniams vartotojams pasiekti. Vartotojai taip pat gali lengvai pasiekti programėlę naudodami " **Myapps** " portalą.

- **Norite sužinoti, kurias taikomąsias programas ir taikomųjų programų tipus naudoja vartotojai?**

Galite atsisiųsti pastarųjų 30 dienų prisijungimo ataskaitas iš **portal.azure.com > "Azure Active Directory"> Signins> atsisiųsti ataskaitas**.

- Sužinokite, kaip [suteikti nuomotojo plačios versijos administratoriaus sutikimą taikomajai programai](https://docs.microsoft.com/azure/active-directory/manage-apps/grant-admin-consent) ir [Konfigūruoti, kaip galutiniai vartotojai sutinka su taikomosiomis programomis](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent).

- Supraskite, [kaip veikia sutikimas](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent) ir [valdykite taikomųjų programų sutikimą](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-consent-requests).


