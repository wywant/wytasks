# 从返回值角度来看
## 返回 Stream的方法

  * map mapToDouble mapToInt mapToLong 
  * filter
  * peek
  * distinct
  * limit
  * skip
  * sorted  
  
##  返回 boolean的方法

  * allMatch
  * anyMatch
  * noneMatch
  
## 返回 Optional<T> 及 T的方法
  
  * findAny 
  * findFirst
  * max
  * min
  * reduce  
  
## 返回 R的方法

  * collect
  * reduce
 
## 返回 void的方法

  * forEach
  * forEachOrdered
  
## 前提返回值的方法

  * toArray
  
# 从接口角度来看
## Predicate

  * filter
  * anyMatch
  * allMatch
  * noneMatch

## Function ToDoubleFunction ToIntFunction  ToLongFunction

  * map
  * mapToInt
  * mapToLong
  * mapToDouble
  * flatMap
  * flatMapToInt
  * flatMapToLong
  * flatMapToDouble

## Consumer

  * peek
  * forEach
  * forEachOrdered

## Collector
collect
## Comparator

  * sorted
  * min
  * max

## BinaryOperator
## BiFunction
## IntFunction
