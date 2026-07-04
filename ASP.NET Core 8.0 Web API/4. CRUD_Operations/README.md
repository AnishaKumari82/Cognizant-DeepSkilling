# Lab 4: CRUD Operations using ASP.NET Core Web API
Status: ✅ Completed

## Objective

- Perform Create, Read, Update, and Delete (CRUD) operations using ASP.NET Core Web API.
- Use the `FromBody` attribute to receive JSON data.
- Validate employee ID before updating or deleting records.
- Test the API using Swagger.

---

## Technologies Used

- ASP.NET Core Web API
- C#
- Swagger (Swashbuckle.AspNetCore)

---

## Project Structure

```
4. CRUD_Operations
│
├── Controllers
│   └── EmployeeController.cs
│
├── Models
│   ├── Employee.cs
│   ├── Department.cs
│   └── Skill.cs
│
├── Program.cs
├── appsettings.json
├── README.md
└── image.png ...
```

---

## API Endpoints

| Method | Endpoint | Description |
|---------|----------|-------------|
| GET | `/api/Employee` | Retrieve all employees |
| POST | `/api/Employee` | Add a new employee |
| PUT | `/api/Employee/{id}` | Update an existing employee |
| DELETE | `/api/Employee/{id}` | Delete an employee |

---

## How to Run

```bash
dotnet restore
dotnet build
dotnet run
```

Open Swagger:

```
http://localhost:5168/swagger
```

---

## Output

### 1. Swagger Home

![Swagger](image.png)

---

### 2. GET Employee

Displays the list of employees.

![GET](image-1.png)

---

### 3. POST Employee

Adds a new employee successfully.

![POST](image-3.png)


---

### 4. PUT Employee (Success)

Updates employee information successfully.

![PUT Success](image-3.png)
![](image-4.png)

---

### 5. PUT Employee (Invalid ID)

Returns:

```
400 Bad Request

Invalid employee id
```

![PUT Invalid](image-5.png)

---

### 6. DELETE Employee (Success)

Deletes the selected employee.

![DELETE Success](image-6.png)

---

### 7. DELETE Employee (Invalid ID)

Returns:

```
400 Bad Request

Invalid employee id
```

![DELETE Invalid](image-7.png)

---

## Learning Outcomes

- Implemented CRUD operations using ASP.NET Core Web API.
- Used `FromBody` to bind JSON request data.
- Validated employee IDs before update and delete operations.
- Returned appropriate HTTP status codes.
- Tested REST APIs using Swagger.

---

## Conclusion

Successfully implemented CRUD operations on Employee data using ASP.NET Core Web API. The application supports creating, retrieving, updating, and deleting employee records with proper validation and was tested successfully using Swagger.