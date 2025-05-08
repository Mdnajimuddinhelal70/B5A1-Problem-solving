# Understanding TypeScript: Interface vs Type and the Power of keyof

TypeScript enhances JavaScript by adding static types. It helps developers write safer, cleaner, and more maintainable code. In this blog post, we will explore two essential features of TypeScript: the difference between `interface` and `type`, and the use of the `keyof` keyword.

---

## Interface vs Type in TypeScript

In TypeScript, both `interface` and `type` can be used to describe the shape of an object. However, they are not exactly the same.

**Interface** is mainly used to define the structure of an object, especially in object-oriented designs. One powerful feature of interfaces is *declaration merging*, which allows the same interface name to be declared multiple times, and TypeScript will merge them into a single interface.

**Type**, on the other hand, is more flexible. It can define not only object shapes but also unions, intersections, tuples, and more. Types cannot be merged like interfaces.

In general, interfaces are preferred when working with class-based code or defining object shapes, while types are more useful when you need advanced type composition.

---

## The keyof Keyword in TypeScript

The `keyof` keyword in TypeScript is used to extract the keys of a given type and create a new type based on them.

For example, if you have a type with properties like `name`, `age`, and `email`, using `keyof` on that type will result in a union type: `"name" | "age" | "email"`.

This is especially useful in generic functions where you want to access object properties in a type-safe way. It helps prevent bugs by ensuring that you only access existing keys, improving the safety and predictability of your code.

Using `keyof` makes your functions more reusable, generic, and robust — a big advantage when working on larger projects.

---

## Conclusion

These features—`interface`, `type`, and `keyof`—help make TypeScript a powerful tool for writing robust, scalable, and type-safe applications.

---

## 🔗 Repository Link

You can access the GitHub repository here:  
👉 [https://github.com/Mdnajimuddinhelal70/B5A1-Problem-solving](https://github.com/Mdnajimuddinhelal70/B5A1-Problem-solving)

---


Submitted by: *Md. Najim Uddin*  
Assignment for: *TypeScript 1st Assignment*
