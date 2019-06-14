---
layout: default
title: Từ khóa THIS trong Java
description: Từ khóa THIS trong Java
---

# Từ khóa THIS trong Java là gì
Từ khóa **THIS** là một biến tham chiếu trong Java dùng tham chiếu đến đối tượng hiện tại.

Các cách sử dụng khác nhau của **THIS** trong Java như sau:
- Nó có thể sử dụng để tham chiếu đến một biến thể hiện(instance variable) của class hiện tại
- Nó có thể sử dụng để gọi hoặc khởi tạo constructor của class hiện tại
- Nó có thể được truyền như một tham số trong method gọi
- Nó có thể được truyền như một tham số trong constructor gọi
- Nó có thể được dùng để trả về thể hiện của class hiện tại

# Tìm hiểu từ khóa THIS với ví dụ

![Từ khóa THIS trong Java](./images/java-this-keyword-1.png)

1. Class: class Account
2. Instance Variable: a và b
3. Method Set data: Để set giá trị cho a và b
4. Method Show data: Để hiển thị giá trị a và b
5. Main method: Nơi mà chúng ta tạo một object của class Account và gọi method set data và show data.

Biên dịch source code và chạy thử.

Kết quả mong muốn của chúng ra cho A và B nên được khởi tạo giá trị 2 và 3 tương ứng.

Nhưng giá trị là 0. Tại sao? Hãy điều tra xem.

![Từ khóa THIS trong Java](./images/java-this-keyword-2.png)

Trong method Set data, các tham số được khai báo là a và b, trong khi instance biến cũng có tên là a và b.

![Từ khóa THIS trong Java](./images/java-this-keyword-3.png)

Trong khi thực thi, trình biên dịch hơi bối rối. Liệu "a" bên trái của toán tử là instance biến hay local biến. Tóm lại, nó không set giá trị của "a" khi method set data được gọi.

![Từ khóa THIS trong Java](./images/java-this-keyword-4.png)

Giải pháp là từ khóa **THIS**.

Thêm vào cho cả 2 a và b từ khóa **this**, theo sao bởi toán tử chấm (**.**)

![Từ khóa THIS trong Java](./images/java-this-keyword-5.png)

Trong khi thực thi code, khi một đối tượng gọi method "sendData". Từ khóa **this** sẽ được thay thế bởi đối tượng xử lý "obj". Xem hình bên dưới.

![Từ khóa THIS trong Java](./images/java-this-keyword-6.png)

Bây giờ, trình biên dịch sẽ biết rằng:
- "a" phía bên tay trái là biến instance
- Trong khi, "a" bên tay phải là biến local

Các biến sẽ được khởi tạo chính xác, và kết quả mong muốn sẽ được hiển thị.

![Từ khóa THIS trong Java](./images/java-this-keyword-7.png)

Giả sử, bạn đủ thông minh để chọn tên biến khác nhau cho biến instance và tham số của method.

![Từ khóa THIS trong Java](./images/java-this-keyword-8.png)

Nhưng trong lúc này, bạn tạo 2 đối tượng của class Account, mỗi đối tượng đều gọi đến method sendData.



[Back](./)
