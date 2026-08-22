# Real-Time-Face-Mask-Detection
A Real-time face mask detection system using webcam and static image uploads. Detects if a person is wearing a mask, provides voice alerts, sends WhatsApp image alerts for violations, logs geotagged incidents, displays a heatmap of locations, and generates a compliance report of mask violations and adherence.
## 🔐 Login Page

![Login](images/Login.png)

## 🧭 Dashboard

![Dashboard](images/DashBoard.png) 

- 📸 Detects faces & identifies mask usage (Mask / No Mask)
- 🌐 Real-time webcam or static image detection
- 🔊 Voice feedback for compliance and Violations
- 📲 Sends **WhatsApp alerts** with face snapshots when violations occur
- 🗺️ Heatmap of violation locations based on GPS
- 📊 Tracks compliance & violations daily,weekly,monthly via dashboard

## 📸 Live web Cam Detection 

Real-time mask detection using webcam feed. 

![Live Detection](images/LiveWebDetection.gif)

## 📸 Static Image Detection

You can upload an image and the system will:

- Detect faces
- Identify if a mask is worn
- Display bounding boxes and confidence scores
- Log the result

![Static Detection](images/StaticUpload.png) 


## 🗺️ Geolocation & Heatmap Visualization 

Logged violations are shown on an interactive map based on their GPS coordinates. 

![GeoLoc](images/GeoTaggedLocation.png)  

Visualizes past violations on a location map using intensity colors.

- 🔴 Red = multiple violations
- 🟡 Yellow = few violations
- 🟢 Green = low/no violations

![HeatMap](images/HeatMap.png)

## 📱 WhatsApp  Alerts

- If a violation is detected:
  - WhatsApp image alert sent to registered number
  - All results shown on-screen with labeled bounding box

 ![WhatsappDashBoard](images/WhatsappAlertDB.png) 
 
![WhatsappDetection](images/WhatsappAlert.png) 

![WhatsappAlert](images/WhatsappAlertImg.png)


## 📢 Voice Alerts

- If a violation is detected:
  - 🔊 Voice message plays from dropdown selection
  - All results shown on-screen with labeled bounding box

![VoiceDB](images/VoiceAlertDb.png) 

![Voice1](images/VoiceAlert_Mask.png) 

![Voice2](images/VoiceAlert_NoMask.png)


## 📊 Compliance Tracker

Automatically logs all events:
- Date, time, mask status, confidence, GPS
- Counts violations vs compliance

![Compliance Report](images/ComplianceReport.png)

## 🧠 Model Details
- Face Detection: OpenCV SSD with Caffe model
- Mask Classification: Trained with ResNet50V2 / MobileNetV2
- Image Size: 224x224 RGB
- Framework: TensorFlow + Keras

