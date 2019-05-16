---
layout: default
title: Nền tảng Java
description: Giới thiệu về nền tảng Java
---

# Java là gì?
Java la ngôn ngữ lập trình và là một nền tảng để phát triển ứng dụng. Nó được công bố lần đầu bởi Sun năm 1995, sau này được  mua lại bởi Oracle. Nó là một ngôn ngữ lập trình rất phổ biến.

# Nền tảng Java là gì?
Nền tảng Java - Java platform là tập hợp các chương trình mà giúp phát triển và chạy ứng dụng được viết bởi ngôn ngữ Java. Java  platform bao gồm một trình thực thi, một trình biên dịch và một tập hợp các thư viện. Java là ngôn ngữ độc lập nền tảng. Nó không dành riêng cho bộ xử lý hay hệ điều hành nào.

# Trình thực thi của Java - JVM - Java Virtual Machine
![Image](./java-platform-jvm.png)
1. Các mã được viết bằng Java sẽ được lưu dưới dạng .java
2. Để thực thi các file .java sẽ được trình biên dịch biên dịch thành các file .class. 
3. File .class là file chứa các binary code, tuy nhiên các binary code này không được hiểu bởi một máy tính hay chương trình nào mà chỉ dành cho JVM
4. JVM nằm ở RAM trong hệ điều hành của bạn, nó sẽ nhận biết đang xác định đang thực thi trên nền tảng nào mà sẽ biên dịch thành mã máy tương ứng để thực thi chương trình.

Điều mà làm cho Java mạnh mẽ là nó không chỉ chạy trên PC và còn trên cả các thiết bị Mobile hoặc các thiết bị điện tử mà có hỗ trợ Java

# Nền tảng Java độc lập như thế nào
Giống như C, Java không biên dịch mã cho một máy tính cụ thể nào, thay vào đó Java sẽ có một quy chuẩn riêng biệt về mã code, các mã thực thi theo quy tắc mà JVM định nghĩa. Mã code sẽ được hiểu bởi JVM trên bất cứ nền tảng nào. Vì vậy, mã Java có thể chạy trên bất cứ nền tảng nào.  
