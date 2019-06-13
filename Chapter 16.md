## __Threat: Data Corruption__

Data corruption can occure by the following factors:

-   Typing Error
-   Software Flaw
-   Malicious Code
-   Hardware Failure
-   Transmisison problem
-   Noise Accident
-   Hacker Activity
-   Human Mistake
-   Program Error

### __Sequencing attack__

This attack invloves permuting the order of data. This occurs in network communications, a sequencing error occurs when a later fragment of a data steam arrives before a previous.

### __Substitution attack__

This attack is the replacement of once piece of a data stream with another nonmalicious substition can occur if a hardware or software malfunciton causes two data streams to become tangled, such that a piece of one stream is exchanged with the other steam.

Substitution errors can occur with adjacent cables or multiplexed parallel communications in a network.

### __Insertion Attack__

This attack, which is almost a form of substitution is one in which data values are inserted into a stream. An attacker does not even need to break an cryption scheme in order to insert authentic-seeming data as long as the attacker knows precisely where to slip in the data.


## __Countemeasures: Codes__

To protect data, a technique can be used to detect change in the data.

### __Error Detection Codes__

Checksums, hash codes and message digests all work the same way: In that they are function that can detect some changes, regardless of whether the change was accidental or not. These functions produce a result whose calue depends on each individual bot of the input data.

### __Error Correction Codes__

Error Correction Codes not only detect change but also provide help to correct it. These codes could correct single-bit errors and detect two-bit errors. This was refered to as the Hamming Code.

Reed Solomon Codes where applied to blocks of data, like bytes. These codes are especially suited for correcting bursts of erros, several bits in a row, among the more common computer communications errors. These codes are used to correct data errors on CDs/

## __Countermeasure: Protocols__

Procedures and protocols operate internally so the user sees only the data. THe most common used of protocols is in networked communciations.

## __Countermeasure: Procedures__

Procedures come at a level above the communications stream to which protocols apply. Once correct data has been received and stored for future reference, we want to be sure they remeain intact. Error detection and correction codes are used in storage systems to ensure that what is written is what is returned later when reread.

### __Backup__

Back ups are an effective control against data loss. They are also a way to recover from integrity failures. 

### __Redundancy__

Redundancy is a countermeasure to DoS attacks. If a process or data at one location is attacked, having a second copy elsewhere reduces the risk of diened acces. With the low prices of hardware and especially storage, having several redundatn copies becomes a reasonable option.

## __Countermeasure: Cryptography__

### __Block chaining__

Cryptography is useful in part because it is consistent. The orginiator ecrypts something and the retriever who decrupts it will always receive the same result with the proper key. But that consistency can become a disadvantage if the attacker tries to perform a substitution attack.

# __Threat_Vulnrability_Countermeasure__ 

## Threat

| Threat       | Consequence                    | Severity        | Ease of Exploitation   |
|--------------|--------------------------------|-----------------|---------------|
| Sequencing   | Data Corruption                | Mild to Serious | Easy
| Substitution | Data Corruption, falsificaiton | Mild to Serious | Moderate
| Salami       | Data Corruption                | Mild to Serious | Moderate
| Similarity   | Inappropriate Inference        | Serious         | Moderate

## Vulnrability

| Vulnrability                       | Exploitability    | Prevalence |
|------------------------------------|-------------------|------------|
| Integrity failure: data corruption | Easy to difficult | Morderate  |
| Inappropriate disclosure           | Moderate          | Infrequent |


## Countermeasure

| Countermeasures | Issues Addressed | Mitigation Type | Mitigation Effect | Effort |
|-----------------|------------------|-----------------|-------------------|--------|
| Error Correction and Detection Codes | Substitution modification | Detection, correction, | Strong | Low |
| TCP Protocol | Sequencing substitution corruption | Correction | Storng | Very Low |
| Procedures   | Corruption, modification, loss | Correction | Strong | Low|
| Cryptography | Sequencing, substitution | Detection | Strong | Low |

