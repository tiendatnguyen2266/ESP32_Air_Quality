# ESP32_Air_Quality

## Giới thiệu
**ESP32_Air_Quality** là một dự án đo chất lượng không khí sử dụng board vi điều khiển ESP32 và các cảm biến môi trường. Dự án thu thập dữ liệu từ các cảm biến như nhiệt độ, độ ẩm, và chất lượng không khí (PM2.5, CO2) để:  
- Giám sát chất lượng không khí theo thời gian thực.  
- Hiển thị dữ liệu trên màn hình hoặc ứng dụng web.  
- Gửi dữ liệu lên dịch vụ đám mây (Firebase, MQTT, Thingspeak, v.v.).  

## Tính năng chính
- **Đo lường môi trường:**  
  - Nhiệt độ và độ ẩm.  
  - Chỉ số chất lượng không khí (PM2.5, CO2).  
- **Kết nối IoT:**  
  - Gửi dữ liệu lên Firebase hoặc MQTT.  
  - Xem dữ liệu từ xa qua ứng dụng hoặc dashboard.  
- **Cảnh báo:**  
  - Hiển thị cảnh báo nếu chất lượng không khí vượt mức an toàn.  

## Phần cứng yêu cầu
- **Vi điều khiển:** ESP32.  
- **Cảm biến:**  
  - Cảm Biến Bụi GP2Y1010AU0F
  - BME680 (nếu có) hoặc thay thế bằng cảm biến khác.  
- **Khác:**  
  - Màn hình TFT.  
  - Nguồn cấp: 5V Micro USB hoặc có thể dùng pin.

## Phần mềm sử dụng
- **Arduino IDE:** Viết và nạp code cho ESP32.  
- **Firebase/Thingspeak:** Lưu trữ và hiển thị dữ liệu.  
- **Thư viện:**  
  - `Adafruit_Sensor.h` (nếu sử dụng cảm biến khác).  
  - `WiFi.h` (kết nối Wi-Fi).  
  - `Firebase_ESP_Client.h` (nếu dùng Firebase).