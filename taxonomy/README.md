## Qxel Taxonomy

The Qxel Taxonomy System defines how products are organized and displayed across our Discovery Pages.

While the main search system lives on our backend, the taxonomy provides a simple, guessable way for anyone to browse and explore products — no complicated tracking links required.

---

🔗 Simple, Guessable URLs

Every taxonomy path maps directly to a clean, human-readable URL.

For example:

```
https://www.qxel.in/products/books
```

And you can go deeper:

```
https://www.qxel.in/study-materials/calicut-university
```

This shows all products from Calicut University. You can keep narrowing down:

University → Course → Subject → Semester

We limit paths to 8 taxonomy levels to prevent server and database abuse. If you believe a product deserves more depth, you can request a higher limit.

---

🗂️ Repository Structure

1. Categories (/taxonomy/categories)

The Categories directory lists all product categories available on Qxel (excluding streaming).

Each category represents a large database of its own, so we only add new categories when they truly deserve to stand alone.

· Format: JSON
· Contains: Taxonomy values under each category, e.g. Templates > Canva > Resume
· Optional: You can include an example field

---

2. Items (/taxonomy/items)

The Items directory holds complete records for every product category.

Each taxonomy level is stored as a separate directory inside items/<category>/.

· Format: YAML (.yml)
· Fields:
  · title
  · item

---

3. Info (/taxonomy/info)

Every taxonomy item deserves its own description and details.

The Info directory works like a GitHub Topics page — each item gets a short, clear description.

· Format: Markdown (.md)

---

🧩 Simple by Design

We use only three simple formats:

· Markdown — for descriptions
· YAML — for item records
· JSON — for category structure

You don't need any coding knowledge. Just copy an existing value, replace it with yours, and you're done.

---

📁 Directory Overview

```
taxonomy/
├── categories/     # JSON — all product categories & their taxonomy values
├── items/          # YAML — full records per category, level by level
└── info/           # Markdown — descriptions for each taxonomy item
```

---

🤝 Contributing

Want to add a category, topic, or description? See our Contribution Guide:

https://www.qxel.app/docs/contribution-guide

Every contribution helps improve the marketplace for creators across India.
