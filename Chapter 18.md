## __Threat: Data leakage__

Of particular interest to companies and governments is the concept of data leakage. Data leakage is another term for inappropriate or unauthorized disclosure, occuring without the knowledge or censent of the person holding the data.

## __Threat: Introduction of Malicious Code__

Facebook and other social media sites are excellent places for distribution of malicious code. THese sites represent what appearsto be a trusted environment with little basis for that trust. Friends might never do anything intention to harm theyr friends, but that does not address possible unconscious, unknowing, or ill-advised acts. Precisely because of the interconnectedness of users at networking sites there will be plenty of sharing of photos, documents, videos, programs, apps and other objects capable of containing and transmitting malicious code.

## __Attack Details: Unintended Disclosure__

The disclosure threat in social networking involves several different concepts that come together. First, there is the issue of knowing what is sensitive and what you do not want to release. Second, there is the invisible wall of trust: Face-to-face you can get a sense of someone's reliability and decide at the moment how much to trust that person, but with online interaction you establish a trust relationship which is really an access control decisio, to use the computer security concept

### __Sensitive Data__

Some databases contain what is called sensitive data. As a working definition, let us say that sensitive data are data that should not be made public. Determining which data items and fields are sensitive depends both on the individual database and the udnerlying meaning of the data.

Factors that make data sensitive:

-   Inherently Sensitive
-   From a sensitive source
-   Deckared sensitive
-   Part of a sensitive attribute
-   Sensitive  in relation to previously disclosed information


### __Types of Disclosures__

-   Exact Data
-   Bounds: Sensitve value is between 2 values
-   Negative Result: One value is not the value of another
-   Existence
-   Probable Value

### __Direct Inference__

Inference is a way to infer or derive sensitive data from nonsensitive data. THe inference problem is a subtle vulnerablility in database security.

#### __Direct Attack__
A user tries to determine values of sensitive fields by seeking them directly with queries that yield few record.

### __Inference by Arithmetic__

Another procedure used by the U.S Census Bureau and other ogranizations that gather sensitive data, is to release only statistics.

#### __Sum__
 An attack by sum tries to infer a value from a reported sum.

#### __Count__
The count can be combined with the sum to produce some even more revealing results. Often these two statistics are released for a database to allow users to determine average value.

#### __Mean__
Average allows exact disclosure if the attacker can manipulate the subject population. As a trivial example, consider salary. Giver the number of employees the mean salary for a company and the mean salary of all employees except the president. it is easy to compute the president's salary.

#### __Median__

The mid point of an ordered list of values. The attack requires finding selections having one point of intersection that happens to be exactly in the middle.

#### __Tracker Attacks__

As already explained database management systems may conceal data when a small number of entries make up a large proportion of the data revealed. A tracker attack can fool the database manager into location the desired data by using additional queries that produce small results.

#### __Linear System Vulnerability__
A tracker is a specific case of a more general vulnerability. With a little logic algebra and luck in the distributiuon of the database contenst. It May be possible to cunstruct an algebraic linear system of equations that reutrns results relating to several different sets.

Many sites have privacy policies have these characterisitcs:
-   Length
-   Language
-   Mutability
-   Nontransferability
-   Noncomparability


# __Threat_Vulnrability_Countermeasure__ 

## Threat

| Threat         | Consequence                         | Severity        | Ease of Exploitation   |
|----------------|-------------------------------------|-----------------|---------------|
| Disclosure     | Loss of confidentiality and privacy | Serious | Easy
| Malicious code | System compromise                   | Serious | Easy


## Vulnrability

| Vulnrability                       | Exploitability    | Prevalence |
|------------------------------------|-------------------|------------|
| Analysis of data | High | Morderate  | High



## Countermeasure

| Countermeasures | Issues Addressed | Mitigation Type | Mitigation Effect | Effort |
|-----------------|------------------|-----------------|-------------------|--------|
| Encryption | Privacy | Technical | Prevention | Moderate, but severly contrains usefulness |
| User educaiton, awarenewss | Confidentiality malicious code | Administrative | Prevention | Low, but low effectiveness |
| System design | Privacy | Technical | Prevention | Moderate |




