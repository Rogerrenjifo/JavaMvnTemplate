# 🧪 Cucumber Java Maven Template

This repository is a starter template for setting up automated tests using Cucumber, JUnit 5, and Allure Reports with Maven.
Use it to quickly start writing and running your test cases — without configuring everything from scratch.
run the test cases with 


## 🚀 Run the Tests

To execute the tests and generate Allure reports, use the following commands:

```bash
# Run all test cases
mvn test

# Run tests and automatically open the Allure report in the browser
mvn clean verify allure:serve

# Run tests and generate the Allure report (without opening it)
mvn clean verify allure:report
```

## 🧩 Tech Stack

🥒 Cucumber: 7.11.1

☕ Java: 8+

⚙️ Maven: build and dependency management

🧾 JUnit 5: test framework

📊 Allure Reports: beautiful interactive test reports

## 📁 Project Structure
```bash
src
 └── test
     ├── java/com/screenplay        # Step definitions and test runners
     └── resources/features         # Cucumber .feature files
```



## References 

## 🧠 References

[📘 Allure Report + JUnit 5 Documentation](https://allurereport.org/docs/junit5/)

[🥒 Cucumber JVM Documentation](https://cucumber.io/docs/guides/10-minute-tutorial/)

[⚙️ JUnit 5 User Guide](https://docs.junit.org/current/user-guide/)

[🧩 Allure Maven Plugin Docs](https://docs.qameta.io/allure/#_maven)

[☕ Maven Surefire Plugin](https://maven.apache.org/surefire/maven-surefire-plugin/)

## 📝 Notes

- The test runner (RunCucumberTest.java) is configured to automatically generate Allure results after each test execution.

- The file allure.properties defines the path where Allure results are stored (e.g. target/allure-results/).
- you can set different outputs in: 
```
@ConfigurationParameter(key = PLUGIN_PROPERTY_NAME, value = "io.qameta.allure.cucumber7jvm.AllureCucumber7Jvm")
```