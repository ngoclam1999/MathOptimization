# MathOpt Studio

Ứng dụng web local giúp học tối ưu hóa bằng mô phỏng từng bước.

## Chạy

Mở `index.html` bằng Chrome hoặc Edge. Ứng dụng không cần cài package và không gửi dữ liệu ra ngoài.

Hoặc chạy server local đi kèm:

```powershell
node server.js
```

Sau đó mở `http://127.0.0.1:4173`.

Để tránh một số giới hạn khi trình duyệt mở trực tiếp file, có thể chạy bằng server tĩnh bất kỳ rồi mở `http://localhost:<port>`.

## Bài học tương tác hiện có

- Quy hoạch tuyến tính — Đơn hình thuận.
- Quy hoạch tuyến tính — Đơn hình đối ngẫu với quy tắc RHS âm.
- Quy hoạch nguyên — Nhánh & Cận từ nghiệm LP relaxation.
- Phương pháp hình học — miền khả thi bị chặn, giao điểm, giá trị tại các đỉnh và đường mức.
- Phương pháp hình học — miền không bị chặn và tia cải thiện.
- Bài toán vận tải — phương pháp chi phí thấp nhất (phương án khả thi ban đầu).
- Bài toán vận tải — phương pháp Góc Tây Bắc.
- Bài toán vận tải — phương pháp Thế vị MODI.
- Bài toán phân công — Hungarian trên ma trận vuông.
- Bài toán phân công — Nhánh & Cận.
- Đường đi ngắn nhất — Dijkstra trên đồ thị vô hướng, trọng số không âm.
- Bài toán người du lịch — Lân cận gần nhất.
- Bài toán người du lịch — Thuật toán di truyền tái lập bằng seed.

Mỗi bài có: dữ liệu chỉnh sửa được, phép tính từng bước, giải thích “vì sao”, bảng trạng thái, hình minh họa canvas, phát tự động và điều khiển tốc độ.

## Phím tắt

- `←` / `→`: bước trước / bước tiếp.
- `Space`: chạy / tạm dừng.

## Giới hạn đã nêu rõ trong UI

- Chi phí thấp nhất chưa tự chứng minh tối ưu; cần bổ sung MODI/Stepping-stone.
- MODI hiện yêu cầu phương án cơ sở không suy biến; ứng dụng báo rõ nếu cần thêm ô ε.
- Đơn hình thuận hiện nhận bài toán Max hai biến, ràng buộc `<=`, RHS không âm.
- Đơn hình đối ngẫu minh họa trên tableau hai ràng buộc có cơ sở slack ban đầu.
- Trình giải hình học và Nhánh & Cận nguyên hiện dành cho mô hình hai biến.
- Hungarian trong bản này nhận ma trận vuông.
- Dijkstra từ chối trọng số âm.
- Lân cận gần nhất và Di truyền là heuristic, không chứng minh tối ưu toàn cục.
"# MathOptimization" 
