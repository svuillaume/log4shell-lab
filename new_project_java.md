Here’s your content organized neatly in a single Markdown file without changing anything:

# Maven Quickstart Guide

## Common Maven Commands
- `mvn archetype:generate` → creates project  
- `mvn clean install` → compiles project  
- `mvn exec:java -Dexec.mainClass=...` → runs main class  

---

## Step 1: Create Project Folder with Maven

```bash
mkdir -p ~/projects
cd ~/projects

# Create a new Maven project called foo
mvn archetype:generate \
  -DgroupId=com.example \
  -DartifactId=foo \
  -DarchetypeArtifactId=maven-archetype-quickstart \
  -DarchetypeVersion=1.4 \
  -DinteractiveMode=false


⸻

Step 2: Navigate to Your Project

cd foo

Now your folder structure looks like:

foo/
 ├── pom.xml
 └── src/
      ├── main/java/com/example/App.java
      └── test/java/com/example/AppTest.java


⸻

Step 3: Build the Project

mvn clean install

Note: Maven will compile App.java and run any tests.

⸻

Step 4: Run the Main Class

mvn exec:java -Dexec.mainClass="com.example.App"

You should see output like:

Hello World!


⸻

Step 5 (Optional): Add Your Own Class
	1.	Go to src/main/java/com/example/
	2.	Create a new file, e.g., FooServer.java:

package com.example;

public class FooServer {
    public static void main(String[] args) {
        System.out.println("Foo server running!");
    }
}

Build and run:

mvn clean install
mvn exec:java -Dexec.mainClass="com.example.FooServer"

Output:

Foo server running!

I can also make a **slimmed-down one-page version** with just commands and structure for quick reference if you want. Do you want me to do that?
