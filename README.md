📌 Descrizione del progetto

Questo progetto universitario, sviluppato in Cisco Packet Tracer, ha come obiettivo la configurazione di una rete locale (LAN) con indirizzi privati che vengono tradotti in indirizzi pubblici dal router tramite NAT (Network Address Translation).

Il router, oltre a gestire il NAT, implementa:
Filtraggio delle connessioni uscenti (firewall) permettendo solo:
traffico UDP sulla porta 53 (DNS)
traffico TCP sulla porta 80 (HTTP)
Port forwarding verso un server interno alla LAN:
tutte le connessioni in ingresso all’IP pubblico del router vengono inoltrate al server interno.

⚙️ Requisiti di progetto

LAN privata con indirizzi IP privati.
Router configurato per:
NAT dinamico per l’accesso a internet.
ACL (Access Control List) per filtrare il traffico in uscita.
Port forwarding verso il server interno.
Server nella LAN raggiungibile dall’esterno tramite il port forwarding.
Client nella LAN in grado di accedere a internet (limitato alle porte consentite).

🔍 Verifica e test

Dalla LAN

✅ È possibile visualizzare un sito web sulla rete pubblica (HTTP porta 80).
❌ Non è possibile collegarsi via TELNET a un server sulla rete pubblica (bloccato dal router).

Dalla rete pubblica

✅ È possibile accedere al server web interno tramite l’IP pubblico del router (grazie al port forwarding).
🗂 Struttura del repository

rete.pkt → File del progetto Packet Tracer con la configurazione completa.


🚀 Come utilizzare il progetto

Aprire il file rete.pkt con Cisco Packet Tracer.
Analizzare la topologia della rete e la configurazione dei dispositivi.
Eseguire i test di verifica descritti sopra per confermare il corretto funzionamento del NAT, ACL e port forwarding.

📖 Note didattiche

Questo progetto mostra un’applicazione pratica di NAT, ACL e port forwarding, concetti fondamentali per la gestione della sicurezza e della connettività in reti reali.
È pensato come esercitazione universitaria per consolidare la comprensione delle funzionalità base dei router Cisco.
