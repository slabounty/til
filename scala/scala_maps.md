# Scala Maps

To create a Scala map

```scala
// for an empty map
val emptyMap = Map()

// With values
val fullMap = Map("a" -> "a", "b" -> "b")
```

To get values

```scala
// scala> fullMap.get("a")
// res3: Option[String] = Some(a)

// or
// scala> fullMap.getOrElse("c", "missingValue")
// res2: String = missingValue
```


