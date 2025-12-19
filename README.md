### `README.md`

```markdown
# 🚑 narcan.delivery Data

> **The core dataset powering [narcan.delivery](https://narcan.delivery).** > *A Quantara Project.*

## 📖 About

This repository hosts the primary data source for **narcan.delivery**, a web service dedicated to simplifying access to life-saving naloxone across the United States. 

The dataset (`data.json`) provides a standardized, state-by-state breakdown of:
* **Legal Frameworks:** Standing orders, Good Samaritan laws, and third-party prescribing authority.
* **Access Channels:** Pharmacy availability, mail-order programs (e.g., NEXT Distro), and community distribution points.
* **Practical Guidance:** "How-to" guides for quick access, overcoming barriers, and cost information.
* **Verified Sources:** Citations for all legal and medical claims.

This data is **routinely updated** to reflect changing laws, new distribution programs, and updated pharmacy protocols.

## ⚡ Data Structure

The data is formatted as a JSON array of state objects. Each state object adheres to the following schema:

```json
{
  "state": "State Name",
  "abbreviation": "XX",
  "last_updated": "YYYY-MM-DD",
  "legal_framework": {
    "naloxone_legal_status": "...",
    "standing_order_or_protocol": { ... },
    "good_samaritan_overdose_immunity": { ... }
  },
  "access_channels": {
    "pharmacies": { ... },
    "community_programs": [ ... ],
    "mail_based_programs": [ ... ]
  },
  "practical_guidance": { ... },
  "sources": [ ... ]
}

```

## 🔬 Research & Analysis

You are free to fork this repository and use this data for research, public health analysis, or policy review. We ask that you credit **narcan.delivery / Quantara** in any resulting work.

## 🤝 Contributing

We welcome community contributions! If you notice that a state's laws have changed, or a mail-order program has updated its eligibility:

1. **Fork** the repository.
2. **Edit** the `data.json` file.
3. **Submit a Pull Request** with a description of the change and a link to the new source/law.

All PRs are reviewed by the Quantara team to ensure accuracy before merging.

## ⚠️ Disclaimer

**This data is for informational purposes only.** While we strive for accuracy, laws and programs change rapidly. This dataset does not constitute legal or medical advice. In a medical emergency, always call 911 immediately.

* **Medical:** Consult a healthcare professional for medical advice.
* **Legal:** Consult a qualified attorney for legal counsel regarding state statutes.

---

<div align="center">

**[narcan.delivery](https://narcan.delivery)** is a project by **Quantara**.

*Innovation for Harm Reduction.*

</div>

```

```
