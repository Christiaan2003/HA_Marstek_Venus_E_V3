Home Assistant – Marstek Venus E V3.0 Local API Integratie

Deze repository is bedoeld voor een custom Home Assistant integratie voor het Marstek Venus E V3.0 thuisbatterijsysteem.  
De integratie communiceert met de batterij via de Local API over UDP, die geactiveerd kan worden via de Marstek mobiele app.

Belangrijk:

* Deze integratie gebruikt de RS485-poort niet.  
* Zodra de Local API is ingeschakeld, werkt de communicatie functioneel hetzelfde als RS485 (Modbus), maar dan via je lokale netwerk (LAN/WiFi).  
* Dit voorkomt de noodzaak voor RS485-adapters, ESP-boards of extra bekabeling.  

Huidige status

Dit project is nog in ontwikkeling.  
Het doel is om volledige ondersteuning te bieden voor het uitlezen van batterijgegevens in Home Assistant, inclusief integratie met het Energie-dashboard.

API Activeren (Vereist)

Om deze integratie in de toekomst te gebruiken, moet je eerst zorgen dat de Local API is ingeschakeld op je Marstek Venus E V3.0:

1. Open de Marstek app.  
2. Ga naar Feedback / Support.  
3. Vraag een firmware-update aan (minimaal V137 of nieuwer).  
4. Vraag support om de Local API voor je apparaat te activeren.  

Zodra dit is ingeschakeld, verschijnt er een nieuw menu in de app:  
Instellingen → Geavanceerde functies → Local API  
Hier kun je de Local API aanzetten en de UDP-poort instellen (standaard 30000).  

Voorbeeld bericht (max 500 tekens)

Hallo Marstek team, bedankt voor de firmware-updates. Kunt u de Local API activeren voor mijn Venus E V3.0 batterij (S/N: XXXXX)? Ik wil graag de UDP Local API op poort 30000 gebruiken voor integratie met mijn smart home systeem. Met vriendelijke groet.

Opmerking

Deze repository dient momenteel als een ontwikkelbasis en documentatiehub.  
Naarmate de integratie vordert, zullen installatie- en configuratiedetails worden toegevoegd.
