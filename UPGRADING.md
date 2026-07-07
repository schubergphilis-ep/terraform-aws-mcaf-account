# Upgrading Notes

This document captures required refactoring on your part when upgrading to a module version that contains breaking changes.

## Upgrading to v1.0.0

### Key Changes v1.0.0

The Terraform provider source for `mcaf` has moved:

- Old source: `schubergphilis/mcaf`
- New source: `schubergphilis-ep/mcaf`

### How to upgrade v1.0.0

1. Update your root module provider configuration to use the new source address.
2. Reinitialize providers: `terraform init -upgrade`
3. Run `terraform plan` and confirm no unexpected recreation caused by provider address drift.
