# Test Samples

This project is a test helper class which will package all the samples for orders
so that across all projects we can share the test Samples

## TestOrderBuilder

Builder class which can be used to build the sameples. It has methods to duplicate orders
based on the samples.

##MapBuilder

Builder class to create hash of hashes.Useful to construct HashMaps with builder
pattern.

## Samples

## Using it in your project

Include the following dependency in order to utilise this project

```
<dependency>
  <groupId>com.att.oce.bpm.common</groupId>
  <artifactId>oce-test-orders</artifactId>
  <version>1.0-SNAPSHOT</version>
  <scope>test</scope>
</dependency>
```

Example code snippet to build order samples

Gets Hash of hashes from the order json
```
TestOrderBuilder.build("WirelessAccessoryOrder").getMapofMaps();
```

Gets string from the order json
```
TestOrderBuilder.build("WirelessAccessoryOrder").toString();
```

Gets string from the order json after duplicating it.[yet to be developed]
```
TestOrderBuilder.build("WirelessAccessoryOrder").duplicate().toString();
```

Build a HashMap
```
MapBuilder.build().add("test", "testvalue").get()
```


## TODO

1. duplicate function
