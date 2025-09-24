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

## ▶️ Optional
Demo video link here.
