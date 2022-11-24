# nology-music-player
A simple console based music player used to demonstrate the configuration of a project using Spring Core.

## Overview

The project covers:
- Setting up a project without Spring
- Using XML to configure the Spring project
- Using Annotations to configure the Spring project

### Setup

Clone the project.

```bash
git clone https://github.com/nology-tech/nology-music-player
```

Open the project in Intellij.

Right-click on the project, select Maven and then Reload project.

To change branch.

```bash
git checkout name-of-branch
```

### Branches

- `01-java`
- `02-java-completed`
- `03-xml-spring`
- `04-xml-spring-completed`
- `05-annotations-spring`
- `06-annotations-spring-completed`
- `07-spring-boot-api`

### Class Diagram

This is a simplified class diagram showing the key classes and their dependencies and relationships with other classes and interfaces.

![](./notes/class-diagram.png)

### Spring Core Annotation Reference

| Annotation                    | Description                                                                                                                                                                                                          |
|-------------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| @Configuration                | Where you are going to configure your Spring beans / components. *Reference only not used in this project*                                                                                                           |
| @Bean                         | Creates a new bean in the container. *Reference only not used in this project*                                                                                                                                       |
| @Component                    | A general Spring bean / component.                                                                                                                                                                                   |
| @Component("name")            | The above with the a name. Useful if you need a named reference.                                                                                                                                                     |
| @Repository                   | A specialised annotation for persistence bean.                                                                                                                                                                       | 
| @Controller                   | A specialised annotation for controller bean.                                                                                                                                                                        |
| @Service                      | A specialised annotation for service bean.                                                                                                                                                                           |                                                                                                                                             |
| @ComponentScan                | Indicates packages to scan to look for Annotations.                                                                                                                                                                  |
| @Autowired                    | Used to Inject Dependencies into a class in different ways, instance variable, constructor and methods. If you have one implementation and the field name matches the class name it can do the wiring automatically. |
| @Autowired @Qualifier("name") | Used with @Autowired to distinguish between multiple implementations. Essentially giving the Spring Bean an Id you can reference later on.                                                                           |
| @PostConstruct                | Used above a method that will be called after initialization of the class.                                                                                                                                           |
| @PropertySource(value = "")   | Loads the app.properties files. It takes a value which is the class-path to the file. Used with `@Configuration`.                                                                                                    |
| @Value("${propertyName}")     | Used for loading a property from app.properties. It takes a String with the name of the property in between "${}"                                                                                                    |




