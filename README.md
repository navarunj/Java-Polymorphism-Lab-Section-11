# Java-Polymorphism-Lab-Section-11

Polymorphism allows an object reference of a generic type to point to an object of a
more specific type. For example, a Good reference can point to a Solid or Liquid
product object. In this lab, you use polymorphism to assign any type of good to an
order’s product field. You also explore the equals( ) method to compare MyDate
objects.

Specifically, in this lab you will:
* Update the Order type to use polymorphism and the good type hierarchy (Good,
Liquid, Solid) for products, rather than using a string
* Update MyDate to override the polymorphic equals( ) method from
java.lang.Object.
* Optionally explore the cast operation to cast a general reference back to a more
specific type of object.

## Scenario
Given the product hierarchy (Good, Solid, Liquid), you now have a fine set of
“product” objects to associate with an order (replacing the current String for
product). Of course, an order could be for a Solid or a Liquid type, so what type
should be used on the product field of Order? Here is where polymorphism can help
out. 

## Step 1: Refactor Order

Currently, the product field on Order is of type String. Now it is time to associate the
Good type objects to orders.

1.1 Change the product field’s type. In the Package Explorer view, double-click
on the Order.java file in the com.acme.domain package to open the file in a
Java editor.

<img src="./src/main/resources/selectOrder.png" width="400px">

In Order.java, change the type of product from String to Good.

```java
private Good product;
```


