# Generator Sizing Calculator: Industrial & Commercial Power

**Live demo:** https://zov911.github.io/generator-sizing-calculator/

An interactive generator sizing tool for standby, prime and continuous power. Build a load list, account for motor starting and site conditions, and get a recommended standard genset size with industry-specific guidance on codes, fuel, emissions and common pitfalls.

## Features

- **Load builder** with preset equipment for each industry plus custom loads (kW or motor hp)
- **Motor starting analysis:** starting kVA for across-the-line, wye-delta, soft-starter or VFD starting, with a side-by-side comparison showing how much smaller the genset can be with a VFD
- **Site derating** for altitude and ambient temperature
- **Load-factor gauge** with wet-stacking warning (diesel engines below ~30% load)
- **Fuel burn estimates** for diesel and natural gas, in metric or US units
- **12 industries:** Agricultural, Commercial, Construction & Events, Data Center (incl. AI racks), Forestry, Greenhouses / CEA, Healthcare, Industrial, Mining, Municipal & Emergency, Oil & Gas, Water / Wastewater
- **Up-to-date guidance:** EPA Tier 4 Final vs emergency-standby rules, NFPA 110 Level 1 / Type 10, NFPA 99, CSA C282, NEC 700/701/702/517, HVO renewable diesel, battery-hybrid gensets, and 1 MW+ lead times driven by data-center demand
- **Buyer view / Sales view:** works as a public lead-gen tool ("questions to ask your supplier") or as an internal sales-enablement tool ("sales strategy")
- **Quick estimate mode:** slide through standard sizes from 10 kW to 3 MW
- Copy summary, shareable links (full state in the URL), print/PDF, and a mobile layout

## Sizing method (simplified)

```
Required kW = max( running kW × (1 + growth) ÷ load target,
                   [other running kVA + largest motor starting kVA ÷ 2.5] × 0.8 )
              ÷ site derate factor
→ rounded up to the next standard genset size
```

Load targets: standby 80%, prime 70%, continuous 90%. This is a rule-of-thumb estimate. Final selection must use manufacturer sizing software and a licensed engineer's review.

## Tech

A single self-contained `index.html`: vanilla HTML, CSS and JavaScript with no build step and no dependencies (Google Fonts only).

---

## Want this calculator for your business?

I build custom, on-brand sizing tools and configurators for power-generation dealers, rental fleets and OEMs. They capture qualified leads and help sales teams quote faster.

**Reach out → [zov911.com](https://zov911.com)**

© zov911. All rights reserved.
