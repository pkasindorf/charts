# mailer services 

Buildinglink Mailer Services Reimagined

## queue generator

The queue generator mailer service is part of the digest creation process. It polls the database
at a defined interval looking for digests that are ready to be sent and generates a 
queue message for each result.
