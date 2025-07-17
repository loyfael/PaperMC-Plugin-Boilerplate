# SkySyncro

SkySyncro is a reusable template for creating Minecraft plugins, designed specifically for **version 1.21.7** on Paper. This template provides a clean, ready-to-use structure to help you start your own plugin projects quickly and efficiently.

## About This Template
- **Reusable:** Easily adapt this template for any new Paper plugin project.
- **Modern:** Uses the latest PaperMC API (1.21.7-R0.1-SNAPSHOT) and Java 21.
- **Minimal & Clean:** Only the essentials are included—perfect for building your own features on top.
- **Strict Compatibility:** This template is intended **only** for Minecraft 1.21.7. No support is provided for earlier versions, and backward compatibility is not planned.

## Features
- Pre-configured `pom.xml` with PaperMC repository and dependency.
- Minimal `plugin.yml` ready for customization.
- Main class (`Main.java`) already set up with `onEnable` and `onDisable` methods.
- Clear project structure following best practices for Paper plugins.

## Getting Started
1. **Clone or copy this template** to your own project directory.
2. **Customize the package name, plugin name, and metadata** in `plugin.yml` and `Main.java` as needed.
3. **Develop your features**: Add commands, event listeners, and logic in the `src/main/java` directory.
4. **Build the plugin**:
   - Use Maven: `mvn clean package` (or use the Maven panel in IntelliJ IDEA)
   - The compiled JAR will be in the `target/` directory.
5. **Deploy**:
   - Place the generated JAR in the `plugins` folder of your Paper 1.21.7 server.
   - Start or restart your server.

## Project Structure
```
SkySyncro/
├── pom.xml              # Maven configuration (PaperMC API, Java 21)
├── README.md            # This documentation
├── src/
│   └── main/
│       ├── java/
│       │   └── loyfael/
│       │       └── Main.java   # Main plugin class
│       └── resources/
│           └── plugin.yml      # Plugin metadata
└── target/              # Compiled JAR and build output
```

## Requirements
- **Minecraft:** Paper 1.21.7
- **Java:** 21 or higher
- **Build Tool:** Maven (or use IntelliJ IDEA's built-in Maven)

## Customization Tips
- Change the `main` class path in `plugin.yml` to match your package structure.
- Update the `name`, `version`, `author`, and `description` fields in `plugin.yml`.
- Add new classes for commands, listeners, and features in the `java/` directory.

## Why Only 1.21.7?
This template is intentionally focused on the latest PaperMC API for Minecraft 1.21.7. Supporting only this version ensures you benefit from the newest features, best performance, and up-to-date security. There is **no plan to support older versions**.

## Why Maven and Not Gradle?
I deliberately chose **Maven** over Gradle for this template. Maven offers a simpler, more rigid, and predictable build process, which is ideal for reusable templates and for developers who want clarity and stability in their project setup. Gradle is not supported or recommended for this template.

## License
You are free to use, modify, and share this template for your own plugin projects.

## Author
loyfael
