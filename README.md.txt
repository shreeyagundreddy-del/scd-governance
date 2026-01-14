# SCD Governance – Customer Dimension

## Purpose
Implements SCD Type 2 for customer master data with governance controls.

## Components
- dim_customer table
- SCD2 upsert procedure
- Approval workflow
- Rollback capability
- Audit history

## Deployment
1. Merge PR to main
2. Run SQL in pgAdmin / migration tool
3. Verify current record and approval

## Governance Rules
- Only current records can be approved
- History is immutable
- Rollbacks create new versions
