# Measurement implementation checklist

## Design
- [ ] Name the business event and source of truth.
- [ ] Define event timing and what counts as a valid event.
- [ ] Choose a stable event identifier for deduplication where supported.
- [ ] List each field and justify why it is needed; remove unnecessary identifiers.
- [ ] Document consent/legal review, privacy notice, retention, access, and deletion handling.

## Implementation
- [ ] Use current official documentation for the storefront and each destination.
- [ ] Keep credentials and access tokens server-side; never commit secrets to this repository.
- [ ] Separate test and production environments.
- [ ] Ensure retries do not create duplicate business events.

## Validation
- [ ] Send synthetic test events and confirm expected destination receipt.
- [ ] Check event names, timestamps, currency, value, identifiers, and deduplication behavior.
- [ ] Reconcile event counts and values against the source system for a defined period.
- [ ] Record known gaps and obtain owner sign-off before using the data for optimization.