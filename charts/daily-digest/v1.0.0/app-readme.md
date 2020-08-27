# Buildinglink Daily Digest

This chart install and configures an instance of the buildinglink 
daily digest emails ervce.

## Prerequisites Details

* These services require access to the underlying infrastructure for Rabbit MQ and Sql Server

## Chart Details

This chart will do the following:

* Implement digestqueue - a digest creation/distribution service
* Implement digestmailer - a scalable mailer service
  