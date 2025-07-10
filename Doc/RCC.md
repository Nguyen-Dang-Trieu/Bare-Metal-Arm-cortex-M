
Cấu hình xung clock cho `STM32F103C8T6` dùng HSE chạy ở 72 `MHz` dùng cho Keil C 
- Khi Keil C mở lên, ta cần phải bật HSE trước (vì mặc định là tắt) -> Trong mục Pinout & Configuration, Vào RCC -> Chọn HSE: Crystal/Ceramic Resonator
- HSE input: 8 MHz (hoặc giá trị đúng với thạch anh bạn dùng)
- PLL Source Mux: chọn HSE
- PLL Mul: chọn x9
- SYSCLK: chọn 72 MHz
- APB1 Prescaler: /2 (bắt buộc, vì APB1 max 36 MHz)
- APB2 Prescaler: /1
- HCLK: 72 MHz
