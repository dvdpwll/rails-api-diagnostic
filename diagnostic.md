# Rails API Diagnostic

Place your responses inside the fenced code-blocks where indicated by comments.


What is the purpose of a backend?

```bash
To hold information that can be retrived.
```

Which layer in the MVC pattern is used by the controller to fetch data?

```bash
Model
```

In which part of the MVC pattern can we find C.R.U.D actions?

```bash
Controller
```

List at least 5 standard actions that C.R.U.D corresponds to?

```bash
Post, Index, Show, Patch, Delete
```

A user action fires a `PATCH` request for `pets/1`. Explain in detail each step
required for data to be returned to the client. (bullet points or ordered list,
please include information on dynamic segments, the params hash and seralizers).

```bash
User sends request to router
Router sends request to controller
Controller sends requeset to the model
Model checks the request and retrives information from the database
Model sends the info to the controller
Controller sends the info to the user
```

What is the command to scaffold a `medicalRecords` join table which holds
refrences to a `pets` and a `vets` table?

```bash
rails g scaffold medicalRecords pets:references vets:references
```

What is the point of having a join table?

```bash
To make a Many-to-Many relationship between two tables.
```

Give an example of a one-to-many relationship and a many-to-many relationship:

```bash
One-To-Many: A mother can have many children, but a child can not have multiple biological mothers.
Many-To-Many: A student can have many teachers, and a teacher can have many students.
```
