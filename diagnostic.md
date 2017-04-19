# Rails API Diagnostic

Place your responses inside the fenced code-blocks where indicated by comments.

What is the purpose of a backend?

```md
To store data and to serve up data.
```

Which layer in the MVC pattern is used by the controller to fetch data?

```md
Model layer
```

Which layer in the MVC pattern communicates with the model?

```md
Controller layer
```

Why don't we use views in our interpretation of the MVC pattern?

```md
'Cause we want our client to render the view instead of server
```

What does C.R.U.D stand for?

```md
Create, Read, Update, Destroy
```

In which part of the MVC pattern can we find C.R.U.D actions?

```md
Controller
```

List at least 5 standard rails actions that C.R.U.D requests correspond to?

```md
Create => Create, READ => Show/Index, Update => Update, DESTROY => Destroy
```

A user action fires a `GET` request for `/people/1`. Explain in detail each step
required for data to be returned to the client. (bullet points or ordered list)

```md
1. The user fires a URL GET request
2. The router maps the GET request to a Controller show method
3. The controller show method acts upon the person model
4. The person model creates SQL to select the person record
5. The person model returns the person record to the Controller
6. The controller sends the data to the client
```

What is the command to generate a new rails-api app?

```bash
rails generate new
```

What is the command to start an instance of a rails server?

```bash
rails server
```

What are the commands to drop, create, migrate and seed a database from the command
line? (5 bullet points)

```bash
rails db:drop db:create db:migrate db:seed
```

What is the command to scaffold a pet with a name and age attributes (hint:
Also think of the data types for each attribute)?

```bash
rails generate model Pet name:string age:integer
```
