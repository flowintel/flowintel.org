---
title: FlowIntel 3.0.0 released and MISP integration 
banner: /images/news/flowintelxMISP.png 
author:
 - MISP Project team
date: 2026-02-18
---


## FlowIntel and MISP: Working Together

The integration between [FlowIntel](https://github.com/flowintel/flowintel) and [MISP](https://www.misp-project.org/) is designed to make investigation and intelligence sharing part of the same workflow — not two separate steps handled in different tools.

Instead of finishing an investigation and then rebuilding everything manually in MISP, FlowIntel keeps data structured from the beginning and allows it to move back and forth when needed.

{{<video src="/images/news/flowintel_blog.mp4"  >}}


---

### Creating MISP-Objects Inside a Case

FlowIntel allows the creation of MISP-Objects directly within a case.

When an IP address, domain, file hash, URL, or other indicator is identified, it can be added as a structured object following MISP definitions rather than written as free text.

By the time a case is ready to be shared, the data is already structured correctly. There is no need to rebuild objects or reformat information later.

---

### Sending a Case to MISP

After configuring a MISP connector (URL and API key), a case can be sent to MISP.

A case can either:

- Create a new MISP event  
- Enrich an existing event  

During export:

- The case and its tasks are represented as MISP-Objects  
- All MISP-Objects created in FlowIntel are added to the event  
- Investigation notes are converted into MISP event reports  

This ensures that both indicators and analytical context are shared. The narrative of the investigation becomes part of the event rather than being separated into an external report.

---

### Creating a Case from a MISP Event

The integration also works in the opposite direction.

A MISP event can be used to generate a new FlowIntel case. Objects present in the event are imported as structured objects within the case.

A template is used during case creation to ensure that internal workflows and documentation standards remain consistent. Externally sourced intelligence can therefore be investigated within an organized and standardized framework.

This is particularly useful when:

- Investigating community-shared campaigns  
- Processing intelligence received from partners  
- Performing deeper internal analysis on shared events  

---

### Updating a Case from a Linked MISP Event

If a case is linked to a MISP event, object-related updates in the event can be reflected in the case.

When new objects or attributes are added in MISP, the corresponding case can stay aligned. This helps avoid discrepancies between internal investigations and shared intelligence.

---

### Enrichment Through Integrated MISP Modules

MISP modules are integrated directly into FlowIntel.

During an investigation, enrichment can be performed on attributes. The results can automatically:

- Create new structured objects  
- Add or complete investigation notes  

Enrichment becomes part of the case timeline, preserving traceability and context without requiring manual copying of results between platforms.

---

### Attribute Search and Case Correlation

FlowIntel includes attribute search capabilities across cases.

If the same domain, IP address, or hash appears in multiple investigations, the relationship can be identified. Correlation between cases helps detect recurring infrastructure or patterns internally, complementing MISP’s broader community-wide correlation.

---

### Galaxies, Taxonomies, and Custom Extensions

Galaxies and taxonomies are part of the ecosystem, ensuring classification consistency between FlowIntel and MISP.

Starting with version 3.0.0, custom galaxies and taxonomies can also be integrated. This allows organizations to extend classifications with internal or sector-specific vocabularies while maintaining structured alignment.

---

### A Continuous Workflow

With this integration:

- Investigations begin in a structured format  
- Intelligence can be shared without rebuilding data  
- Context and analysis remain attached to indicators  
- Updates can flow in both directions  

## What’s Next?

FlowIntel and MISP already work closely together, but there’s more coming.

One focus area is improving audit logs and roles. More detailed logging and clearer role separation will make collaboration easier and give better visibility on who did what inside a case — especially useful in larger teams.

Another direction is adding more computer-assisted capabilities. The plan is to make better use of MISP modules to enrich cases more intelligently — automatically creating useful objects or completing notes when possible, while keeping everything traceable.

We plan to integrate FlowIntel more directly inside MISP. The goal is to make the connection between investigation and sharing even smoother, reducing friction between the two platforms.

---

## Try It

FlowIntel is open source and available on GitHub:

https://github.com/flowintel/flowintel

Connecting it to a MISP instance is the best way to see how investigations and intelligence sharing can flow together in a practical, hands-on way.

