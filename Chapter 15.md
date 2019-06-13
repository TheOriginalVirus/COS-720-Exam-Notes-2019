# __Chapter 15__


## __Overview__
   - Types of attacks
   - DDoS attacks (Syn Flood/DDoS -Firewall - Scrubbing)
   - DDoS - volumetric attack - amplification attack - Memchached servers, GitHub case

   - Read the paper "The evolution of DDos" <-- IMPORTANT

   - Intrusion Detection Systems
   - Honeypots


## __Two types of attacks:__

    - Non Technical
    - Technical

## __Types of Technical Attacks__
    - DDoS: Attacker gets access to a number of computers. PC's wil target single host.server.
    - DOS

    - Malicious Code
    - Malware

    - Sniffing
    - Spoofing


Syn Flood Attack
----------------
3 Way TCP Handshake

        Client -------> Server
  attacker      syn           Victim

        Client <------------Server
                  syn + atk

        Client -------------> Server
                    syn

        Client <---------------- Server
                    syn + atk


         x Finite times (Till server is flooded with log table.


Common Network setup
-----------------------------------------------
                     |
    ISP--------------|---------------Target
         Highspeed   |
                   Firewall


New IPs connecting to the server might be a good sign server is being DDoS'd

Scrubbing
-------------

Scrub incomming connections (Client or DDoS)
They clean the connection


Volumetric attack: (Floods)
------------------
Overwhelms the resources of the server
    - Pipe Saturation
    -

Amplification attack: (Memchaced Attack)
---------------------
Attackers send small chunks ---> Server sends large chunks back ----> TYPE: DNS Attack

Classic DDoS
-------------
Attacker has a larger bandwidth than Victim


Summary Story (DDoS):
------------
    - Threats:= DDOS, Amplification, Volumetric
    - Vulnurabilities:= DNS, (memchache: Server misconfig),
    - Risk:= Availability
    - Countermeasures:= IDS/IPS, Scrubbing, Analytics, % of new IPs, Volume of Traffic


IDS = Intrusion Detection System
IPS = Intrusion Prevention System


# __Threat_Vulnrability_Countermeasure__ 

## Threat

| Threat       | Consequence                    | Severity        | Ease of Exploitation   |
|--------------|--------------------------------|-----------------|---------------|
| Denial of Service | Loss of service                | Serious | Varies
| Flooding | Inability to handle valume; loss of service | Serious | Moderate
| Blocked access       | Inability to access; loss of access | Serious | Difficult
| Access failure   | Inability to access        | Serious         | Difficult

## Vulnrability

| Vulnrability           | Exploitability   | Prevalence |
|------------------------|------------------|------------|
| Insufficient resources | Easy to Moderate | Moderate   |
| Resource starvation    | Easy to Moderate | Moderate   |
| Routing failure        | Moderately difficult | Low |
| Known vulnerability    | High | Very High |
| Physical Failure       | Low for human attackers | Very high |


## Countermeasure

| Countermeasures | Issues Addressed | Mitigation Type | Mitigation Effect | Effort |
|-----------------|------------------|-----------------|-------------------|--------|
| Network administration | Insufficient resources | Prevention | Fairly high | Low |
| Intrusion detection systems | Some resource exhaustion | Detection and recovery | Fairly High | Low |
| Preparedness | Resource exhaustion physical failure | Recovery | High | Low |


