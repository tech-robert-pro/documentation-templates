# Documentation Templates

> Reusable templates, style guides, and SOPs for hardware user manuals — built for consistency at scale.

![Status](https://img.shields.io/badge/status-maintained-brightgreen)
![Docs](https://img.shields.io/badge/docs-technical%20writing-blue)

---

## Overview

Nine years of producing hardware documentation taught me that consistency doesn't happen by accident — it happens when you build the system first and write into it. This repository holds the template framework, style conventions, and process documentation behind that system.

These aren't theoretical examples. They're the working files that supported a sustained output of **100+ documentation deliverables per year** across monitor, projector, and large-format display product lines.

**At a glance:**

| Attribute | Detail |
| :--- | :--- |
| **Role** | Sole author and maintainer |
| **Duration** | 9 years of continuous production |
| **Scope** | Multiple template families, SOP guides, illustration standards |
| **Stack** | Adobe InDesign, Illustrator, Photoshop; GIMP, Inkscape; Markdown |
| **Output Formats** | Print PDF, web wiki, downloadable documentation packages |
| **Status** | Actively maintained |

---

## What's Inside

```
/
├── README.md                     # This file
├── adobe-templates/              # InDesign, Illustrator, Photoshop source files
│   └── README.md                 # Version requirements and font dependencies
├── markdown-samples/             # Web-ready documentation fragments
│   ├── advanced-features.md
│   ├── initial-setup.md
│   ├── using-the-monitor.md
│   └── README.md
├── illustration-examples/        # Technical drawing samples
│   ├── io-port-diagram.svg
│   ├── stand-assembly-diagram.svg
│   └── README.md
├── sops/                         # Process documentation
│   ├── template-adoption-guide.md
│   ├── style-consistency-checklist.md
│   └── release-workflow.md
├── samples/                      # Sanitized reference samples
│   └── sample-page-spread.pdf
└── assets/                       # Supporting images and styles
    └── images/                   # Technical illustrations (generic products)
```

Each directory has its own README covering dependencies, version requirements, and known quirks.

---

## Background

Before this system existed, documentation was produced ad hoc. Every manual was a fresh start — new layouts, drifting terminology, inconsistent warning formatting, and no shared figure conventions. The problems compounded:

- **Style drift** across product lines meant customers got a different experience depending on which device they bought.
- **Production time** ballooned because writers rebuilt layouts from scratch each cycle.
- **Ramp-up cost** for anyone joining the documentation effort was high, since conventions lived in people's heads rather than in files.
- **Review cycles** caught formatting inconsistencies instead of substance, wasting reviewer attention.

The constraint shaping the solution was straightforward: **one writer, 100+ deliverables a year, no dedicated design or engineering support.** Whatever I built had to be maintainable by one person and adoptable by others without hand-holding.

This system served a hardware documentation portfolio spanning:
- Professional-grade monitors (including 5K resolution displays)
- Commercial projectors
- Large-format displays for signage and collaborative environments

---

## Approach

Three decisions drove the design.

**1. Templates as enforced structure, not suggestion.**
Master pages and paragraph styles in InDesign do the heavy lifting. Writers apply named styles rather than formatting manually, which makes consistency the default path instead of the disciplined one.

**2. Dual-track output (print + web).**
The same content pipeline produces both print-ready PDFs and web-ready Markdown. Adobe tools handle complex layouts and technical illustrations; Markdown enables wiki integration and searchability. Maintaining parallel tracks means the system survived platform shifts without losing fidelity.

**3. Process written down, not assumed.**
The SOP guides exist because knowledge that lives only with one person is a liability. Writing the adoption guide forced me to articulate decisions I'd been making intuitively, and it surfaced inconsistencies I hadn't noticed.

---

## Outcome

- Supported **100+ documentation deliverables per year** over **9 years** without proportional growth in production time.
- Adopted by **multiple team members** for ongoing documentation work.
- Standardized terminology, warning formatting, and figure conventions across **three hardware product categories**.
- Established a review baseline that let reviewers focus on technical accuracy rather than formatting disputes.

---

## Illustration Standards

Technical illustrations follow a strict visual convention:

| Element | Specification |
| :--- | :--- |
| **Line weight** | Consistent stroke weight across all diagrams |
| **Numbering** | Callout circles with numbers |
| **Labels** | Minimal text, positioned adjacent to callouts |
| **Color usage** | Grayscale base; accent colors (red arrows/highlights) for emphasis only |
| **Views** | Exploded views for assembly; orthographic projections for connectivity |

Example illustrations are included in `illustration-examples/`. These depict **generic monitor hardware** and have been sanitized to remove all brand identifiers and proprietary product information.

---

## Usage

### Working with Markdown samples

1. Review `markdown-samples/README.md` for structure conventions.
2. Each `.md` file represents a complete documentation chapter.
3. Images reference files in `assets/images/` — ensure they're present in the same relative path.
4. Tables use standard Markdown syntax with HTML extensions for complex layouts.

### Adopting the SOPs

Read `sops/template-adoption-guide.md` first. It walks through the conventions in the order you'll encounter them and explains the reasoning behind each rule, which matters when you hit a case the template doesn't cover.

---

## Notes & Limitations

**Sanitized examples only.** All content in this repository has been stripped of brand identifiers, model numbers, and proprietary specifications. The structural and typographic decisions are intact; the subject matter is generic hardware documentation.

**Font dependencies.** Templates reference commercial fonts. Substitutions will shift line breaks and page counts. Substitute deliberately and re-check pagination.

**Not a CMS.** This is a file-based template system, not structured content management. 

**What I'd do differently.** Given another pass, I'd build the open-source track first and treat Adobe as the derivative. Maintaining two parallel sets taught me that the more portable format should be canonical, since it constrains you to decisions that survive tooling changes.

---

## Related Projects

- [Portfolio and case study](https://tech-robert-pro.github.io)
- [Hardware manual samples](https://github.com/tech-robert-pro/hardware-manual-samples)
- [Documentation wiki project](https://github.com/tech-robert-pro/wiki-project)
- [Terminology management](https://github.com/tech-robert-pro/terminology-management)
- [LLM automation tools](https://github.com/tech-robert-pro/llm-tool-examples)

---

## License

© 2026 Robert. All rights reserved.

Shared for portfolio and reference purposes. Template architecture and process documentation are my original work. Any content depicting third-party products has been sanitized to remove proprietary information. Not licensed for redistribution or commercial use.

---

<!--
MAINTENANCE
Last reviewed: October 2026
Review cadence: Annually, or when templates change materially
Contact: tech.robert@protonmail.com
-->
