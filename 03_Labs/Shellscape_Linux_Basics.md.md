---
type: lab
platform: Shellscape
active_track: 🌐 Networking Tools
status: In Progress
overall_progress: 8/31
linux_progress: 8/8
network_progress: 0/6
crypto_progress: 0/7
web_progress: 0/5
forensics_progress: 0/5
date_started: 2026-07-03
---

# Lab: Linux Terminal Basis (Shellscape)

## 1. Doelstelling

Het opbouwen van command-line reflexen, begrijpen van de Linux mappenstructuur en het leren navigeren en manipuleren van bestanden via een virtuele shell.

## 2. De "Ninja" Commando-tabel

_Vul deze tabel aan naarmate je verder komt in de 31 levels._

| **Commando**         | **Wat doet het?**                                   | **Praktisch Voorbeeld (Shellscape)** |
| -------------------- | --------------------------------------------------- | ------------------------------------ |
| ls                   | Toont bestanden en mappen                           | ls                                   |
| cd                   | Wisselen van map                                    | cd documents                         |
| cat                  | Leest de inhoud van een bestand                     | cat secret.txt                       |
| pwd                  | Toont de huidige maplocatie                         | pwd                                  |
| ls -l                |                                                     |                                      |
| ls -a                | laat alle bestand zien in jouw directery            |                                      |
| grep                 | Het kan super snel door vinden wat je zoekt in een  |                                      |
| find . -name ".key*" |                                                     |                                      |

## 3. Belangrijke Concepten & Inzichten

_Schrijf hier in je eigen woorden korte aantekeningen over concepten die je tijdens de levels leert. Bijvoorbeeld:_

-- **Absoluut vs. Relatief pad:** Een absoluut pad begint altijd bij de root (`/`) en werkt onafhankelijk van waar je staat. Een relatief pad navigeert vanaf de map waar je op dat moment in werkt.
    
- **De Wildcard (`*`):** Het sterretje is een wildcard (globbing) die door de shell wordt vertaald naar "alles". Bij `grep flag *` vervangt de shell de `*` door alle niet-verborgen bestanden in de huidige map voordat het zoekcommando wordt uitgevoerd.
    
- **Piping (`|`):** De pipe koppelt de uitgang (Standard Output / STDOUT) van het linker commando rechtstreeks aan de ingang (Standard Input / STDIN) van het rechter commando. Hierdoor kun je krachtige ketens van kleine, gespecialiseerde tools bouwen zonder bestanden op te hoeven slaan.
    
- **Recursief zoeken (`-r`):** Standaard weigert `grep` door mappen te zoeken. Met de `-r` (recursive) vlag dwing je `grep` om door de opgegeven map én alle submappen daaronder te graven om bestanden te scannen.
    
- **SUID-permissie (`rws`):** Set User ID is een speciale Linux-permissie. Het zorgt ervoor dat een programma altijd wordt uitgevoerd met de rechten van de eigenaar van het bestand (meestal root/administrator), in plaats van de rechten van de gebruiker die het opstart.
    
    - **Kleine `s` (`rws`):** SUID is actief en het bestand heeft ook execute (`x`) rechten.
        
    - **Hoofdletter `S` (`rwS`):** SUID is wel ingesteld, maar execute (`x`) rechten ontbreken. Dit duidt meestal op een configuratiefout van de beheerder.
        
- **Sudo (`superuser do`):** Dit is je digitale beveiligingsbadge. Hiermee voer je tijdelijk een commando uit met de hoogste privileges (root) zonder dat je volledig hoeft in te loggen op het gevaarlijke root-account.

## 4. Voortgangslog per Discipline

### ACTIEF: 🐧 Linux Fundamentals (8 levels)

- **SSH Commando:** `ssh level0@linux`
    
- [x] Level 1: Inleiding & navigatie (`ls`, `cd`)
    
- [x] Level 2: Mappenstructuur begrijpen
    
- [x] Level 3: Bestanden lezen (`cat`)
    
- [x] Level 4: Locaties bepalen (`pwd`)
    
- [x] Level 5: Bestanden aanmaken & bewerken
    
- [x] Level 6: Bestanden kopiëren & verplaatsen
    
- [x] Level 7: Bestanden verwijderen
    
- [x] Level 8: Zoeken naar specifieke bestanden
    

### 🔒 VOLGENDE: 🌐 Networking Tools (6 levels)

- **SSH Commando:** `ssh level0@network`
    
- [ ] Levels 9 t/m 14 (Nog niet gestart)
    

### 🔒 VOLGENDE: 🔑 Cryptography (7 levels)

- **SSH Commando:** `ssh level0@crypto`
    
- [ ] Levels 15 t/m 21 (Nog niet gestart)
    

### 🔒 VOLGENDE: 🕷️ Web Security (5 levels)

- **SSH Commando:** `ssh level0@web`
    
- [ ] Levels 22 t/m 26 (Nog niet gestart)
    

### 🔒 VOLGENDE: 🕵️ Digital Forensics (5 levels)

- **SSH Commando:** `ssh level0@forensics`
    
- [ ] Levels 27 t/m 31 (Nog niet gestart)