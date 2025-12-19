**Exam Fraud Detection Project**

**Overview**

This project presents an automated Exam Fraud Detection System designed to identify impersonation and fraudulent behavior in examination halls using computer vision and machine learning techniques. The system verifies a student’s identity by comparing facial images and textual information from multiple trusted sources, ensuring exam integrity with minimal human intervention.

The entire project is implemented and demonstrated using Google Colab, making it easy to reproduce and evaluate.

**Problem Statement**

Manual identity verification during exams is time-consuming, error-prone, and vulnerable to impersonation. Traditional methods such as physical ID checks do not scale well and can fail under high-volume examination environments.

This project aims to automate identity verification by:

      Detecting faces in real-time
      
      Extracting student details from exam documents
      
      Performing multi-level verification to detect mismatches and fraud

**Key Features**

            Face detection using Haar Cascade Classifier
            
            Text extraction using Optical Character Recognition (OCR)
            
            Multi-stage identity verification pipeline
            
            Automated fraud detection and alert mechanism
            
            Fully reproducible implementation in Google Colab


**System Workflow**

       Capture the live webcam image of the student   
       Detect faces using Haar Cascade  
       Extract student name and image from the hall ticket using OCR 
       Retrieve registered student data from the database 
       Perform the following validations:
       Live image vs Hall ticket image
       Live image vs Database image
       Hall ticket name vs Database name 
       Flag the student as Valid or Potential Fraud 
       Trigger an alert if discrepancies are found
        


**Technologies Used**

      Python
      
      OpenCV
      
      Haar Cascade Classifier
      
      Tesseract OCR
      
      NumPy
      
      Google Colab

**Project Structure**

Exam-Fraud-Detection/

│

├── notebooks/

│   └── exam_fraud_detection.ipynb

│

├── data/

│   ├── hall_ticket_images/

│   ├── database_images/

│   └── sample_webcam_images/

│

├── haarcascade/

│   └── haarcascade_frontalface_default.xml

│

├── README.md


**How to Run the Project**

      Open the notebook in Google Colab
      
      Upload required datasets (hall ticket images, database images)
      
      Run the notebook cells sequentially
      
      Allow webcam access when prompted
      
      Observe verification results and fraud alerts


**Results**

Successfully detects face mismatches and identity inconsistencies

Demonstrates real-world feasibility of automated exam monitoring

Highlights how layered verification improves fraud detection accuracy

Limitations and Future Improvements

Haar Cascade can struggle under poor lighting conditions

OCR accuracy depends on image quality

Can be extended using deep learning models like FaceNet or ArcFace

Real-time video stream integration and cloud deployment can improve scalability
