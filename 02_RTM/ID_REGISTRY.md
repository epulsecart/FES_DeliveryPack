# سجل معرفات المتطلبات (مقدمة عربية)
هذا القسم العربي يوضح أن المعرفات فريدة وغير قابلة لإعادة الاستخدام.
يجب إصدار أي ID جديد هنا قبل إضافته إلى RTM.
باقي الملف بالإنجليزية لأغراض هندسية دقيقة.

# Requirement ID Registry

Purpose: Prevent duplicate or conflicting IDs across requirements, APIs, pages, rules, and tests.

## ID Types
- FR-#### Functional Requirement
- NFR-#### Non-Functional Requirement
- UC-#### Use Case
- ALG-#### Business Rule / Algorithm
- API-#### API Requirement
- P-#### Page/UI Requirement

## Issuance Rules
1) Reserve IDs here before adding to RTM.
2) Never reuse an ID once assigned.
3) IDs increase sequentially within each type.
4) If a requirement is removed, keep the ID and mark as BLOCKED in RTM.

## Registry Table (append new rows)
Format: `ID | Title | Date | Owner | Status`

Example:
- FR-0001 | Create Production Order | 2026-01-27 | Analyst | ACTIVE
- NFR-0001 | Response Time | 2026-01-27 | Analyst | ACTIVE

## Duplicate Prevention
- Check RTM.csv before assigning a new ID.
- Keep a single source of issuance here.
