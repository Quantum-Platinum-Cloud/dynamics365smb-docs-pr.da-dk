---
title: Oprette interaktioner for kontakter og målgrupper
description: 'Beskriver, hvordan du kan oprette interaktioner for kommunikation, som du har med kontakter og målgrupper i Business Central, f.eks. direct mail.'
documentationcenter: ''
author: jswymer
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 'relationship, prospect'
ms.search.forms: '5077, 5078, 5074, 5076, 5186, 5075, 5079'
ms.date: 04/01/2021
ms.author: jswymer
---
# <a name="create-interactions-on-contacts-and-segments" />Oprette interaktioner for kontakter og målgrupper
Du kan oprette interaktioner for at registrere al interaktion og kommunikation, som du har med kontakter og målgrupper, f.eks. direct mail.

Du kan først oprette interaktioner, når du har defineret interaktionsskabeloner. Du kan finde flere oplysninger i [Definere interaktionsskabeloner](marketing-interactions.md).

## <a name="to-create-an-interaction" />Sådan oprettes en interaktion
1. Åbn kontakt-, sælger- eller interaktionslogposten.
2. Vælg handlingen **Opret interaktion**.
3. Udfyld felterne, og vælg derefter knappen **OK**.

> [!NOTE]  
>   Hvis du vil udføre en anden opgave, før du afslutter interaktionen, kan du vælge **Annuller** og derefter vælge at afslutte interaktionen på et senere tidspunkt. Dette udsætter interaktionen.

## <a name="to-finish-and-delete-postponed-interactions" />Sådan afsluttes og slettes udsatte interaktioner
1. Åbn kontakt-, sælger- eller interaktionslogposten.
2. Vælg **Udsatte interaktioner**.
3. Marker den interaktion, som du vil afslutte, og klik derefter på handlingen **Fortsæt**.

## <a name="to-create-an-interaction-on-a-segment" />Sådan oprettes en interaktion for en målgruppe
1. Vælg ![Lightbulb, der åbner funktionen Fortæl mig.](media/ui-search/search_small.png "Fortæl mig, hvad du vil foretage dig") ikon, skriv **Segmenter**, og vælg derefter det relaterede link.
2. Udfyld felterne i sektionen **Interaktion** på siden **Målgruppe** for at angive, hvilken interaktion du vil knytte til målgruppen.

    Når du har tildelt en interaktion til målgruppe, kan du tilpasse interaktionen til hver kontakt i målgruppen. Du kan f.eks. vælge en anden interaktionsskabelon på linjerne på siden **Målgruppe**.  
3. Hvis du vil logge målgruppen og interaktionerne, skal du vælge handlingen **Log**. Siden **Gemt målgruppe** åbnes.
4. Hvis du vil oprette en ny målgruppe, der indeholder de samme kontakter, skal du markere afkrydsningsfeltet **Opret opfølgningsmålgruppe**. Du kan kun oprette en opfølgningsmålgruppe, hvis du har angivet nummerserier for målgrupper på siden **Marketingopsætning**.

Der gemmes en interaktion, der er registreret for hver kontakt i målgruppen, i tabellen **Interaktionslogpost**, og målgruppen logges. Logførte målgrupper vises på siden **Gemte målgrupper**.

Hvis du har markeret afkrydsningsfeltet **Opret opfølgningsmålgruppe**, oprettes der automatisk en ny målgruppe, der indeholder de samme kontakter som den målgruppe, du netop har gemt.

## <a name="see-also" />Se også
[Registrere interaktioner](marketing-interactions.md)  
[Administrere kontakter](marketing-contacts.md)  
[Administrere salgsleads](marketing-manage-sales-opportunities.md)  
[Arbejde med Business Central](ui-work-product.md)


[!INCLUDE[footer-include](includes/footer-banner.md)]
