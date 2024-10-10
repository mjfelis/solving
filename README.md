# Idea box

## Browser authentication

## Browser logs

## Pay per verification

### Idea #1

This is a privacy preserving solution.

1. Browser sends a random `sessionId` (UUID) to the DTS when sending the browser profile.
2. When a DTS would like to request presentation of a credential of a specific schema, it first executes a transaction in the PTR. Transaction MUST include `CredentialSchemaPerm.id` and UUID.
3. When presentation request is received, to verify if verifier is allowed to do so, query to Trust Registry includes the sessionId.

Example, if sessionId = ee606c76-76e9-41ae-9e5a-21ae64a76c9b

`GET /did:web:trust-registry/trqp-2.0/entities/did:web:service-credential-verifier/authorization?authorizationVID=did:web:trust-registry/cs/js/f4524751-8617-40de-bbe6-b2e0fef63c7a#VERIFIER-ar-ee606c76-76e9-41ae-9e5a-21ae64a76c9b`


## Unic ID card

Use a NFC card to store recovery keys.
Issue a physical nfc ID card
Use your ID card as a recovery key for your wallet

## Unic ID for callcenters

Give a PIN to the user to identify transaction

### Qualification

- End user MUST be able to qualify DTSs.
- End user MUST be able to report DTSs.
- Service MUST provide a bank note to all users so that they can qualify without having to pay.
- Each time a user qualifies a service, its trust deposit grows.
- As end user has a trust deposit too, 

### Bank notes

- for preserving privacy of end users
- bank notes are convertible to balance and/or trust deposit

