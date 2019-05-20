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

