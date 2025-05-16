# Computer Science Notes

## 9.4.2024

### OOP (Object Oriented Programming)
- **Stands for**: Object Oriented Programming
- **Oriented**: Focus on objects
- **Java** is fundamentally OOP

#### Definition of Object
An object has two components:
1. **Data/State**: Variables or data structures (properties/attributes)
2. **Actions/Behavior**: Functions or procedures (methods in Java)

#### Advantages of OOP
- **Clarity**: Matches human understanding of real-world objects
- **Reusability**: Code can be reused across projects
- **Debugging**: Easier to isolate issues

#### Disadvantages of OOP
- **Verbosity**: Requires more code
- **Complexity**: Steeper learning curve for small projects

#### Scanner Example (OOP in Java)
```java
Scanner kb = new Scanner(System.in);
String eg = kb.nextLine();
```

#### Method Example
```java
public int getArea() {} 
// Call using: a.getArea()
```
- **Scope**: Methods can access variables declared in their class.

---

## 9.5.2024

### Objects vs. Classes
- **Class**: Template/blueprint (e.g., `Scanner`, `Rectangle`)
- **Object**: Instance of a class (e.g., `kb`, `r`)

#### Constructor
- Initializes object state.
- Prefer parameters over forcing external initialization.

---

## 9.6.2024

### `static` Keyword
- Belongs to the **class**, not individual objects.
- Shared across all instances (e.g., `IBIO`, `Math`).

### `private` Access Modifier
- Restricts access to class-only.
- Ensures encapsulation and controlled state modification.

---

## 9.9.2024

### Constructors in Depth
```java
public Rectangle() { width = 1; }
public Rectangle(int w, int h) { 
    this.width = w; 
    this.height = h; 
}
```
- **`this` Keyword**: Refers to the current object's instance variables.

### UML (Unified Modeling Language)
- Visual representation of class structure.

---

## 9.11.2024

### Reference Types
- Objects are reference types (e.g., `Rectangle a = b` shares memory).
- Primitive types (e.g., `int`) copy values.

---

## 9.18.2024

### Encapsulation
- Hides internal state and exposes controlled access via methods.
- **Getter/Accessor**: Retrieves data.
- **Setter/Mutator**: Modifies data with validation.

---

## 9.23.2024

### Advantages of Encapsulation
1. **Control**: Validate inputs via setters.
2. **Modularity**: Isolate components for easier testing.
3. **Security**: Protect sensitive data.

### Inheritance Benefits
- **Code Reuse**: Reduce duplication.
- **Flexibility**: Extend functionality easily.

---

## 9.25.2024

### Polymorphism
- **Overloading**: Same method name, different parameters.
- **Constructor vs. Setter**:
  - Constructor initializes state at creation.
  - Setter modifies state post-creation.

---

## 9.26.2024

### OOP Disadvantages
- **Complexity**: Overkill for simple tasks.
- **Performance**: Higher memory/CPU usage.

### Teamwork in Software
- **Pros**: Concurrent development, specialization.
- **Cons**: Coordination challenges, version control needs.

---

## 9.27.2024

### Modularity
- Break programs into smaller units (classes/methods).
- **Benefits**: Reusability, easier debugging, collaboration.

---

## 10.10.2024

### Platform Independence
- Java's "Write Once, Run Anywhere" via JVM.

---

## 10.24.2024

### Pre/Post Conditions
- **Precondition**: Requirements before method execution.
- **Postcondition**: Guarantees after execution.

#### Example
```java
/**
• Pre: name ≠ null

• Post: Prints greeting or error

*/
public void printGreeting(String name) {
    if (name == null || name.isEmpty()) {
        System.out.println("Error: Invalid name");
    } else {
        System.out.println("Hello, " + name);
    }
}
```

---

## 11.4.2024

### Exceptions
- **Errors**: Unrecoverable (e.g., `OutOfMemoryError`).
- **Exceptions**: Recoverable (e.g., `InputMismatchException`).

#### Handling
```java
try { ... } 
catch (Exception e) { 
    System.out.println(e.getMessage()); 
}
```

---

## 11.21.2024

### File I/O
- **`BufferedReader`**: Efficient text reading.
- **CSV**: Comma-separated values (plaintext format).

---

## 11.28.2024

### Sorting Algorithms
- **Bubble Sort**: Compares adjacent elements.
- **Selection Sort**: Finds minimum element each iteration.

---

## 12.2.2024

### GUI Basics
- **Stage**: Window container.
- **Scene**: Contains UI elements (buttons, labels).

---

## 12.11.2024

### Compiler vs. Interpreter
| **Compiler** | **Interpreter** |
|--------------|-----------------|
| Translates entire code | Translates line-by-line |
| Faster execution | Immediate feedback |
| Portability | Easier debugging |

---

## 2.19.2025

### CPU Components
1. **ALU**: Arithmetic/Logic Operations
2. **CU**: Coordinates activities
3. **Registers**: Temporary storage (e.g., MAR, MDR)

---

## 3.3.2025

### OS Security
- **Authentication**: Verify user identity.
- **Authorization**: Define access rights.
- **Encryption**: Protect data confidentiality.

---

## 3.19.2025

### Application Software Types
1. **Word Processors**: Formatting, tables, find/replace.
2. **Spreadsheets**: Data analysis (e.g., Excel).
3. **CAD**: Design/modeling (e.g., AutoCAD).

---

## 4.7.2025

### Network Security
- **Firewall**: Filters external traffic.
- **VPN**: Encrypted tunnel for remote access.
- **VLAN**: Segments network for security.

---

## 4.23.2025

### OSI Model Layers
1. Physical → 2. Data Link → 3. Network → 4. Transport → 5. Session → 6. Presentation → 7. Application

---

## 5.9.2025

### Network Threats
- **DDoS**: Overwhelm servers with traffic.
- **Malware**: Viruses, worms, trojans.
- **Countermeasures**: Firewalls, encryption, user education.

---

## Q&A Section

### Common Questions
1. **Why use `new` for exceptions?**  
   Exceptions are objects; `new` allocates memory.

2. **LAN vs. WLAN**  
   LAN uses cables; WLAN is wireless (Wi-Fi).

3. **Compiler Advantages**  
   Error checking, optimization, portability.
