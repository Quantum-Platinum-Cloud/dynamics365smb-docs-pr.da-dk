---
title: Udvidelsen Overførsel af QuickBooks-data
description: 'Beskriver, hvordan du bruger udvidelsen til at importere debitorer, kreditorer, varer og konti fra QuickBooks Desktop til Business Central.'
author: edupont04
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 'app, add-in, manifest, customize, import, implement'
ms.search.form: '1911, 1912, 1913, 1914, 1915, 1916, 1918, 1919'
ms.date: 06/24/2021
ms.author: edupont
---

# <a name="the-quickbooks-data-migration-extension" />Udvidelsen Overførsel af QuickBooks-data

Denne udvidelse gør det nemt at overflytte debitorer, kreditorer, varer og konti fra QuickBooks til [!INCLUDE[prod_short](includes/prod_short.md)]. Hvis din virksomhed bruger QuickBooks i dag, kan du eksportere de relevante oplysninger og derefter åbne en assisteret opsætningsvejledning for at overføre dataene til [!INCLUDE[prod_short](includes/prod_short.md)].  
Du kan finde flere oplysninger i [Importere virksomhedsdata fra andre økonomisystemer](across-import-data-configuration-packages.md).

## <a name="data-from-quickbooks-desktop" />Data fra QuickBooks Desktop

Du kan importere følgende data fra QuickBooks Online til Business Central:

- Kunder (Debitorer)  
- Leverandører (Kreditorer)  
- Varer  
- Kontoplan  
- Primosaldopostering i regnskabet  
- Disponible antal for lagervarer  
- Åbne dokumenter for debitorer og kreditorer, f.eks. fakturaer, kreditnotaer og betalinger  

Vi overfører kun fulde beløb på salgs- og købsdokumenter. Delvist betalte beløb opdateres ikke. F.eks. hvis en debitor har indbetalt 300 af i alt 500 dollar på en salgsfaktura, overfører vi hele 500. Hvis du har modtaget delbetalinger, skal du opdatere dem manuelt, før eller efter at du overfører data. Det anbefales, at du anvender udestående transaktioner, inden du overfører, for at gøre tingene nemmere bagefter.

> [!NOTE]
> Vi overfører ikke indkøbsordrer eller salgsordrer.

## <a name="before-you-start" />Før du starter

Det er en vigtig del af overførslen at angive de konti, transaktioner skal overføres til. Det er en god ide at planlægge denne tilknytning, før du overfører data. F.eks. de konti, hvor du bogfører poster for:

- Salget af varer eller servicer til debitorer  
- Køb af varer eller servicer fra kreditorer  
- Ændringer i finansbogholderiet  

Business Central kræver, at finanskonti har kontonumre tilknyttet. Sørg for, at kontonumre er tildelt til kontiene i QuickBooks.
Hvis der er transaktioner i QuickBooks, der har momsbeløb, du skal oprette en momskonto for dine skatteregioner i Business Central, før du kan bogføre transaktioner.

For at få data ud af programmet QuickBooks Desktop skal du hente værktøjet Microsoft-dataeksportværktøjet.  Instruktioner til værktøjet findes i dataoverførselsguiden i [!INCLUDE[prod_short](includes/prod_short.md)]. Værktøjet opretter forbindelse til programmet QuickBooks og eksportere de relevante oplysninger til en .zip-fil.  

> [!NOTE]
> I øjeblikket fungerer dataeksportværktøjet kun sammen med QuickBooks 2017 og 2018.

## <a name="finding-the-quickbooks-data-migration-extension" />Sådan finder du udvidelsen Overførsel af QuickBooks-data

Udvidelsen Overførsel af QuickBooks-data er installeret og klar til brug som en integreret del af den assisterende opsætningsvejledning til dataoverførsel. Hvis du er klar til at komme i gang nu og har eksporteret dine data fra QuickBooks, skal du vælge ![lightbulb, der åbner funktionen Fortæl mig.](media/ui-search/search_small.png "Fortæl mig, hvad du vil foretage dig") ikon, angiv **Assisteret opsætning** og vælg derefter det relaterede link. Vælg **Overflyt forretningsdata**, og følg derefter trinnene i vejledningen.  

## <a name="what-do-i-do-after-i-migrate-data" />Hvad gør jeg gøre, når jeg har overført data?

Når du har overført data, har transaktioner status Ikke-bogførte, så du kan gennemgå dem og foretage ændringer. For at få vist transaktionerne skal du gå til siden, hvor du vil finde dem normalt. F.eks. for at få vist ikke-bogførte salgsfakturaer, skal du gå til siden Salgsfakturaer. For at få vist udbetalingskladder skal du gå til siden Udbetalingskladder.
Der er især nogle ting, du skal gøre: Hvis transaktionerne i QuickBooks havde avance- eller rabatbeløb, skal du manuelt føje beløbene til de relaterede transaktioner i Business Central, før du bogfører dem.
Hvis du bruger moms, skal du evt. tilføje en virksomhedsbogføringsgruppe og en produktbogføringsgruppe i bogføringsopsætningen, så du kan bogføre momsbeløb.
Kontroller primosaldi for konti i finansbogholderiet. QuickBooks gemmer ikke den aktuelle saldo for alle konti, så det kan være nødvendigt at rette primosaldi.

## <a name="see-related-microsoft-trainingtrainingmodulesmigrate-data-dynamics-365-business-central" />Se relateret [Microsoft-træning](/training/modules/migrate-data-dynamics-365-business-central/)

## <a name="see-also" />Se også

[Import af virksomhedsdata fra andre økonomisystemer](across-import-data-configuration-packages.md)  
[Tilpasse [!INCLUDE[prod_short](includes/prod_short.md)] ved hjælp af udvidelser](ui-extensions.md)  

[!INCLUDE[footer-include](includes/footer-banner.md)]
