---
layout: default
title: Khái niệm OOP trong Java
description: Khái niệm OOP trong Java
---

# OOP là gì?
Object Oriented Programming là một khái niệm lập trình mà nó làm việc dựa trên nguyên tắc là các đối tượng là một phần quan trọng nhất của chương trình. Nó cho phép người dùng tạo những đối tượng mà họ muốn và cũng tạo ra phương thức để xử lý các đối tượng đó. Thao tác những đối tượng để lấy kết quả là mục tiêu của Object Oriented Programming.

Object Oriented Programming được biết phổ biến với tên OOP, nó được sử dụng trong các ngôn ngữ lập trình hiện đại như Java. 

# Những khái niệm cơ bản trong OOP
## 1. Class
Class là một nhóm các thực thể giống nhau, nó chỉ là thành phần logic, không phải là thành phần vật lý. Ví dụ, nếu bạn có một class được gọi là “Expensive Cars”, nó có thể có những đối tượng như Mercedes, BMW, Toyota, etc. Những thuộc tính(data) của nó có thể là giá xe(price) hoặc tốc độ(speed) của những chiêc xe. Trong khi những phương thức có thể thực hiện với những chiếc xe như là lái xe(driving), lùi xe(reverse), đỗ xe(braking), ...

## 2. Objects
Một đối tượng có thể được định nghĩa như một bản sao của một class, và có thể có nhiều bản sao của một class trong một chương trình. Một đối tượng chứa data và các chức năng, nó hoạt động dựa trên data. Ví dụ như cái bàn, xe đạp, cây bút, ...

## 3. Kế thừa
Kế thừa là một khái niện của OOP, trong đó một đối tượng có được các thuộc tính và hành vi của đối tượng cha. Nó tạo nên quan hệ cha-con giữa hai class. Nó cung cấp cơ chế mạnh mẽ và tự nhiên để cấu trúc và tổ chức cho bất cứ phần mềm nào.

## 4. Polymorphism

Polymorphism refers to the ability of a variable, object or function to take on multiple forms. For example, in English, the verb run has a different meaning if you use it with a laptop, a foot race, and business. Here, we understand the meaning of run based on the other words used along with it.The same also applied to Polymorphism.

## 5. Abstraction

An abstraction is an act of representing essential features without including background details. It is a technique of creating a new data type that is suited for a specific application. For example, while driving a car, you do not have to be concerned with its internal working. Here you just need to concern about parts like steering wheel, Gears, accelerator, etc.

## 6. Encapsulation

Encapsulation is an OOP technique of wrapping the data and code. In this OOPS concept, the variables of a class are always hidden from other classes. It can only be accessed using the methods of their current class. For example - in school, a student cannot exist without a class.

## 7. Association

Association is a relationship between two objects. It defines the diversity between objects. In this OOP concept, all object have their separate lifecycle, and there is no owner. For example, many students can associate with one teacher while one student can also associate with multiple teachers.

## 8. Aggregation

In this technique, all objects have their separate lifecycle. However, there is ownership such that child object can’t belong to another parent object. For example consider class/objects department and teacher. Here, a single teacher can’t belong to multiple departments, but even if we delete the department, the teacher object will never be destroyed.

## 9. Composition

A composition is a specialized form of Aggregation. It is also called "death" relationship. Child objects do not have their lifecycle so when parent object deletes all child object will also delete automatically. For that, let’s take an example of House and rooms. Any house can have several rooms. One room can’t become part of two different houses. So, if you delete the house room will also be deleted.

[Back](./)