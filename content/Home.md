---
dg-publish: true
dg-home: true
---
This vault has been a work in progress since 11-09-2024.

This will serve as a vault to store everything related to my study of math from my second year of undergrad through whenever I stop maintaining this.

#### Course Work
```dataview
table Name, Professor, Term
from "Courses"
SORT choice(Term = "Fall 2023", "1", choice(Term = "Spring 2024", "2", choice(Term = "Fall 2024", "3", choice(Term = "Spring 2025", "4", choice(Term = "Fall 2025", "5", choice(Term = "Spring 2026", "6", "other"))))))
```

#### Material
```dataview
table Textbook, Author, Context, Depth, Sections, When
from "Textbooks"
SORT choice(When = "Fall 2023", "1", choice(When = "Spring 2024", "2", choice(When = "Fall 2024", "3", choice(When = "Spring 2025", "4", choice(When = "Fall 2025", "5", choice(When = "Spring 2026", "6", "other"))))))
```