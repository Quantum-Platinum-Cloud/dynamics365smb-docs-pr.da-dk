---
title: Registrere og refundere medarbejdernes udgifter
description: 'Bogfør medarbejdernes udgifter med finanskladden til medarbejderens konto, og bogfør senere en betaling til medarbejderens bankkonto for at refundere for de forretningsrelaterede udgift.'
author: SorenGP
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: reimbursement
ms.search.form: '63, 234, 625, 5224, 5237, 5238, 5239, 5240'
ms.date: 06/16/2021
ms.author: edupont
---
# <a name="record-and-reimburse-employees-expenses" />Registrere og refundere medarbejdernes udgifter

[!INCLUDE[prod_short](includes/prod_short.md)] understøtter transaktioner for medarbejdere på samme måde som for kreditorer. Derfor findes der medarbejderbogføringsgrupper for at sikre, at medarbejderposter bogføres på de relevante konti i regnskabet.

> [!NOTE]  
> Medarbejdertransaktioner kan kun bogføres i den lokale valuta. Refusion af betalinger til medarbejdere understøtter ikke rabatter og betalingstolerancer.

Hvis medarbejdere bruger deres egne penge under forretningsaktiviteter, kan du bogføre udgiften til medarbejderens konto. Du kan derefter refundere medarbejderen ved at foretage en betaling til medarbejderens bankkonto, på samme måde som når du betaler leverandører.  

> [!TIP]
> I denne artikel forklares det, hvordan du registrerer udgiften i bøgerne og refunderer medarbejderen. Din organisation kan have en portal eller app, som medarbejderne kan sende deres udgiftsrapporter til.

[!INCLUDE [prod_short](includes/prod_short.md)] er fleksibel nok til at dække mange forskellige fremgangsmåder. De nøjagtige kontonumre, der skal bruges, afhænger af organisationens konfiguration og processer.  

## <a name="to-record-an-employees-expense" />Sådan registrerer du en medarbejders udgift

Du bogfører medarbejdernes udgifter på siden **Finanskladde**.

1. Vælg ![Lightbulb, der åbner funktionen Fortæl mig.](media/ui-search/search_small.png "Fortæl mig, hvad du vil foretage dig") ikon, skriv **Finanskladder**, og vælg derefter det relaterede link.  
2. Åbn det relevante finanskladdenavn. Du kan finde flere oplysninger i [Arbejde med finanskladder](ui-work-general-journals.md).
3. Udfyld felterne efter behov på en ny kladdelinje. [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]  

    > [!NOTE]
    > [!INCLUDE[journal-showhide-columns-inline-tip](includes/journal-showhide-columns-inline-tip.md)]
4. Gentag trin 3 for alle de udgifter, som er påløbet medarbejderen.

    > [!TIP]  
    > Hvis du vil angive flere udgiftslinjer over én modkontolinje for medarbejderens bankkonto, skal du markere afkrydsningsfeltet **Foreslå modkontobeløb** på linjen for kørslen på siden **Finanskladdenavne**. Feltet **Beløb** på modkontolinjen udfyldes derefter automatisk med den værdi, der skal bruges til at afstemme udgifterne.
5. Vælg handlingen **Bogfør** for at registrere udgifter på medarbejderens konto.

## <a name="to-reimburse-an-employee" />Sådan refunderer du en medarbejder

Du refunderer medarbejdere ved at bogføre betalinger til deres bankkonto på siden **Udbetalingskladde**.  

1. Vælg ![Lightbulb, der åbner funktionen Fortæl mig.](media/ui-search/search_small.png "Fortæl mig, hvad du vil foretage dig") ikon, skriv **Udbetalingskladder**, og vælg derefter det relaterede link.
2. Åbn den relevante udbetalingskladdekørsel. Du kan finde flere oplysninger i [Arbejde med finanskladder](ui-work-general-journals.md).
3. Udfyld felterne efter behov. Du kan finde flere oplysninger i [Foretage betalinger](payables-make-payments.md).
4. Du kan også vælge handlingen **Foreslå medarbejderbetaling** for automatisk at indsætte kladdelinjerne for ventende medarbejderrefusioner.
5. Vælg handlingen **Bogfør** for at registrere refusionen.  

## <a name="to-reconcile-reimbursements-with-employee-ledger-entries" />Sådan afstemmes refusioner med medarbejderposter

Du udligner medarbejderbetalinger til deres relaterede åbne medarbejderposter på samme måde som for kreditorbetalinger, f.eks. på siden **Betalingsudligningskladde**, baseret på de relaterede bankkontoudtogsposter. Du kan finde flere oplysninger i [Udligne betalinger automatisk og afstemme bankkonti](receivables-apply-payments-auto-reconcile-bank-accounts.md). Du kan også udligne manuelt på siden **Medarbejderposter**. Du kan finde flere oplysninger i det relaterede emne [Afstemme kreditorbetalinger med udbetalingskladden eller fra kreditorposter](payables-how-apply-purchase-transactions-manually.md).  

## <a name="see-also" />Se også

[Bogføre transaktioner direkte i finansposterne](finance-how-post-transactions-directly.md)  
[Arbejde med finanskladder](ui-work-general-journals.md)  
[Tilbageføre kladdeposteringer og annullere modtagelser/leverancer](finance-how-reverse-journal-posting.md)  
[Finans](finance.md)  
[Arbejd med [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)  


[!INCLUDE[footer-include](includes/footer-banner.md)]
