# Variable Dictionary — Carers' Leave Policy Dataset (Work Sample)

**Note:** This dataset is a PhD application work sample and **not a complete dataset**.

| Variable Name                  | Variable Type | Variable Definition                                                                 | Predefined Labels                                                                 |
|--------------------------------|---------------|-------------------------------------------------------------------------------------|----------------------------------------------------------------------------------|
| country_iso3                   | string        | ISO-3 code (e.g., JPN, FRA)                                                         |                                                                                  |
| year                           | integer       | Calendar year the rule is in force                                                  |                                                                                  |
| date_enactment                 | integer       | Official adoption date of the act/decree that creates or amends the leave provision |                                                                                  |
| date_entry_into_force          | integer       | Effective date when the provision became usable/legally binding                     |                                                                                  |
| leave_name_english             | string        | Standard English name of the leave                                                  |                                                                                  |
| leave_name_original            | string        | Official name of the leave in the original language                                 |                                                                                  |
| entitlement_basis              | categorical   | Legal/institutional basis establishing the right                                    | statutory, collective_agreement, employer_policy                                  |
| legal_citation_english         | string        | English title of the governing law/regulation                                       |                                                                                  |
| legal_citation_original        | string        | Title of the governing law/regulation in the original language                      |                                                                                  |
| source_url                     | string        | Primary source URL to the official legal text or consolidated version               |                                                                                  |
| min_employer_tenure_mo         | numeric       | Minimum continuous tenure (months) with the current employer required at the time   |                                                                                  |
| min_contract_term_mo           | numeric       | Minimum contract term (months) to qualify                                           |                                                                                  |
| min_weekly_hours               | numeric       | Minimum contracted weekly hours (hours/week) required to qualify                    |                                                                                  |
| eligible_contracts             | categorical   | Contract types covered by the entitlement                                           | all, permanent_only, incl_temp_fixed, incl_parttime, self_employed_incl/excl     |
| eligible_sectors               | categorical   | Sectors covered by entitlement                                                      | all, public_only, private_only, listed_exclusions                                |
| eligibility_work_note          | string        | Free-text clarification of work-related eligibility                                 |                                                                                  |
| work_eligibility_exclusions    | string        | Work-related exclusions from eligibility                                            |                                                                                  |
| eligible_kin_relations         | string        | Kin relationships covered by the entitlement                                        |                                                                                  |
| co_residence_requirement_level | ordinal       | Whether co-residence with the care recipient is legally required (0/0.5/1)          |                                                                                  |
| care_dependency_requirement    | string        | Free-text description of any dependency/severity requirement                        |                                                                                  |
| eligibility_note               | string        | Free-text clarification of care-recipient–related eligibility conditions            |                                                                                  |
| notice_required_days           | numeric       | Minimum number of calendar days of advance notice required before leave start       |                                                                                  |
| application_note               | string        | Free-text details of the application procedure                                      |                                                                                  |
| job_protection_level           | ordinal       | Whether the job/position is legally protected during leave (0/0.5/1)                |                                                                                  |
| job_protection_note            | string        | Free-text details of return rights (same vs equivalent job), scope, and exceptions  |                                                                                  |
| anti_retaliation_level         | ordinal       | Whether an explicit anti-retaliation / non-discrimination clause exists (0/0.5/1)   |                                                                                  |
| max_duration_days              | numeric       | Total number of job-protected leave days (convert weeks→FTE workdays)               |                                                                                  |
| entitlement_periodicity        | categorical   | Unit by which entitlement is allocated                                              | per_episode, per_relative_lifetime, per_relative_year, per_carer_lifetime, per_carer_year |
| periodicity_note               | string        | Free-text explanation of cycles, carryover, pooled vs per-person caps               |                                                                                  |
| partial_leave_allowed_level    | ordinal       | Whether partial-day/part-week use is permitted (0/0.5/1)                            |                                                                                  |
| split_blocks_allowed_level     | ordinal       | Whether leave can be taken in multiple blocks (0/0.5/1)                             |                                                                                  |
| flexibility_note               | string        | Free-text details on increments, block constraints, simultaneous use, etc.          |                                                                                  |
| paid_leave_level               | ordinal       | Whether any statutory cash benefit is provided (0/0.5/1)                            |                                                                                  |
| flat_rate_daily_local          | numeric       | Flat-rate daily benefit amount in local currency (NA if not applicable)             |                                                                                  |
| income_replacement_rate        | numeric       | Earnings-related replacement rate as decimal (NA if only flat-rate/unpaid)          |                                                                                  |
| max_benefit_days               | numeric       | Total number of days for which a monetary benefit is payable                        |                                                                                  |
| funding_source                 | categorical   | Source of financing for the cash benefit                                            | social_insurance, tax, employer, mixed                                           |
| administering_agency           | categorical   | Entity administering the entitlement/benefit                                        | social insurance fund, ministry, employment service, employer, mixed             |
| benefit_taxability_level       | ordinal       | Whether the benefit is taxable (0/0.5/1)                                            |                                                                                  |
| social_security_note           | string        | Free-text note on social-security treatment during leave                            |                                                                                  |
| notes_misc                     | string        | Additional information not captured elsewhere                                       |                                                                                  |

---

### Legend
- `*_level` = ordinal (0/0.5/1):  
  - 0 = none  
  - 0.5 = partial/conditional or applies to some workers  
  - 1 = generally applies  
  - NA = not specified  

- `*_local` = local-currency amount


