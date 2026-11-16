# FORJA · 3D range viewer

> **Academic project.** FORJA is a **fictional** strength-equipment manufacturer designed for the practical project of the course **Production and Operations Management** (4th year, Business Administration, **EDEM Escuela de Empresarios**, Valencia, 2026-2027). The machines are concept prototypes created for the coursework. They are not real products and nothing here is for sale.

**Live viewer:** https://alekostormo-collab.github.io/forja-3d/

## What it is

An interactive 3D viewer of the FORJA range, opened from the QR code printed on each technical data sheet of the report:

- **Basics:** power rack, Olympic bench press, deadlift platform, adjustable bench
- **Smith machine**
- **Selectorised (pin-loaded):** lat pulldown, chest press, leg extension, seated leg curl
- **Classics:** pullover, lateral raise, leg extension (own designs inspired by the 1970s variable-cam machines)

Each machine exists in the **CLUB** and **PRO** lines (same movement, different finish and robustness). You can rotate it, switch line, change frame and upholstery colours and read its biomechanics notes and bill of materials.

Open a specific model with `?m=<code>`, for example `?m=FJ-LE1-P`.

## How it was made

The geometry is parametric (Python) and is built as solids in **FreeCAD 1.1**, which also computes the mass, steel content, coated area and upholstery of every model. This page draws the same geometry with **three.js**. Photoreal images in the report were rendered with **Blender Cycles**.

Single static page: no server, no cookies, no tracking.

## Licence

Code: MIT. FORJA name, logo and machine designs: created for this coursework; please do not reuse them as a real brand.

## Mannequins

The realistic posed mannequins are generated with [MPFB](https://static.makehumancommunity.org/mpfb.html) (MakeHuman for Blender). MakeHuman base meshes and targets are released under CC0. They are anonymous display mannequins for ergonomic checks (P5 woman 1.52 m, P50 man 1.76 m, P95 man 1.88 m).
