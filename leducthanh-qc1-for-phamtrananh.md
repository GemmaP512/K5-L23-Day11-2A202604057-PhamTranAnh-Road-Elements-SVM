# Phiếu QC 1 — Road v1.0

Lô được kiểm (học viên): Phạm Trần Anh        Người kiểm (học viên): Lê Đức Thanh  
Ngày: 20/11/2026                          Phiên bản guideline: Road v1.0  
File được kiểm (tên + `revision` trong manifest): `phamtrananh-front.zip`, `phamtrananh-fisheye.zip`; revision 1 theo `phamtrananh-manifest.json`.  
Số ảnh kiểm: 6 theo mẫu lab, chờ người kiểm xác nhận danh sách và hoàn tất kiểm trực quan (+ số ảnh thêm chờ xác nhận). Số nhãn đã kiểm (shape + tag): chờ người kiểm xác nhận.

Phiếu dự thảo từ kết quả tự kiểm bằng script trên 20 ảnh, gồm 123 shape và 80 tag. Lê Đức Thanh cần xác nhận kết quả kiểm trực quan, số nhãn đã kiểm và quyết định cuối cùng. Hai job đã Completed theo xác nhận của Phạm Trần Anh.  

## Tổng hợp theo mã
| Mã | Loại lỗi | Số mục kiểm | Số lỗi | Mức |
| --- | --- | ---: | ---: | --- |
| QC1-01 tag camera | sai thuộc tính / bỏ sót | Chờ xác nhận | Chờ xác nhận | nặng |
| QC1-02 đủ L1, R1 | bỏ sót | Chờ xác nhận | 5 cảnh báo, chờ xác nhận lỗi | nặng |
| QC1-03 position | sai thuộc tính / thừa | Chờ xác nhận | Chờ xác nhận | nặng |
| QC1-04 tâm vạch, chiều, điểm dừng | sai phạm vi / bỏ sót | Chờ xác nhận | Chờ xác nhận | chính |
| QC1-05 vạch đứt, che | sai phạm vi / sai thuộc tính | Chờ xác nhận | Chờ xác nhận | chính |
| QC1-06 style, color, kind | sai thuộc tính | Chờ xác nhận | Chờ xác nhận | chính |
| QC1-07 vùng lái | sai phạm vi / bỏ sót / thừa | Chờ xác nhận | Chờ xác nhận | chính |
| QC1-08 đèn, màu | bỏ sót / sai phạm vi / sai thuộc tính | Chờ xác nhận | Chờ xác nhận | nặng / chính |
| QC1-09 facing, type, group, biển phụ | sai thuộc tính | Chờ xác nhận | Chờ xác nhận | chính |
| QC1-10 hình in, đủ biển | bỏ sót / sai phạm vi | Chờ xác nhận | Chờ xác nhận | chính |
| QC1-11 fisheye | sai phạm vi / sai thuộc tính | Chờ xác nhận | Chờ xác nhận | chính |
| QC1-12 file | lỗi file | 2 ZIP | 0 lỗi cấu trúc phát hiện | nhẹ / nặng |

## Danh sách lỗi (mỗi lỗi một dòng)
| # | Mã | Ảnh | Nhãn (label, id) | Mức | Mô tả ngắn |
| --- | --- | --- | --- | --- | --- |
| 1 | QC1-02 | A05 | lane, L1; không có ID vì nhãn đang bị báo thiếu | Nặng nếu xác nhận bỏ sót | Script báo thiếu L1; chờ người kiểm và coach xác nhận có vạch nhìn thấy cần gán |
| 2 | QC1-02 | A05 | lane, R1; không có ID vì nhãn đang bị báo thiếu | Nặng nếu xác nhận bỏ sót | Script báo thiếu R1; chờ người kiểm và coach xác nhận có vạch nhìn thấy cần gán |
| 3 | QC1-02 | A06 | lane, R1; không có ID vì nhãn đang bị báo thiếu | Nặng nếu xác nhận bỏ sót | Script báo thiếu R1; chờ người kiểm và coach xác nhận có vạch nhìn thấy cần gán |
| 4 | QC1-02 | A07 | lane, L1; không có ID vì nhãn đang bị báo thiếu | Nặng nếu xác nhận bỏ sót | Script báo thiếu L1; chờ người kiểm và coach xác nhận có vạch nhìn thấy cần gán |
| 5 | QC1-02 | A08 | lane, L1; không có ID vì nhãn đang bị báo thiếu | Nặng nếu xác nhận bỏ sót | Script báo thiếu L1; chờ người kiểm và coach xác nhận có vạch nhìn thấy cần gán |

## Ca mơ hồ
| Ảnh | Câu hỏi cho lead | Lời đáp (nếu có) |
| --- | --- | --- |
| A05 | Có thể xác nhận ảnh không thấy vạch sơn L1/R1 để ghi ngoại lệ? | Chờ xác nhận |
| A06 | Có vạch R1 nhìn thấy và thuộc phạm vi cần gán? | Chờ xác nhận |
| A07 | Bên trái có vạch L1 hay chỉ có mép dải phân cách? | Chờ xác nhận |
| A08 | Vạch L1 có đủ rõ để gán theo guideline? | Chờ xác nhận |

## Quyết định
Lỗi nặng: chờ xác nhận 5 cảnh báo   Lỗi chính: chờ xác nhận / chờ số nhãn đã kiểm = chưa tính %   Lỗi nhẹ: chờ xác nhận   Ca chờ lead: 4 ảnh  
Quyết định (Release / Hold / Rework): Hold tạm thời trong bản dự thảo, chờ Lê Đức Thanh xác nhận.  
Lý do (theo luật của phiếu): Còn ca mơ hồ thiếu L1/R1 cần lời đáp để kết luận. Nếu xác nhận có lỗi nặng thì áp dụng Rework. Kết quả lint hiện có 5 cảnh báo nặng, 0 chính, 0 nhẹ; fisheye có 0 cảnh báo. Số lỗi thực tế và tỷ lệ lỗi chính cần người kiểm đánh giá.  

Loại lỗi: bỏ sót = thiếu nhãn phải có; thừa = gán cái không phải đối tượng; sai phạm vi = hình lệch, sai chiều, dừng sai chỗ, tràn vùng. Ba loại này theo cách chia lỗi gán nhãn của ISO/IEC 5259-4 (mục 8.4.2); "sai thuộc tính" và "lỗi file" là khóa học thêm. Cách xếp mức: [thang mức lỗi](docs/qc_severity_road_v1.0.md).
