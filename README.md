# 🏥 Medical Document Automation with Google Cloud Document AI & BigQuery

Streamline medical insurance claim processing with advanced AI techniques, reducing manual efforts and improving efficiency with real-time analytics.

## 📚 Project Overview
This project leverages **Google Cloud Document AI** (Vertex AI and Generative AI) to automate the processing of medical insurance claim documents. By integrating **OCR** for digitization and **NLP** for content categorization, the system efficiently extracts structured data with high accuracy and integrates seamlessly with **BigQuery** for advanced data analysis.


## 🚀 Setup and Implementation

### 1. Create a Processor
- Navigate to the **Google Cloud Document AI** console.
- Create a custom processor for structured data extraction.
- Select the appropriate region and enable Google-managed storage and encryption.
![image](https://github.com/user-attachments/assets/ec20c736-af8f-4f5d-9219-12c3b76c8a62)


### 2. Processor Configuration
- **Field Definition**: Identify fields such as `claim_number`, `company_name`, `service_date`, `amount_billed`, `amount_paid`, and `medical_procedure`.
- **Field Attributes**: Define data types (e.g., Number, Date, Currency) and set occurrence parameters (Required, Optional).
<img width="1470" alt="Screenshot 2024-08-22 at 2 14 21 PM" src="https://github.com/user-attachments/assets/9aec788c-faec-4ade-960d-b9c3466525a7">


### 3. Document Labeling
- **Upload Documents**: Import PDFs into the labeling console from Google Cloud Storage.
- **Annotation**: Use built-in annotation tools to label fields. Leverage the foundation model for initial suggestions and manually correct any inaccuracies.
<img width="1470" alt="Screenshot 2024-08-22 at 2 18 20 PM" src="https://github.com/user-attachments/assets/8daf0ee6-bc89-4730-876a-e2749d1d22b0">
<img width="1470" alt="Screenshot 2024-08-22 at 2 18 28 PM" src="https://github.com/user-attachments/assets/b34ff4d8-d3e4-4509-ade7-34cce0f2369e">


### 4. Model Training
- **Build Processor Version**: Start with a pretrained foundation model and fine-tune it for medical document extraction.
- **Auto-Labeling**: Utilize **Generative AI** to automate the labeling process, ensuring efficient and accurate training data.
<img width="1470" alt="Screenshot 2024-08-22 at 2 14 26 PM" src="https://github.com/user-attachments/assets/f9aa6e67-979c-41a2-997b-7d1cb216774e">


### 5. Training Custom Model
- Ensure a balanced dataset with at least 10 examples per field.
- **Setup Training**: Configure and train a custom processor for optimal performance.
![image](https://github.com/user-attachments/assets/8ccd3554-88ec-470a-8630-75df0a3b380c)


### 6. Deployment
- Deploy the trained model for real-time processing.
- Manage processor versions for easy updates and scalability.
![image](https://github.com/user-attachments/assets/916f9448-1307-441b-88f5-76c3539b3afa)


### 7. Evaluation and Testing
- **Model Evaluation**: The model achieved a performance accuracy (96.1%), precision (95.5%), and recall (96.8%).
- **Document Testing**: Evaluate with new claim documents and make adjustments as necessary.
<img width="1470" alt="Screenshot 2024-08-22 at 2 14 33 PM" src="https://github.com/user-attachments/assets/f45b177d-e5eb-45a0-90fb-22f8d85eb207">


### 8. Integration with BigQuery
- Connect the **Document AI** output to **BigQuery** for comprehensive data analysis.
- Use **SQL queries** to extract insights and support data-driven decision-making.
<img width="1470" alt="Screenshot 2024-08-22 at 2 15 52 PM" src="https://github.com/user-attachments/assets/fbae5d22-e380-4844-87aa-7c6da4e494a3">
<img width="1470" alt="Screenshot 2024-08-22 at 2 20 43 PM" src="https://github.com/user-attachments/assets/1b740fce-4266-4783-872a-d18d59f84212">


## 🌟 Key Insights and Summary
- **Automated Document Processing**: Reduced manual data entry by 80%, achieving 96.1% accuracy in entity extraction.
- **NLP & OCR Integration**: Enhanced data digitization and content categorization for efficient handling.
- **Real-time Analytics**: Reduced processing time by 60%, providing instant insights.
- **Error Reduction**: Decreased processing errors by 75%, improving data reliability.
- **Scalable Solution**: Supports easy scaling for increased document volumes.
- **Generative AI Utilization**: Optimized training with automated labeling processes.

## 💻 Technology Stack
- **Google Cloud**: Document AI, Vertex AI, Generative AI
- **Data Processing**: OCR, NLP
- **Database**: BigQuery
- **Data Analytics**: SQL, AI/ML

## 📈 Impact
This project significantly improved the efficiency of processing medical insurance claims. It automated data entry, reduced errors, and enabled real-time analytics, making it a highly effective tool for healthcare data management.

---

Feel free to contribute, open issues, or suggest improvements to this project!
