---
layout: default
title: Java Virtual Machine
description: Giới thiệu về kiến trúc của JVM - Java Virtual Machine
---

Trong mục này chúng ta sẽ tìm hiểu:
1. JVM là gì 
2. Kiến trúc JVM
3. Quá trình biên dịch và thực thi mã Java
4. 

# JVM là gì?
JVM là một máy ảo cung cấp môi trường để chạy các chương trình được viết bằng ngôn ngữ Java. JVM sẽ chuyển đổi mã code được biên dịch từ mã Java thành mã máy và thực thi chúng. JVM là một phần của JRE - Java Runtime Environment. Nó được gọi là Máy ảo Java - Java Virtual Machine.

Đối với các ngôn ngữ khác, trình biên dịch sẽ thực hiện biên dịch mã code thành mã máy cho từng hệ thống cụ thể. Tuy nhiên, trình biên dịch Java thực hiện biên dịch mã Java thành mã chỉ dành cho JVM và chỉ được hiểu bởi JVM.
Đầu tiên, Java code sẽ được biên dịch thành mã bytecode, mã bytecode này sẽ được JVM biên dịch thành mã máy tương ứng với từng hệ điều hành cụ thể. Giữa máy tính và source code Java, mã bytecode Java là trung gian. JVM chịu trách nhiệm phân bổ nó vào bộ nhớ máy tính để thực thi.

# Kiến trúc JVM
![Kiến trúc JVM](./images/java-virtual-machine-jvm.png)

## 1. ClassLoader
Class Loader là một hệ thống con được sử dụng để tải các file .class - được biên dịch từ file .java. Nó thực hiện 3 nhiệm vụ chính: Tải file class(Loading), Liên kết(Linking) và Khởi tạo(Initialization)

## 2. Method Area
Là nơi chứa cấu trúc của Class, giống như metadata, cấu trúc này không thay đổi trong quá trình chạy, và nó chứa các mã của các method - phương thức.

## 3. Heap
Tất cả các Object, các biến liên quan và các mảng được chứa trong vùng Heap. Vùng nhớ này được chia sẻ đồng thời cho nhiều threads.

## 4. JVM language Stacks
Java language Stacks chứa các biến local, và một phần kết quả của chúng. Mỗi thread sẽ có JVM stack riêng biệt, được tạo đồng thời lúc thread được tạo. Một vùng mới được tạo bất cứ khi nào một method được gọi và nó sẽ được xóa đi khi quá trình gọi method đó được hoàn thành.

## 5. PC Registers
PC Registers lưu địa chỉ của JVM đang thực thi. Trong Java, mỗi thread đều có PC Registers của riêng nó.

## 6. Native Method Stacks
Native Method Stacks lưu các hướng dẫn đến các thư viện liên kết, các thư viện này được viết bằng ngôn ngữ khác ngoài Java.

## 7. Execution Engine
Nó là một kiểu phần mềm được dùng để kiểm tra phần cứng, phần mềm hoặc hệ thống.
It is a type of software used to test hardware, software, or complete systems. The test execution engine never carries any information about the tested product.

## 8. Native Method interface
Native Method interface là một khung lập trình. Nó cho phép mã Java đang chạy trong JVM để gọi bởi các thư viện và ứng dụng gốc.
The Native Method Interface is a programming framework. It allows Java code which is running in a JVM to call by libraries and native applications.

## 9. Native Method Libraries
Native Method Libraries là một tập hợp các Thư viện riêng (C, C ++) cần thiết cho Công cụ thực thi.
Native Libraries is a collection of the Native Libraries(C, C++) which are needed by the Execution Engine.

