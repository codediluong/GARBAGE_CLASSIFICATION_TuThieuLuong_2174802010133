# ♻️ Garbage Detection YOLOv11

Model phát hiện và phân loại rác sử dụng YOLOv11 (Ultralytics)

 Cài đặt

pip install ultralytics

## Tổng quan
Model có thể nhận diện 6 loại rác:
- BIODEGRADABLE (Rác hữu cơ)
- CARDBOARD (Giấy carton)
- GLASS (Thủy tinh)
- METAL (Kim loại)
- PAPER (Giấy)
- PLASTIC (Nhựa)

Ứng dụng:
- Phân loại rác tự động
- Smart city / môi trường
- AI camera nhận diện vật thể

---

##  Model
- Framework: Ultralytics YOLOv11
- Image size: 416x416
- Dataset: Roboflow (Object Detection)
- Classes: 6
Predict
yolo detect predict model=best.pt source=your_image.jpg
Train lại model
yolo detect train model=yolo11n.pt data=data.yaml epochs=50 imgsz=416
<img width="1418" height="715" alt="image" src="https://github.com/user-attachments/assets/7b576cb3-c0ea-4ebd-b7d5-d83058488921" />
<img width="1406" height="638" alt="image" src="https://github.com/user-attachments/assets/b2db1772-9746-4e0c-b648-80eb0efa14d5" />
<img width="1439" height="671" alt="image" src="https://github.com/user-attachments/assets/65f387cd-b2f8-4de8-8451-e19a13f94509" />
<img width="1203" height="654" alt="image" src="https://github.com/user-attachments/assets/75ce0e04-633e-4fb3-b1bd-b37419ea0ba6" />
<img width="1423" height="226" alt="image" src="https://github.com/user-attachments/assets/3624a912-82bc-4dba-9e1a-cfc169cfd89e" />
<img width="1445" height="405" alt="image" src="https://github.com/user-attachments/assets/2111b591-1172-4b8b-b7e9-b6058d86c891" />
!yolo detect predict model=/content/runs/detect/train/weights/best.pt source=/content/garbage_dataset/test/images save=True
<img width="1421" height="584" alt="image" src="https://github.com/user-attachments/assets/7b79b90c-95ab-4d96-94b3-bd3d9058b49d" />
<img width="1450" height="510" alt="image" src="https://github.com/user-attachments/assets/17d943c4-866b-4cee-b703-c690471dc4b7" />








---

