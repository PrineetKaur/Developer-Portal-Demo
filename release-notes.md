# Release Notes – v2.3.0 (September 2025)

## 🚀 New Features
- Payments API: Added support for recurring transactions (`/v1/payments/recurring`)
- Data Export Tool: New CLI option `--format parquet` for large-scale analytics

## 🐛 Bug Fixes
- Fixed issue with API authentication tokens expiring prematurely
- Corrected SQL export schema mismatch in the Analytics API

## ⚠️ Deprecations
- `/v1/payments/initiate` endpoint is deprecated; use `/v1/payments/create` instead
