# Read: Class 18

## Reflections

This reading assignment talks about many to many relationships in databases, as well as an unintentionally opaque article about the opaqueness of security.

## Readings

[Many to many relationships](https://www.baeldung.com/hibernate-many-to-many)

1. Name a few examples of real world ManyToMany relationships.

    Students and Courses, Employees and Projects, Doctors and Patients

2. Explain the significance of a join table for ManyToMany relationships.

    The significance of a join table in a ManyToMany relationship is that it allows for the relationship to be represented in a separate table, rather than directly in the tables of the related entities.

3. What are the values held within a join table?

    A join table typically contains two foreign keys that reference the primary keys of the related entities, as well as any additional attributes that describe the relationship between them, such as the date when the relationship started or ended, or the role of each entity in the relationship

[Security: a humorous overview](https://scholar.harvard.edu/files/mickens/files/thisworldofours.pdf)

1. According to the author of the article, will you ever be truly secure from ALL possible security threats?

    According to the author, security is a process, not a product, and it is impossible to be truly secure from all possible security threats. The author argues that the best we can do is to try to manage risks and mitigate threats as best as we can, while acknowledging that we will always be vulnerable to some degree.

## Things I want to know more about

1. I'm being charitable in the review above, because the author really wants you to know how funny he is every other sentence and it ruins the pacing and message of the paper, Which is why he's a computer scientist and not Douglas Adams or Terry Pratchett.
