# Spring MongoDB OData $filter
OData Version 4.0 $filter parser for Spring Data MongoDB

###### Maven
```xml
<dependency>
    <groupId>com.efindi</groupId>
    <artifactId>smo-filter</artifactId>
    <version>0.0.1-RELEASE</version>
</dependency>
```

###### Gradle
```groovy
compile ('com.efindi:smo-filter:0.0.1-RELEASE')
```

### Usage
This will throw an InvalidODataFormatException if the string input is not valid.
```java
Filter mf = new Filter("LastName eq 'Smith' and Age gt 16 and LastUpdatedDate ge datetime'2017-12-28T21:48:28Z'");
Criteria criteria = mf.getCriteria();
```


javax.validation
```java
public class RequestObject {
    @ODataFilter
    private String $filter;
}
```

## Alpha
This project is still in early alpha stage. We welcome any collaborator who is interested in working for this project. 