Database Schema Overview

This table outlines the entities, primary keys (PK), foreign keys (FK), and corresponding attributes for the database schema.

Entity (Table)

Primary Key (PK)

Foreign Key (FK)

Attributes

region

id

-

name

sales_reps

id

region_id (FK to region)

name

accounts

id

sales_rep_id (FK to sales_reps)

name, website, lat, long, primary_poc

orders

id

account_id (FK to accounts)

standard_qty, poster_qty, glossy_qty, total, occurred_at, standard_amt_usd, gloss_amt_usd, poster_amt_usd, total_amt_usd

web_events

id

account_id (FK to accounts)

occurred_at