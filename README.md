# Nihon no Benkyou — Japanese Library | Cinema + Music

Ứng dụng học tiếng Nhật **all-in-one** chạy hoàn toàn trên trình duyệt (1 file HTML).  
Giao diện tối, cảm hứng Netflix + Spotify, tối ưu cho việc học qua **phim / nhạc / thẻ từ / JLPT**.

---

## ✨ Tính năng chính

| Mục | Mô tả |
|-----|--------|
| **Trang chủ** | Tổng quan thư viện video, nhạc, mục tiêu & streak học hàng ngày |
| **Từ vựng** | Sổ thẻ (flashcard), đánh dấu đã thuộc / chưa thuộc, nhóm theo nguồn |
| **Hán tự** | Học kanji riêng |
| **Ngữ pháp** | Lưu cấu trúc ngữ pháp (tách biệt với từ vựng) |
| **Quiz thẻ** | Quiz ngẫu nhiên từ sổ từ của bạn (nhiều chế độ) |
| **JLPT Quiz** | Luyện đề theo format JLPT |
| **Video (Cinema)** | Xem phim/series local, phụ đề JP click được → thêm từ ngay vào sổ |
| **Nhạc** | Nghe nhạc + lời (LRC/SRT), click từ trong lời để lưu |
| **Từ điển** | Tra cứu offline trong app |
| **Sao lưu** | Export / import dữ liệu (JSON), đồng bộ theo tài khoản |

**Điểm nổi bật**
- Click vào **từ tiếng Nhật** trên phụ đề video hoặc lời bài hát → mở form thêm vào sổ từ / ngữ pháp.
- Hỗ trợ **series + số tập** (xem như Netflix: chọn series → danh sách tập).
- Album nhạc + ảnh bìa (vinyl spinning khi phát).
- Dữ liệu lưu **IndexedDB** trên trình duyệt (video/nhạc/phụ đề có thể lưu local).
- Giao diện tiếng Việt, dark mode.

---

## 🚀 Cách chạy

1. Tải file `nihonnobenkyou.html`.
2. Mở bằng trình duyệt (Chrome / Edge / Firefox khuyến nghị).
3. Không cần cài đặt, không cần server.

> File khá nặng (~45MB) vì gói sẵn từ điển + logic offline. Lần đầu mở có thể hơi chậm vài giây.

---

## 📖 Hướng dẫn sử dụng nhanh

### 1. Học qua Video
1. Vào tab **Video**.
2. Thêm video local (MP4 / WebM / MKV…) + file phụ đề Nhật (`.srt` / `.vtt` / `.ass`).
3. (Tuỳ chọn) Gán **tên series** + **số tập** để quản lý như series.
4. Khi xem, phụ đề JP hiện trên video → **click vào từ** → thêm vào sổ từ vựng hoặc ngữ pháp.
5. Dùng nút **Tập trước / Tập sau** nếu đã phân loại series.

### 2. Học qua Nhạc
1. Vào tab **Nhạc**.
2. Thêm file audio (MP3, M4A…) + lời (`.lrc` / `.srt`).
3. Gán album nếu muốn nhóm bài + ảnh bìa.
4. Click từ trong lời bài hát để lưu vào sổ.

### 3. Từ vựng & Flashcard
- Tab **Từ vựng**: xem / sửa / xoá thẻ, đánh dấu “đã thuộc”.
- Tab **Quiz thẻ**: chọn nguồn, chế độ, số câu → luyện.
- Có thể lọc chỉ học từ **chưa thuộc**.

### 4. JLPT & Daily
- **JLPT Quiz**: luyện theo dạng đề.
- Trang chủ có **mục tiêu hàng ngày** + streak (chuỗi ngày học liên tiếp).

### 5. Sao lưu dữ liệu
1. Tab **Sao lưu**.
2. **Export** ra file JSON (giữ toàn bộ thẻ, ngữ pháp, thư viện…).
3. Máy mới / trình duyệt khác → **Import** file đó lại.

> Nên export định kỳ. Dữ liệu nằm trong trình duyệt; xoá cache / đổi máy sẽ mất nếu chưa backup.

---

## 📁 Định dạng file hỗ trợ

**Video:** `.mp4`, `.webm`, `.mkv`, `.mov`…  
**Phụ đề video:** `.srt`, `.vtt`, `.ass`, `.ssa`  
**Nhạc:** `.mp3`, `.m4a`, `.aac`, `.ogg`, `.wav`…  
**Lời nhạc:** `.lrc`, `.srt`, `.vtt`  
**Sao lưu:** `.json`

---

## 💡 Mẹo

- Muốn lấy phụ đề từ YouTube: dùng [downsub.com](https://downsub.com) (chọn Japanese).
- Video YouTube: tải MP4 về máy (y2mate…) rồi thêm vào app (nhúng trực tiếp bị hạn chế).
- MKV trình duyệt không phát được → app sẽ cố **remux sang MP4** (không encode lại video).
- Dùng Chrome/Edge để tương thích IndexedDB + file lớn tốt nhất.

---

## 🛠 Kỹ thuật

- Single-page app (HTML + CSS + JS thuần).
- Lưu trữ: **IndexedDB** (media) + localStorage (cài đặt / progress).
- Không phụ thuộc server; chạy offline sau khi mở lần đầu.
- Giao diện responsive, hỗ trợ fullscreen video + phụ đề overlay kiểu Netflix.

---

## License / Ghi chú

Project cá nhân học tiếng Nhật.  
Có thể fork / chỉnh sửa tự do cho mục đích học tập.
