# Chinh Phạt Cửu Châu – Khung Thiết Kế MVP (Paper + MMOCore stack)

## 1) Trụ cột thiết kế

**Triết lý cốt lõi:** Không khóa class, khóa **build**.

- Người chơi nào cũng có thể học võ công nếu có **bí kíp**.
- Không ai có thể ôm toàn bộ sức mạnh vì bị giới hạn bởi:
  - slot kỹ năng,
  - yêu cầu vũ khí,
  - yêu cầu chỉ số,
  - tài nguyên nội tức,
  - hồi chiêu và tương khắc meta.

## 2) Core loop gameplay

Farm quái / nhiệm vụ / phụ bản → nhận exp + nguyên liệu + bí kíp + trang bị → tăng cấp + mở slot + mở thiên phú/cảnh giới → tối ưu build → tham gia boss/chinh chiến lãnh thổ → nhận tài nguyên bậc cao → quay lại vòng lặp.

## 3) Progression 1–100 (đề xuất MVP khả thi)

## 3.1 Mốc mở slot kỹ năng

| Mốc level | Mở khóa |
|---|---|
| 1 | 1 Active |
| 10 | +1 Active (tổng 2) |
| 20 | +1 Active (tổng 3) |
| 30 | 1 Passive |
| 40 | +1 Active (tổng 4) |
| 50 | +1 Passive (tổng 2) |
| 60 | 1 Ultimate |
| 70 | 1 Talent nhánh phụ |
| 80 | +1 Passive (tổng 3) |
| 90 | +1 Talent nhánh chính |
| 100 | 1 Ultimate augment / rune |

## 3.2 Cảnh giới (nội công)

| Cảnh giới | Điều kiện | Thưởng chính |
|---|---|---|
| Luyện Thể | Lv 15 + nhiệm vụ nhập môn | +HP cơ bản, mở bảng cảnh giới |
| Thông Mạch | Lv 30 + phụ bản 1 | +Nội tức tối đa, +1 passive node |
| Tụ Khí | Lv 45 + boss trấn thủ | Tăng hiệu quả skill nội công |
| Hóa Kình | Lv 60 + chuỗi truyền thừa | Mở Ultimate slot |
| Tông Sư | Lv 80 + danh vọng châu | Nâng trần chỉ số build |
| Tuyệt Đỉnh | Lv 100 + chiến dịch liên server (tuỳ giai đoạn) | Aura/Nameplate + đặc quyền endgame |

## 4) Bộ chỉ số theo chất Tam Quốc

Tên hiển thị frontend (backend map về stat kỹ thuật của MythicLib/MMOCore):

- **Võ Lực**: damage cận chiến, xuyên phá.
- **Thân Pháp**: tốc đánh, né tránh, cơ động.
- **Nội Tức**: năng lượng kỹ năng, hồi năng lượng, cường hóa kỹ năng.
- **Mưu Trí**: hiệu quả khống chế/debuff/buff chiến thuật.
- **Căn Cốt**: HP, thủ, kháng.
- **Khí Vận**: chí mạng, may mắn rơi đồ, cơ duyên sự kiện.

## 5) Build framework (không class cứng)

Dùng 1 class nền: **Hào Kiệt**.

Build được hình thành bởi 3 lớp:

1. **Vũ khí chính**: Kiếm / Thương / Cung (MVP phase 1).
2. **Nhóm võ học**: Ngoại công / Nội công / Thân pháp / Mưu thuật.
3. **Phong cách chiến đấu**: Burst, Duel, AoE, Du kích, Chống chịu, Hỗ trợ.

=> Cùng học bí kíp nhưng build khác nhau do khác vũ khí + phân bổ stat + slot loadout.

## 6) Hệ bí kíp (xương sống retention)

## 6.1 Phân hạng

Phàm phẩm → Lương phẩm → Trân phẩm → Địa phẩm → Thiên phẩm → Tuyệt học.

## 6.2 Nguồn rơi

- Quái thường / tinh anh.
- World Boss theo giờ.
- Phụ bản.
- Chuỗi nhiệm vụ truyền thừa.
- Shop danh vọng châu.
- Sự kiện tranh đoạt lãnh thổ.

