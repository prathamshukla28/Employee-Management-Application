# Employee Management Application

A console employee management system in Java. It keeps employees in memory and lets you
add, view, update, delete and list them from a numbered menu.

## Features

1. **Add** an employee (id, name, age, designation, department, salary)
2. **View** one employee by id
3. **Update** an employee's name and salary
4. **Delete** an employee by id
5. **List** all employees
6. **Exit**

It starts with four sample employees (ids 101 to 104) so you can try every option straight away.

## Run it

Needs JDK 8 or newer.

```bash
javac -d out *.java
java -cp out com.sj.empmanagmentapplication.Main
```

## How it works

| File | Role |
| --- | --- |
| `Main.java` | Menu loop and input handling |
| `EmployeeService.java` | CRUD operations over a `HashSet<Employee>` |
| `Employee.java` | Employee model with getters, setters and `toString` |

Data lives in memory only, so it resets every time the program starts.
