# Covid19_Flutter
1621050078_HoangMinhThang

Tổng quan màn hình: 





























1.	 Setup:

 
Hình 1. Setup pubspec.yaml


	Cài đặt google_maps_flutter
Link: https://pub.dev/packages/google_maps_flutter
2.	Màn hình
Màn hình 1: Hiển thị số liệu về số người mặc bệnh, tử vong, chết của việt nam (các nước khác) và thế giới
Màn hình 2: Hiển thị map, 1 số người mặc bệnh ở việt nam.
3.	Code
 
Hình 2. Main App
HomeScreen

appBar 
 

DropdownButton

 

Chọn một đất nước khác


















Kết quả	
 
Hình 3. Code Dropdown


-	Body: 
Mô tả call api fetchCovidByCountry sẽ lấy dữ liệu từ dropdown khi chọn (khi init app mặc định là Việt Nam) và fetchCovidWord để lấy dữ liệu đổ vào màn hình.


  
Hình 5. Màn hình body

 
Hình 6. Code body


ViewTodo (hiển thị các dữ liệu được lấy về lên màn hình)






Hình 8. Giao diện ViewTodo


Button switch màn hình (chuyển sang màn hình mapScreen)


  


 


MapScreen
Hiển thị vị trí  hiện tại của thiết bị, hiển thị vị trí của 1 số người bị nhiễm bệnh


 

 
Hình 9. Lấy vị trí hiện tại của thiết bị gán vào myLocation


Khởi tạo map

 

Vị trí ban đầu của máy ảnh của bản đồ.

 

Khởi tạo các markers cho bản đồ (đoạn này chưa tìm được api lên e fake tạm);

 