## 6.3 Điều kiện sử dụng hiệu quả

- Đúng loại vũ khí.
- Đủ ngưỡng chỉ số (ví dụ Võ Lực/Nội Tức).
- Đạt danh vọng châu tối thiểu.
- Hoàn thành nhiệm vụ mở khóa truyền thừa.

Nếu chưa đạt điều kiện: vẫn học được nhưng bị giảm hiệu năng (đúng triết lý “học tự do, dùng có giá”).

## 7) Bản đồ Cửu Châu = tiến trình gameplay

## Giai đoạn MVP (2 châu đầu)

### U Châu (newbie)

- Quái: sơn tặc, sói, đào binh.
- Mục tiêu: làm quen slot skill + vũ khí + nội tức.
- Nội dung: nhiệm vụ chính tuyến + mini boss doanh trại.

### Ký Châu (mid-early)

- Quái: quân phiệt địa phương, vệ binh hạng nặng.
- Nội dung: phụ bản lăng mộ 3 người + world boss theo khung giờ.
- Mở danh vọng châu + thương nhân bí kíp cấp cao hơn.

## 8) Endgame trục kép (để tránh “farm boss xong nghỉ”)

1. **Tranh đoạt lãnh thổ** (bang hội)
   - Điểm tranh: mỏ sắt, kho lương, đồn biên, thành trấn.
   - Quyền lợi: thuế tài nguyên, buff farm/exp, mở boss đặc biệt.

2. **Danh vọng cá nhân + bang hội**
   - Mở shop, danh hiệu, nhiệm vụ ẩn, vật phẩm truyền thừa.

3. **PVE thử thách theo mùa**
   - Solo trial, tổ đội, thủ thành, hộ tống quân lương.

## 9) Mapping vào plugin hiện tại

- **MMOCore**: level, stat point, skill slot, resource (mana/energy).
- **MythicLib**: custom stat, scaling formula, combat trigger.
- **MMOItems**: vũ khí/giáp/trang sức, set bonus, affix.
- **MythicMobs**: quái/boss/phụ bản/drop bí kíp.
- **Nexo**: model bí kíp, token, đạo cụ quest.
- **LuckPerms**: quyền truy cập mốc tính năng, rank danh vọng.
- **CMI**: warp/mail/alias/QoL.
- **WorldEdit**: dựng map châu, phụ bản, chiến trường.

## 10) 5 build mẫu để chốt meta đầu mùa

1. **Thương Kỵ Xung Phong** (Võ Lực + Thân Pháp)
2. **Kiếm Khách Du Long** (Thân Pháp + Nội Tức)
3. **Mưu Sĩ Khống Trận** (Mưu Trí + Nội Tức)
4. **Đao Tướng Trấn Quân** (Võ Lực + Căn Cốt) – mở ở phase 2
5. **Xạ Thủ Phá Quân** (Thân Pháp + Khí Vận)

## 11) Lộ trình phát triển thực tế

## Phase 1 (MVP ra mắt)

- 1 class nền Hào Kiệt.
- 3 vũ khí (Kiếm, Thương, Cung).
- 12–15 kỹ năng tổng.
- 2 châu đầu (U Châu, Ký Châu).
- 1 phụ bản + 2 world boss.
- 1 khu bang chiến nhỏ.

## Phase 2

- Mở Đao, Phiến/Trượng.
- Bổ sung nội công + bị động nâng cao.
- Hệ danh vọng châu hoàn chỉnh.
- Thành chiến theo khung giờ.

## Phase 3

- Mở đủ Cửu Châu.
- Boss trấn châu + world event theo mùa.
- Trang bị/set theo phe hoặc truyền thừa.
- BXH chiến công + danh vọng toàn server.

---

## Kết luận ngắn gọn

Nếu giữ đúng công thức:

- **Học skill tự do** (bí kíp),
- **Dùng skill hữu hạn** (slot + điều kiện),
- **Endgame tranh đoạt thực sự** (lãnh thổ + danh vọng),

thì “Chinh Phạt Cửu Châu” sẽ có bản sắc riêng, khác biệt rõ với server class-based thông thường.
