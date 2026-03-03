# Web APIs with .NET Core 
This repository pretends to provide learning example for creating Web APIs with .NET Core
By Rafael Xolio

## Prerequisites

Install next tools:
- Visual Studio 2022+
- Postman 


## Adding Swagger (+VS 2026)

Swagger library is not include by default in Visual Studio 2026 as previous versions, noy it is contained in the Swashbucle nuget package.

<img width="1884" height="676" alt="image" src="https://github.com/user-attachments/assets/c273390b-e53d-4aba-91e9-d93717b30976" />

## Create Api with .NET Core

<img width="713" height="341" alt="image" src="https://github.com/user-attachments/assets/82331620-2d24-4fe0-8b56-0b8af2dcd9a5" />

<img width="473" height="328" alt="image" src="https://github.com/user-attachments/assets/9b957170-95cf-4446-b9cb-99f552bf8787" />

### Adding an ActionResult
```C#
using Microsoft.AspNetCore.Http;
using Microsoft.AspNetCore.Mvc;

namespace Web.API.Learning.Controllers
{
    // https://localhost:portnumber/api/students
    [Route("api/[controller]")]
    [ApiController]
    public class StudentsController : ControllerBase
    {
        // GET: https://localhost:portnumber/api/students
        [HttpGet]
        public IActionResult GetAllStudents() {
            string[] studentNames = new string[] {"John", "Jane" };

            return Ok(studentNames);
        }
    }
}

```

### Testing

<img width="842" height="513" alt="image" src="https://github.com/user-attachments/assets/a1c5922e-2edc-4da5-8497-c29511601628" />

<img width="641" height="338" alt="image" src="https://github.com/user-attachments/assets/14e796a7-28f8-4767-98ef-052ac1ff44f2" />

## Adding Packages

<img width="382" height="514" alt="image" src="https://github.com/user-attachments/assets/5faa2648-bca5-4576-89a0-10e9cb5d850e" />


