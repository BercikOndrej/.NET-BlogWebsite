# Blog Web (ASP .NET Core)
It is a **Blog web** using `C#` on backend developmnet and **ASP .NET Core** framework for web requests handling. On this web page user can register, login/logout, edit his profile, change the password, view all articles or write own article or comment. Of course user can delete his own comments or articles.

Application uses `MVC architecture` in IDE names `Rider`

## Project structure
- **wwwroot**
    - Here are static files like css, js, Bootstrap
- **appsettings.json**
    - Setting file
- **Program.cs**
    - This is a start file for running an application
- **Areas**
    - Here we are defining a database context for manipulating with database via `EntityFramework`
- **Controllers**
    - Objects for user interaction
    - These objects are manipulating with **models**
    - Contains an application endpoints 
    - Also it produces **views** components
    - **ArticleController**
        - Here is the article logic defined like view all articles, delete article, save article etc
    - **HomeArticle**
        - And here is a home page logic defined
- **Migrations**
    - Folder contains database migrations
- **Models**
    - Here are specified classes names models, which the project display on the website
    - It is data objects implementing application data logic, mostly getting and saving data into database
    - It can be change
    - They can be identified with EntityFramework entities
    - **BlogArticle**
        - Represents an article
    - **Comment**
        - Represents a comment for the article
    - **ErrorViewModel**
        - Represents error view for the user
- **Views**
    - Components for display UI of application
    - It uses data from **Models** 
    - Using `Razor` templates system for rendering websites (mix `html` and `C#` -> `.cshtml`)

## Used technology
- `ASP .NET Core framework` for handling web requests
- `C#` and standart libraries for backend development (it is possible use C# for Fronend because of `Razor` templates system)
- `Entity Framework` for object-relation mapping
- `SQLite database` for saving data
