# Taxonomy Structure Documentation

## Overview

This document outlines the taxonomy structures used in the system. Taxonomies can be represented in different formats depending on the level of nesting required.

---

## Taxonomy 1: Basic List Format

**File:** `taxonomy1.yml`

**Structure:** Pure list of items without categorization

```yaml
- item: "hello-birds"
  title: "Hello Birds"
- item: "my-world"
  title: "My World"
```

**Use Case:** When items don't require hierarchical organization or categorization.

---

## Taxonomy 2: Single-Level Categorization

**File:** `taxonomy2.yml`

**Structure:** Items categorized under parent categories (2 levels deep)

```yaml
- hello-birds:
    - item: "penguin"
      title: "Penguin is a Bird"
    - item: "another-bird"
      title: "It's Title"
- my-world:
    - item: "earth"
      title: "Our Planet"
    - item: "universe"
      title: "The Cosmos"
```

**Use Case:** When items need to be grouped under broader categories.

---

## Taxonomy 3: Multi-Level Nesting

**File:** `taxonomy3.yml`

**Structure:** Three levels of nested categorization

```yaml
- hello-birds:
    - penguin:
        - item: "emperor"
          title: "Emperor Penguin"
        - item: "adelie"
          title: "Adelie Penguin"
    - another-bird:
        - item: "sparrow"
          title: "House Sparrow"
- my-world:
    - earth:
        - item: "ocean"
          title: "Pacific Ocean"
        - item: "mountain"
          title: "Everest"
```

**Use Case:** When items require deeper hierarchical organization.

---

## Taxonomy 4: Deep Nesting

**File:** `taxonomy4.yml`

**Structure:** Four or more levels of nested categorization

```yaml
- hello-birds:
    - penguin:
        - emperor:
            - item: "male"
              title: "Male Emperor"
            - item: "female"
              title: "Female Emperor"
        - adelie:
            - item: "chick"
              title: "Adelie Chick"
```

**Use Case:** When items require highly detailed hierarchical organization.
## sometimes the taxonomy 1 wouldn't be included in the taxonomy 3 or 4 because in that case only taxonomy 2 will be necessary. in case of study material subjects only course and semester were actually necessary it doesn't matter university/school
---

## Important Note 📢

**Flexibility in Structure Selection**

The nesting level can vary based on the specific taxonomy requirements:

- **When nesting is necessary:** Use appropriate nested structures (Taxonomies 2-4)
- **When nesting is NOT necessary:** Use the basic list format (Taxonomy 1)

### Example: Semesters in Courses

```
Semesters are almost uniform (1 to 8) across all courses
→ No need to categorize them based on courses
→ Use basic list format (Taxonomy 1)
```

**The loop continues for more items as needed.**
