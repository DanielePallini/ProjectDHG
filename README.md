# Guida all'installazione delle macchine virtuali

Per installare le macchine virtuali che sono alla base dell'infrastruttura sicura, è necessario installare sul proprio computer un software per l'esecuzione di macchine virtuali, come _VirtualBox_.

I file OVA delle due macchine virtuali sono disponibili al seguente link di google drive: [link](https://www.google.it/).

Una volta installate, è possibile avviare le due macchine e testare l'intero sistema.

La prima macchina virtuale, denominata Dual-homed Host, svolge i compiti di uno Screening Router e di un Bastion Host. Al suo avvio, l'utente può accedere ad uno dei due account disponibili: 
* **screening**: account con permessi di root, necessario per l’implementazione e la gestione delle policy e della sicurezza di tutta l’infrastruttura. È riservato all’amministratore di sistema. La password per poter accedere a tale account è: univpm2223.
* **guest**: account senza permessi di root, predisposto per l'accesso via SSH degli utenti. La password per poter accedere a tale account è: guestscreening.

La seconda macchina virtuale, la macchina "Client", simula il comportamento di una macchina appartenente alla rete interna. Al suo avvio, l'utente può accedere ad uno dei due account disponibili:
* **client**: account con permessi di root, necessario per la gestione e il controllo dei file presenti sulla macchina. È riservato all’amministratore di sistema. La password per poter accedere a tale account è: gruppo8.
* **guest**: account senza permessi di root, predisposto per l’accesso via SSH degli utenti. La password per poter accedere a tale account è: guestclient.

Tramite queste macchine, sarà possibile eseguire personalmente alcuni test sull'infrastruttura. Alcuni esempi di test sono riportati nel Capitolo 4 del file PDF.
