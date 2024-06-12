# 2048 game

Đây là 1 dự án về trò chơi 2048 bằng C++, mục tiêu của trò chơi là di chuyển các ô vuông sao cho có 1 ô bất kỳ đạt giá trị là 2048 để giành chiến thắng.

## Mục lục

- [Giới thiệu](#giới-thiệu)

- [Cách chơi](#cách-chơi)

- [Liên hệ](#liên-hệ)

## Giới thiệu

## Tác giả:

- **Họ và tên**: Nguyễn Hưng Nguyên
- **MSSV**: 23120149
- **Thời gian hoàn thiện**: Ngày 13/06/2024

## Cài đặt:

Chạy source code 23120149.sln

## Luật chơi:

- Trò chơi bắt đầu trên 1 lưới ô vuông 4x4 (hoặc lớn hơn, tùy vào setting của người chơi) với hai ô có giá trị ngẫu nhiên (2 hoặc 4).
- Người chơi sử dụng các phím mũi tên (**lên, xuống, trái, phải**) hoặc các phím chữ (**W, A, S, D**) để thực hiện việc di chuyển các ô vuông.
- Khi 2 ô vuông có cùng 1 giá trị đụng vào nhau, chúng sẽ tạo nên 1 ô vuông có giá trị gấp đôi (ví dụ: 2 + 2 = 4, 4 + 4 = 8).
- Trò chơi kết thúc khi không còn bước di chuyển hợp lệ nào (không còn khoảng trống và không thể kết hợp các ô vuông).

## Cách thức di chuyển:

- **Phím mũi tên lên (hoặc phím W)**: Di chuyển tất cả các ô vuông lên trên. Các ô vuông sẽ kết hợp nếu có cùng số.
- **Phím mũi tên xuống (hoặc phím S)**: Di chuyển tất cả các ô vuông xuống dưới. Các ô vuông sẽ kết hợp nếu có cùng số.
- **Phím mũi tên trái (hoặc phím A)**: Di chuyển tất cả các ô vuông sang trái. Các ô vuông sẽ kết hợp nếu có cùng số.
- **Phím mũi tên phải (hoặc phím D)**: Di chuyển tất cả các ô vuông sang phải. Các ô vuông sẽ kết hợp nếu có cùng số.

## Chiến lược chơi:

- **Tập trung số lớn ở một góc**: Cố gắng giữ ô vuông có giá trị lớn nhất ở một góc và xây dựng các ô có giá trị nhỏ hơn xung quanh nó.
- **Không di chuyển quá nhiều**: Hạn chế di chuyển các ô vuông nhiều lần mà không tạo ra sự kết hợp để giữ khoảng trống cho các ô mới.
- **Lên kế hoạch trước**: Luôn nghĩ trước một vài bước để xem các di chuyển của bạn sẽ tạo ra điều gì và tránh làm mất các ô quan trọng.

