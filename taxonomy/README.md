
---

## Here are valid YAML files for each taxonomy:

### **Taxonomy 1** (`taxonomy1.yml`) — Pure list of items:
```yaml
- item: "hello-birds"
  title: "Hello Birds"
- item: "my-world"
  title: "My World"
```

---

### **Taxonomy 2** (`taxonomy2.yml`) — Categorized under Taxonomy 1:
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

---

### **Taxonomy 3** (`taxonomy3.yml`) — Nested under both (3 levels deep):
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

---

### **Taxonomy 4** (`taxonomy4.yml`) — Even deeper nesting:
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

---
**The loop just repeats for more and more items**  
# **Note📢: If the Nesting isn't necessary for some Taxonomies then we will use basic list for them too.**
**Example: Semesters for courses are almost same(1 to 8) so we dont have to categorize them based on course**
