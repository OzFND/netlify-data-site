# Public Data Files

This repository hosts public CSV datasets intended for programmatic access by web applications and AI tools.

All files under `/data` are publicly accessible via Netlify and CORS-enabled for read-only access.

---

## Base URL
https://muslimans.netlify.app/data/


---

## Datasets

### mosques-usa.csv

A national dataset of mosques in the United States.

**File path**
/data/mosques-usa.csv

**Example URL**
https://muslimans.netlify.app/data/mosques-usa.csv


**Schema**

| Column        | Description |
|--------------|------------|
| `record_id`  | Stable unique identifier (never reused) |
| `name`       | Mosque name |
| `city`       | City |
| `state`      | Two-letter US state code |
| `denomination` | Islamic denomination (e.g. sunni) |

**Notes**
- `record_id` values are permanent and must never be reused
- Text values are case-preserved for readability
- Enumerated fields (e.g. denomination) are lowercase
- This file will grow over time as new mosques are added

---

### businesses-ny.csv

A dataset of Muslim-owned businesses in New York State.

**Schema**

| Column        | Description |
|--------------|------------|
| `record_id`  | Stable unique identifier (never reused) |
| `name`       | Business name |
| `city`       | City |
| `state`      | Two-letter state code |
| `category`   | One or more categories, pipe-delimited |

**Category format**
- Multiple categories are separated using `|`
- Example: `butcher|grocery`

---

## Access & Usage

- All CSV files are read-only
- No authentication required
- Suitable for:
  - Frontend apps
  - Search indexes
  - AI ingestion
  - Data analysis

---

## Update Policy

- New records are appended with new `record_id` values
- Existing records may be corrected but IDs remain unchanged
- Deleted records are not reused

---

## License

Data is provided as-is for public informational use.
