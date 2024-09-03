# Workshop - Mentoria 4

# IDE
* Intellij

# Dependências
* [Selênio Java » 4.24.0](https://mvnrepository.com/artifact/org.seleniumhq.selenium/selenium-java/4.24.0)
* [API JUnit Júpiter » 5.11.0](https://mvnrepository.com/artifact/org.junit.jupiter/junit-jupiter-api/5.11.0)
* [Cucumber JVM: Java » 7.18.1](https://mvnrepository.com/artifact/io.cucumber/cucumber-java/7.18.1)
* [Cucumber JVM: JUnit 4 » 7.18.1](https://mvnrepository.com/artifact/io.cucumber/cucumber-junit/7.18.1)

# Plugin
* [Cucumber for Java](https://plugins.jetbrains.com/plugin/7212-cucumber-for-java)
* [Gherking](https://plugins.jetbrains.com/plugin/9164-gherkin)

# Criar estrutura de pastas

* test
    * java
        * botão direito
            * new > package
                * runner: execução
                    * Botão direito > new > class: runnerTest
                * core: controlar selenium e navegador
                    *  Botão direito > new > class: Driver
                * pages: pageObjects - controle de paginas
                    * Botão direito > new > class: pagesTest
                * steps: espaço para o Cucumber
                    * Botão direito > new > class: stepsTest
                * maps: mapeamentos
                    * Botão direito > new > class: mapsTest

* test
    * botão direito
        * new >
            * Directory: resources
                * feactures
                    * Botão direito > new > file: login.feature
                        * Configurar login.feacture com o plugin Gherkin
                            * login.feacture > Botão direito > Override File Type > Gherkin


* 1º runnerTest
* 2º Driver
* 3º Feature
* 4º LoginSteps


# Erros

**Erro:** java.lang.NullPointerException: Cannot invoke "org.openqa.selenium.WebDriver.get(String)" because the return value of "core.Driver.getDriver()" is null

**Correção:** O erro ocorre por falta da dependência JUnit Jupiter. Importe a dependência  [API JUnit Júpiter » 5.11.0](https://mvnrepository.com/artifact/org.junit.jupiter/junit-jupiter-api/5.11.0) e atualize o Maven.