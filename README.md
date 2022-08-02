# Class

## Learning Goals

- Explain a Class

## Classes in Java

Java is an object-oriented programming language. This means it thinks of the world as "objects", which then have
"properties" and "actions".

For example, a bicycle is an object that has a color and a height (expressed in inches).

If we were to think about describing this object in writing, we might come up with something like this:

- Object name: `bicycle`
- Object properties:
  - `color`
  - `height in inches`

Let's say you and I both have a bicycle. How do we distinguish your bike from my bike? Both of these "objects" have the
same overall properties, except that yours is yellow and mine is silver, and they have different heights.

In an object-oriented programming language, like Java, the general description of an object's "properties" and "actions"
that are used to construct an **object** is called a **class**. Whereas **objects** are _instances_ of a **class**.

To use another example from our everyday life, we can think of the class as the blueprint for a house, and the object as
a specific house, which are both based on the same blueprint, i.e. they have the same number of rooms and
the same layout.

Using the syntax we've already seen in this unit, our Bicycle example might yield a class like this:

```java
public class Bicycle {
    String color; 
    int height;
} 
```

Here are a few things to note:

- By convention, in Java the name of the class always starts with an uppercase character.
  - If the name of the class has multiple words in it, each word starts with an uppercase character. Example: 
  `ClassicBicycle`.
    - This is often referred to as "**pascal case**", meaning multiple words are put together where each word starts
    with an uppercase character.
    - In Java, class names are pascal case, starting with an uppercase character.
- The `public` keyword is covered in a section below.
- The `class` keyword indicates we are defining a new Java class.
- The open curly brace `{` indicates the beginning of the class definition and has a matching close curly brace `}` at
the end of the class definition.
- Each property is defined on its own line with a `;` at the end
- Each property has a "type" and a "name". The name is how we want to be able to refer to the property and the type
allows us to tell Java what type of value we expect this property to be. In this example, we expect the `color`
to be a "word" and the `height` to be a "number". We will learn more on these exact types later on.

Before we learn more about types, let's dig into objects some more!
