# Diagrama de clases

# Diagrama de secuencia

```mermaid
sequenceDiagram
    participant User as User
    participant Controller as StudentController
    participant Model as StudentModel
    participant View as StudentView

    User->>Controller: User interacts (addStudent, getStudent)
    Controller->>Model: addStudent(studentData)
    Model->>Model: Save student data
    Controller->>Model: getStudent(studentId)
    Model-->>Controller: Return student data
    Controller-->>View: Pass student data
    View->>User: Display student data
```