---
title: Siuntimo perdavimo telkinys
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/08/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3000003"
- "12315"
ms.openlocfilehash: 8750c9036f258d9c5edc94bb027d564140bbd9914712cc1f25ff3abc3f4b9468
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54041594"
---
# <a name="outbound-relay-pool"></a>Siuntimo perdavimo telkinys

"Microsoft" keičia el. laiškų perdavimo arba persiuntimo per Microsoft 365. Tam tikrų scenarijų pranešimai persiunčiami arba perduodami per Microsoft 365 naudojant specialų perdavimo telkinį. Laiškai, siunčiami naudojant perdavimo telkinį, gali būti gavėjo nepageidaujamų laiškų aplanke. Daugiau informacijos žr. [Siuntimo pristatymo telkiniai](/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages#relay-pool)

Norėdami išvengti scenarijaus naudodami perdavimo telkinį, įsitikinkite, kad persiųsti / perduoti laiškai atitinka vieną iš šių kriterijų:

- Siunčiamas siuntėjas yra priimtas nuomotojo domenas.
- Siuntėjo strategijos sistema (SPF) pereina, kai pranešimas Microsoft 365.
- DomainKeys Identified Mail (DKIM) on the P2 sender domain passes when the message comes to Microsoft 365.
 
Pranešimai, kurie atitinka anksčiau nurodytus kriterijus, nėra perteikite per perdavimo telkinį.

Jei jūsų domeno MX įrašas yra nukreiptas į trečiosios šalies arba vietinį serverį, naudokite patobulintą filtravimą, kad įsitikintumėte, jog SPF tikrinimas yra tinkamas gaunamiesiems el. laiškams ir kad el. laiškai nebūtų siunčiami per perdavimo telkinį.

**Kaip sužinoti, ar mus paveikė relės telkinys?**

Jei jūsų persiunčiami arba persiunčiami el. laiškai naudoja vieną iš aukščiau nurodytų kriterijų, pranešimai nebus perduodami per perdavimo telkinį. Tačiau, jei pranešimas siunčiamas per perdavimo telkinį, siuntimo serverio IP yra diapazone 40.95.0.0/16, o siuntimo serverio vardas pavadinime yra **rly.**

