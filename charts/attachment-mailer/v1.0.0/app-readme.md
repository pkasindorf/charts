# Cloud Mail

## priority-mailer

The priority mailer sends mail messages on demand by default. It implements
a rules based priority system.

## digest-mailer

The digest mailer service is use to compose a digests of notification
messages from the buildinglink website. It then sends that digest to subscribers
at a predefined time each day.

## attachment-mailer

The attachment mailer service is a priority mailer (like the the one above). It
is dedicated to processing priority emails with attachments.

## digest-q-gen

The digest-q-gen service is used to queue notifications that will be sent by 
the digest mailer at the designated time.
