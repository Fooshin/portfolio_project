# PASTA Threat Modeling 
!!!note
    The breakdown below is an initial look at threat modeling working on a ficitious company. The course walked through each of the components in the PASTA threat model. My notes and assessement are my own.

|Stages|Sneaker Company|
|----------|--------------|
| I.Define business and security objectives| Will the app accept all kinds of payments? What third party apps will be used? Will there be collecting of data for marketing that will need to be protected? Will the company hold login credentials that give access to C.C information? What are the regulations about handling the data based on where they are in the world? How will customers and employees see each others data during customer service help sessions|
| II.Define the technical scope | I would prioritize SQL injection threats based on the vulnerabilites of this company. Additionally, systems should be checked for correct configuration across this model analysis.|
| III.Decompose Application | [Sample data flow diagram](https://docs.google.com/presentation/d/1ol7y79popTFfNHM-90ES-H-i1Lpd0YNvPShxBlXozjg/template/preview?resourcekey=0-DZAkf7Vzh2PXsP-j3oXV-g)|
| IV.Threat analysis | Based on the information given, the largest looming threat are SQL injections through user requests for searches to the database. Threat actors may also acquire hash functions that have not been properly salted. An assessement and audit for authorization should be standardized to ensure employees can only access and view sensitive data from the database for isolated customer service situations.|
| V.Vulnerability Analysis | Poorly written code or code review practices can allow for injections into the website to gain knowledge of the database. If the server has also not been properly hardened or configured, other network protocols could be used to attack customers and launch malware attacks.|
| VI.Attacking Modeling | [Sample attack tree diagram](https://docs.google.com/presentation/d/1FmWLyHgmq9XQoVuMxOym2PHO8IuedCkan4moYnI-EJ0/template/preview?usp=sharing&resourcekey=0-zYPY7AhPJdcClXamlAfOag)|
| VII.Risk Analysis and Impact | Prepared Statements, Principle of Least Privilege ,Input Sanitation, Input Validation |