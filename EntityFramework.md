# Learnings
## Installation
  * Should install the **EntityFrameworkCore.SqlServer** package to use the SqlServer in Configure Services in Startup.cs file.
    ```csharp
     services.AddDbContext<CoWorksCommunityContext>(options =>
     {
         options.UseSqlServer(Configuration.GetConnectionString("Default"));
     });
    ```
  * Database key Should be pluarals 
    ```json 
    "ConnectionStrings":{ 
    "Default": "Data Source=(LocalDb)\\.\\devdb;Initial Catalog=CoWorksCommunity;Integrated Security=True"
    }
    ```
