# Machine Learning-Based Promotion Finder for E-commerce Websites

## Project Overview
This project aims to design a system that automatically detects promotions and offers from e-commerce websites using machine learning models. The system extracts promotional content such as banners, pop-ups, and text from selected e-commerce sites and classifies them to identify valid promotions.

## Project Phases

### Phase 1: Data Collection
- **Target Websites:**  
  - [Amazon](https://www.amazon.com/)  
  - [Flipkart](https://www.flipkart.com/)  
  - [Walmart](https://www.walmart.com/)
  
- **Tools Used:**  
  - Web scraping tools such as Selenium and Beautiful Soup.
  
- **Data Extracted:**  
  - Page content (HTML and visible text).  
  - Image links (banner images).  
  - Focused data includes:  
    - Titles, subtitles, descriptions  
    - Pop-up or banner text  
    - Button labels like "Get Offer", "Shop Now"

- **Deliverable:**  
  - A raw dataset containing website text and images.

### Phase 2: Dataset Labelling
- Manually label the scraped data with the following categories:  
  - **Promotion**  
  - **Non-Promotion**
  
- **Example labels:**  
  - `"Up to 50% off"` → Promotion  
  - `"New Arrivals"` → Non-Promotion (unless linked to an offer)
  
- **Deliverable:**  
  - A labelled dataset in CSV or JSON format for training the model.

### Phase 3: Model Development

1. **Text-based Promotion Classifier**  
   - Machine learning model that classifies text blocks from the web pages as promotion or non-promotion.
   
- **Deliverable:**  
  - A trained ML model capable of accurately classifying promotions.

## Technologies & Libraries Used
- Python  
- Selenium  
- Beautiful Soup  
- Scikit-learn / TensorFlow / PyTorch (for ML models)  



