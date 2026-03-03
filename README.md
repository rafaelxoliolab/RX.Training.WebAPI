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

## Create Controller with .NET Core Sample

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


## Create a new API
### Adding Packages

<img width="382" height="514" alt="image" src="https://github.com/user-attachments/assets/5faa2648-bca5-4576-89a0-10e9cb5d850e" />

### Adding DbContext

<img width="947" height="380" alt="image" src="https://github.com/user-attachments/assets/ab4bac9f-4141-425d-948f-3910a356dcd3" />

### Adding ConnectionString

<img width="930" height="382" alt="image" src="https://github.com/user-attachments/assets/a9025c1c-f3eb-4402-895a-e2ca6c1558c9" />

### Adding DI for DbContext
<img width="883" height="386" alt="image" src="https://github.com/user-attachments/assets/7a2c3ebf-f23a-4472-b82c-bd4adce22723" />

### Run Migrations

<img width="439" height="314" alt="image" src="https://github.com/user-attachments/assets/87351d17-b6b9-4e5b-b818-79da2e6a51b5" />

<img width="403" height="242" alt="image" src="https://github.com/user-attachments/assets/580a1c7b-839d-48d1-882e-4eed5d3395c2" />

<img width="896" height="382" alt="image" src="https://github.com/user-attachments/assets/b09c5e7f-1339-47ed-8942-249bd081a564" />

<img width="195" height="68" alt="image" src="https://github.com/user-attachments/assets/a517f09c-7ac7-46d1-b473-d559f7809827" />

<img width="262" height="215" alt="image" src="https://github.com/user-attachments/assets/48caacca-e649-4a03-a3ea-a9701f5c1cb3" />







