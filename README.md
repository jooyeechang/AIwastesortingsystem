Eco-Assistant ♻️
Eco-Assistant is an AI-powered waste management and recycling assistant. This web app allows users to ask questions about recycling and waste sorting or upload images of waste materials for analysis. The app provides information about the recyclability of materials and gives suggestions on how to manage different types of waste, including pricing details for materials in MYR (Malaysian Ringgit) based on market prices.

Table of Contents
Features
Installation
Usage
Technologies
API Setup
File Upload Support
Location-Based Recycling Centers
Quick Suggestions
Contributing
License
Features
Text-Based Inquiry: Users can ask waste management and recycling-related questions directly.
Image Analysis: Upload an image of waste material and receive recommendations for recycling, reusing, and categorization.
Recycling Center Lookup: Find nearby recycling centers based on your location input.
Material Market Prices: Display current market prices in MYR for materials such as plastics, metals, and aluminum detected in uploaded images.
Quick Suggestions: Ready-made queries to get information about common recycling topics like plastic, electronic waste, and food waste.
Installation
Clone the repository:

bash
Copy code
git clone https://github.com/your-repo/eco-assistant.git
cd eco-assistant
Install the required packages:

bash
Copy code
pip install -r requirements.txt
Set up environment variables: Create a .env file in the root of the project and add the following variables:

makefile
Copy code
Gemini_API=your_gemini_api_key
OpenAI_Api_Key=your_openai_api_key
Usage
Run the Streamlit app:

bash
Copy code
streamlit run app.py
Interact with the app:

Type your waste management questions in the chat input or upload an image of waste material.
Use the sidebar to get recycling center recommendations based on your location or try one of the quick suggestions.
Technologies
Streamlit: A framework for building interactive web applications in Python.
Google Generative AI (Gemini): For generating responses to waste management queries and processing image uploads.
OpenAI API (ChatGPT): To fetch real-time information about nearby recycling centers.
Python: Backend logic.
Environment Variables: For API key management.
API Setup
Google Generative AI (Gemini)
To use Gemini's model for content generation, follow these steps:

Sign up for Google Generative AI and get your API key.
Set up your environment variable:
bash
Copy code
export Gemini_API=your_gemini_api_key
OpenAI API
For location-based recycling center lookups, configure your OpenAI API key:

Sign up at OpenAI and generate an API key.
Add the OpenAI API key to your environment:
bash
Copy code
export OpenAI_Api_Key=your_openai_api_key
File Upload Support
Users can upload .png, .jpg, and .jpeg files to receive recommendations on recycling based on image content.
The app uses Google Generative AI (Gemini) to analyze the images and provide feedback on recyclability, categorization, and pricing.
Location-Based Recycling Centers
The app can suggest nearby recycling centers based on a city, state, and postcode entered by the user.
Powered by OpenAI for real-time lookup, ensuring that users receive the most accurate and up-to-date information.
Quick Suggestions
The sidebar contains buttons for quick inquiries:
How do I recycle plastics?
How to dispose of electronic waste?
How can I reduce food waste at home?
These quick questions allow users to receive information on common recycling topics instantly.

Contributing
Contributions to the project are welcome. To contribute:

Fork the project.
Create a new feature branch: git checkout -b feature-name.
Commit your changes: git commit -m 'Add some feature'.
Push to the branch: git push origin feature-name.
Open a pull request.
License
This project is licensed under the MIT License. See the LICENSE file for more details.
