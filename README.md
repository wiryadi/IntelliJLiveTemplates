IntelliJLiveTemplates
=====================
This is my IntelliJ IDEA 12 Live Template

Unfortunately IntelliJ does not provide simple way to export/import partial content of your live templates. So you need to manually copy this file.

To install
----------
Copy the xml file`customjava.xml` into your `~/Library/Preferences/IntelliJIdea12/templates`

To execute
----------
Just type the keyword (test, with, log) then tab

Content:
========
* __test__ - junit `test` method

```java
    @Test
    public void should() throws Exception {
        
    }
```
* __with__ - builder patttern `with` method

```java
    public SomeBuilder withPropertyName(String propertyName) {
        this.propertyName = propertyName;
        return this;
    }
```
`SomeBuilder` is automatically inferred from current class, and propertyName automatically synchronize to the method name

* __log__ - SLF4J logger declaration

```java
    private static final Logger logger = LoggerFactory.getLogger(MyClass.class);
```
`MyClass` is automatically inferred from current class.
