# Campus Course & Records Manager (CCRM)

## 📌 Project Overview
A Java SE console application for managing students, courses, enrollments, grades, transcripts, and backups.

## 🚀 How to Run
1. Install JDK 17+
2. Compile:
   ```bash
   javac -d out $(find src -name "*.java")
   ```
3. Run:
   ```bash
   java -cp out edu.ccrm.cli.MainMenu
   ```

## 📖 Evolution of Java
- 1995: Java 1.0 released
- 2004: Java 5 (Generics, Annotations)
- 2014: Java 8 (Lambdas, Streams, Date/Time API)
- 2017: Java 9+ (Modules, var)
- 2021: Java 17 LTS
- 2023: Java 21 LTS

## 📊 Java Editions
| Feature | Java ME | Java SE | Java EE |
|---------|---------|---------|---------|
| Target  | Mobile/Embedded | Desktop/Standard | Enterprise/Server |
| Scope   | Lightweight APIs | Core language + libraries | Servlets, EJB, Web apps |

## ⚙️ Java Architecture
- **JDK** – Developer toolkit (compiler, debugger)
- **JRE** – Runtime environment
- **JVM** – Executes bytecode

## 🖥️ Setup
- Install JDK (screenshot in `screenshots/`)
- Install Eclipse → New Java Project → Import packages → Run `MainMenu`

  ## Java ME vs Java SE vs Java EE (Jakarta EE)

| Feature | Java ME | Java SE | Java EE (Jakarta EE) |
|---|---|---|---|
| Target | Embedded/mobile & constrained devices | Desktop/server general-purpose | Enterprise apps (web, transactions, messaging) |
| APIs | Subset, device profiles | Core language + standard libraries | Adds enterprise APIs (Servlets/JAX-RS/JPA/JMS) |
| Packaging | MIDlets | JARs | WAR/EAR |
| Footprint | Small | Medium | Larger |
| Typical Use | Feature phones/IoT | CLI apps, libraries | Enterprise backends |

**Platform note (SE vs ME vs EE):** CCRM is a **Java SE** console app. It does not rely on app servers or enterprise containers.

---

## JDK, JRE, JVM: What/How
- **JVM**: The virtual machine that executes bytecode.
- **JRE**: JVM + standard libraries to *run* Java apps (deprecated as a separate download in modern JDKs).
- **JDK**: JRE + compiler/tools to *develop* Java apps.
- Relationship: Source → `javac` → bytecode (class files) → executed by JVM.


## 📑 Mapping Table
| Topic | Implementation |
|-------|----------------|
| Encapsulation | `Student` private fields + getters/setters |
| Inheritance | `Person` → `Student`, `Instructor` |
| Abstraction | `Person` (abstract class) |
| Polymorphism | `printProfile()` overrides |
| Singleton | `AppConfig` |
| Builder | `Course.Builder` |
| Enum | `Semester`, `Grade` |
| Exception Handling | custom exceptions in `service.exceptions` |
| File I/O (NIO.2) | `ImportExportService`, `BackupService` |
| Streams | `StudentService.searchByName()` |
| Recursion | `BackupService.computeDirectorySize()` |
| Lambda | Comparator/Predicates in services |

## 📸 Screenshots
- JDK version check
- Eclipse setup
- Program menu
- Exported CSV
- Backup folder


---

## Acknowledgements
- Java standard docs for API references.

> **Note on Integrity:** This repository is provided solely as a learning aid/starter. Please customize heavily and add your own work, screenshots, and demonstrations per your evaluator’s policy.


