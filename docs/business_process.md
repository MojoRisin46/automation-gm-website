### Phase 1 – Process audit (no data access)

You only analyze **workflows**, not systems.

You ask questions like:

* What repetitive tasks exist?
* What tools are used?
* Where do employees copy data between systems?
* What triggers manual work?

Deliverable:
**Automation Opportunity Map**

No sensitive data required.

This already builds trust.

---

### Phase 2 – Synthetic or anonymized data

Instead of real data you request:

* screenshots
* exported schema
* fake datasets
* sanitized logs

Example:

Instead of customer database:

```
customer_id
order_date
order_value
status
```

No names, addresses, etc.

You only need **structure**, not identity.

---

### Phase 3 – controlled technical access

Only if necessary.

Options:

* screen sharing sessions
* temporary accounts
* read-only database access
* access to staging environments

Never request production access immediately.

---