# Rails API Diagnostic

Place your responses inside the fenced code-blocks where indicated by comments.


What is the purpose of a backend?

```bash
Back end handles the server, data storage and running the application that front end touches on the surface.
```

Which layer in the MVC pattern is used by the controller to fetch data?

```bash
Model
```

Which layer in the MVC pattern communicates with the model?

```bash
Controller
```

Why don't we use views in our interpretation of the MVC pattern?

```bash
We are doing single-page-app, we do not need to rely on views that is necessary where sites have multiple pages.
```

What does C.R.U.D stand for?

```bash
C.R.U.D. stands for Create, Read, Update and Delete.
```

In which part of the MVC pattern can we find C.R.U.D actions?

```bash
C.R.U.D. actions are performed in the controller layer.
```

A user action fires a `GET` request for `person/1`. Explain in detail each step
required for data to be returned to the client. (bullet points or ordered list)

```bash
1. Client browser makes GET request to a curl --request GET --data ='' http://localhost:3000/person/1 of a Rails app
2. Web server receives the request, then matches with appropriate controller action
3. Web server uses dispatcher to create new controller
4. Controller parses the user requests, either deny the request or proceed to translate it into a command that the Rails model layer can understand
5. Model retrieves data from which the controller translates that to HTTP
6. Controller returns the translated data to the server into viewable HTTP response format to the user
```

What is the command to generate a new rails-api app?

```bash
rails new
```

What is the command to start an instance of a rails server?

```bash
rails server
```

What are the commands to drop, create and migrate a database? (3 bullet points)

```bash
1. db:drop
2. db:create
3. db:migrate
```

What is the command to scaffold a pet with a name and an age?

```bash
rails generate scaffold Pet name:string age:integer
```

List two advantages of using serializers? (2 bullet points)

```bash
- makes API safer and easier to use
- combine different models, through their serializers, into a same JSON response
- keep your code DRY and organized
```
