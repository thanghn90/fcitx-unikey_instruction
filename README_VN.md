[English](README.md)
# Tại sao dùng fcitx-unikey?
Chắc hẳn bạn đã biết đến ibus-unikey và ibus-bamboo là các công cụ gõ tiếng Việt thông dụng nhất trên Linux. Tuy nhiên, nếu bạn dùng ibus-unikey hay ibus-bamboo với phiên bản WPS Office cho Linux mới nhất (wps-2019-snap trên SNAP store, build 9125), bạn sẽ thấy các chương trình của WPS Office mở lên rất chậm. (Lưu ý là nếu bạn cài file deb download trực tiếp từ trang chủ của wps office, lúc gõ tiếng Việt sẽ không thấy hiển thị bất kì gì cho tới khi bấm nút cách " ", đối với cả fcitx và unikey). Trong khi đó, fcitx-unikey không hề gặp vấn đề chậm mở app này, khả năng nhiều là do một lỗi không tương thích giữa thư viện qt và gtk trong module ibus. Ngoài ra, hướng dẫn sử dụng fcitx-unikey trên mạng hiện nay vẫn rời rạc và không hoàn chỉnh. Vì thế, tôi viết bài này, mong đem đến cho bạn đọc một hướng dẫn chi tiết từng bước nhằm giúp bạn cài đặt và sử dụng fcitx-unikey để gõ tiếng Việt.

# Hướng Dẫn Chi Tiết Từng Bước
1. Trước hết, bạn cần cài tiếng Việt. Nhớ kết nối internet. Vào Start --> Settings --> Language Support

![alt text](https://github.com/thanghn90/fcitx-unikey_instruction/blob/main/1.%20Settings%20Language.png)

2. Nếu có thông báo "incomplete language package", bỏ qua. Sau đó ấn nút "Install/Remove Languages...":

![alt text](https://github.com/thanghn90/fcitx-unikey_instruction/blob/main/2.%20Install%20New%20Language.png)

3. Kéo xuống, ấn đúp trái chuột vào "Vietnamese" để nó tô đậm và dòng chữ "1 to install" xuất hiện:

![alt text](https://github.com/thanghn90/fcitx-unikey_instruction/blob/main/3.%20Install%20Vietnamese.png)

Sau đó ấn "Apply". Nó sẽ tự động tải và cài đặt các module cần thiết cho tiếng Việt, bao gồm - may mắn thay - fcitx và fcitx-unikey! Sau khi cài xong tiếng Việt, log out rồi log in (hoặc khởi động lại máy).

4. Mở lại Language Support (Start --> Settings --> Language Support). Lần này, đổi "Keyboard Input Method System" thành "fcitx":

![alt text](https://github.com/thanghn90/fcitx-unikey_instruction/blob/main/4.%20Change%20Input%20Method.png)

5. Tiếp theo, bật fcitx bằng cách vào Start --> System --> Fcitx:

![alt text](https://github.com/thanghn90/fcitx-unikey_instruction/blob/main/5.%20Start%20fcitx.png)

6. Biểu tượng fcitx hình nút "a" sẽ xuất hiện ở thanh status. Nhấn trái chuột vào biểu tượng đó --> "Configure":

![alt text](https://github.com/thanghn90/fcitx-unikey_instruction/blob/main/6.%20Configure%20fcitx.png)

7. Cần cài thêm input method mới là "Unikey", bằng cách ấn nút hình dấu cộng "+" gần góc trái bên dưới của cửa sổ fcitx configure:

![alt text](https://github.com/thanghn90/fcitx-unikey_instruction/blob/main/7.%20Add%20New%20Input%20Method.png)

8. Bỏ chọn "Only Show Current Language", rồi gõ "Unikey" ở ô tìm kiếm (chú ý viết hoa chữ "U"), chọn Unikey, rồi bấm OK:

![alt text](https://github.com/thanghn90/fcitx-unikey_instruction/blob/main/8.%20Unikey.png)

9. Đến đây bạn cần có 2 input methods:

![alt text](https://github.com/thanghn90/fcitx-unikey_instruction/blob/main/9.%20Final%20Input%20Methods.png)

10. Trong "Global Config" tab, bạn có thể thay đổi tổ hợp phím "Trigger Input Method". Tôi chọn Alt+Z để giống với Unikey trên Windows:

![alt text](https://github.com/thanghn90/fcitx-unikey_instruction/blob/main/10.%20Switch%20Keyboard%20Shortcut.png)

11. Trong "Appearance" tab, tăng font size của hộp gõ tiếng Việt hiển thị trong WPS Office (xem hình cuối, bước 13):

![alt text](https://github.com/thanghn90/fcitx-unikey_instruction/blob/main/11.%20Hint%20Appearance.png)

12. Để đổi ngôn ngữ gõ (từ tiếng Việt sang tiếng Anh và ngược lại), bạn có thể dùng tổ hợp phím set up như bước 10, hoặc bấm vào biểu tượng của fcitx trên thanh status --> Input Method. Lưu ý là ngôn ngữ gõ chỉ thay đổi khi chuột đang nhấp nháy ở ô gõ nào đó. Ngôn ngữ gõ sẽ không thay đổi, ví dụ, trong trường hợp bạn ở ngoài desktop và không đang gõ gì cả.

![alt text](https://github.com/thanghn90/fcitx-unikey_instruction/blob/main/12.%20Switch%20Input%20Method.png)

13. Đây là hộp gõ tiếng Việt trong WPS Office:

![alt text](https://github.com/thanghn90/fcitx-unikey_instruction/blob/main/13.%20WPS%20Unikey%20Demo.png)
