# RuTracker4j

A Java library that provides convenient access to RuTracker.org with support for searching torrents, retrieving topic details, and downloading torrent files.

## Features

- Search for torrents by keyword
- Retrieve detailed topic information
- Download torrent files
- Simple and intuitive API

## Documentation

For more information and examples, see the [GitHub Wiki](https://github.com/silenzzz/RuTracker4j/wiki).

## Installation

### Maven

Add the dependency to the `<dependencies>` section in your `pom.xml`:

```xml
<dependency>
    <groupId>ru.syntezis</groupId>
    <artifactId>RuTracker4j</artifactId>
    <version>0.0.1</version>
</dependency>
```

The library is available on Maven Central Repository, so no additional repository configuration is required.

### Gradle

```groovy
implementation 'ru.syntezis:RuTracker4j:0.0.1'
```

## Usage

### Initialize the client

```java
import dev.silenzzz.rutracker4j.RuTracker4jDefaultClient;
import dev.silenzzz.rutracker4j.scrapper.net.AccountCredentials;

RuTracker4j ruTracker = new RuTracker4jDefaultClient(
    new AccountCredentials("username", "password")
);
```

### Get topic by ID

```java
Topic topic = ruTracker.findTopicById(633781);
System.out.println(topic.getTitle());
```

## License

This project is licensed under the [Apache License 2.0](LICENSE).

---

<div style="text-align: center;">
  <a href="https://syntezis.ru">
    <img src="https://syntezis.ru/img/logo.svg" alt="Syntezis" height="40"/>
  </a>
  <br/>
  <sub>Built and maintained by <a href="https://syntezis.ru">Syntezis</a></sub>
</div>