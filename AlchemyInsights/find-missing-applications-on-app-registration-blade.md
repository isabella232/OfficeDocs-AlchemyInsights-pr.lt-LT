---
title: Trūkstamų taikomųjų programų radkite "App Registration" ašmenyse
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004352"
- "9654"
ms.openlocfilehash: 00b5821e2edad8b60ff60b1f85264d81c72277e4
ms.sourcegitcommit: 1f43598a726cdb9904aa501eb8db87f143020d9e
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 03/23/2021
ms.locfileid: "51404698"
---
# <a name="find-missing-applications-on-app-registration-blade"></a>Trūkstamų taikomųjų programų radkite "App Registration" ašmenyse

1. Nepavyksta rasti taikomųjų programų programų registracijos portale.

    Jei programa yra kelių nuomotojų taikomoji programa ir ji buvo užregistruota kitame nuomotoje, ji nebus rodoma dalyje Taikomosios programos registracijos ašmenys. Tačiau galite jį rasti dalyje "Enterprise Applications" ašmenys, kai jis bus atvertas (sutikus) ir jūsų nuomotoje bus sukurtas pagrindinis paslaugos punktas. Daugiau informacijos žr. "Azure AD" & paslaugų teikimo [principai – "Microsoft" tapatybės platforma](https://docs.microsoft.com/azure/active-directory/develop/app-objects-and-service-principals).
2. Nepavyksta peržiūrėti programėlių "App Registration" ašmenyje, net jei esate administratorius.

    Įsitikinkite, kad esate tinkamame "Azure" portalo kataloge.
3. Mano taikomoji programa nėra įtraukta į "Enterprise Applications" ašmenį, bet rodoma, kai pateikiau užklausą "PowerShell" komandai.

    Kartais, kai panaikinate taikomąją programą iš "Azure" portalo, ji nerodo portale, bet gali būti, kad ji nebuvo visiškai panaikinta. Daugiau informacijos rasite:
    - Galite gauti anksčiau panaikintų programų sąrašą ir pamatyti, ar programa rodoma sąraše, naudodami "PowerShell" komandą: **Get-AzureADDeletedApplication**. Norėdami sužinoti daugiau, [žr. Get-AzureADDeletedApplication (AzureAD)](https://docs.microsoft.com/powershell/module/azuread/get-azureaddeletedapplication).
    - Jei norite visiškai pašalinti taikomąją programą, galite išbandyti šiuos veiksmus programoje "PowerShell": **Remove-AzureADApplication -ObjectId**. Norėdami sužinoti daugiau, [žr. "AzureADApplication" pašalinimas ("AzureAD")](https://docs.microsoft.com/powershell/module/azuread/remove-azureadapplication).
    - Taip pat galite pabandyti atkurti panaikintą taikomąją programą naudodami šią "PowerShell" komandą: **Atkurti AzureADDeletedApplication -ObjectId**. Norėdami sužinoti daugiau, [žr. Restore-AzureADDeletedApplication (AzureAD)](https://docs.microsoft.com/powershell/module/azuread/restore-azureaddeletedapplication).
4. Negaliu rasti visų iš anksto įdiegtų įmonės taikomųjų programų sąrašo naujame "Azure" nuomotoje.

    Pagal numatytuosius nustatymus "Azure AD" nėra iš anksto įdiegtų įmonės taikomųjų programų. Turite įtraukti ją rankiniu būdu iš parinkties "Nauja taikomoji programa", naršydami ją iš "Azure AD" galerijos arba įtraukdami ne galerijos taikomąją programą. Norėdami sužinoti daugiau, [žr. "Quickstart": taikomosios programos įtraukimas į "Azure Active Directory" ("Azure AD") nuomotoją.](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal)
    Jei esate visuotinis administratorius, galite lengvai pasiekti savo programas naudodami ["Microsoft 365" taikomųjų programų vykdyklę](https://docs.microsoft.com/microsoft-365/admin/manage/customize-the-app-launcher).
5. Nepavyksta rasti mano programėlių mano programėlių portale.

    Įsitikinkite, kad taikomosios programos nėra paslėptos puslapyje Mano taikomosios programos rinkinys. Norėdami sužinoti daugiau, [žr. Rinkiniai (peržiūra) mano programų portale – "Azure AD".](https://docs.microsoft.com/azure/active-directory/user-help/my-apps-portal-user-collections)
6. Norėdami paleisti programėles iš portalo Mano programėlės, [žr. & programėlių radimas mano programų portale – "Azure AD".](https://docs.microsoft.com/azure/active-directory/user-help/my-apps-portal-end-user-access)
7. Įdiegus "Office 365 Mover" programa nerodoma "Enterprise Applications" ašmenyse.

    "Office 365 Mover" programa yra daugialypis taikomoji programa, kurios nereikia įtraukti į AAD naudojant skyrių Galerijos taikomosios programos dalyje "Enterprise App Registration". Norėdami pasiekti "Office 365 Mover" programą, tiesiog prisijunkite prie taikomosios programos ir prašys vartotojo sutikimo dėl teisių. Kai vartotojas pateikia sutikimą, ši programa automatiškai bus įtraukta į nuomotoją su jūsų prisiregistravęs el. pašto ID.

    Prisijungę prie taikomosios programos, galėsite rasti šios taikomosios programos įrašą AAD dalyje Įmonės taikomųjų programų ašmenys. Tos taikomosios programos reikia ieškoti įvesdami vardą ir pavardę, t. y. "Office 365 Mover" arba tiesiog ieškokite "office" ir joje turėtų būti programos sąrašas. Norėdami sužinoti daugiau, žr. ["Office 365 Mover"](https://docs.microsoft.com/answers/questions/30186/office-365-mover-says-its-already-installed-but-it.html)sako, kad jis jau įdiegtas, bet jis nėra nurodytas "Enterprise" taikomųjų programų galerijoje .
8. "Quickstart": peržiūrėkite programų, kurios naudoja ["Azure Active Directory" ("Azure AD")](https://docs.microsoft.com/azure/active-directory/manage-apps/view-applications-portal) nuomotoją tapatybės valdymui, sąrašą, kuriame rodoma, kaip peržiūrėti taikomąsias programas, dar vadinamas programomis, kurios jau nustatytos naudoti "Azure AD" nuomotoją kaip tapatybės teikėją (IDP).
9. [Dažnai pasitaikančių problemų įtraukiant arba šalinant taikomąją programą į "Azure Active Directory"](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-adding-apps) šalinimas padeda suprasti įprastas problemas, su kuriomis žmonės susiduria peržiūrėdami programas "Azure Active Directory".
