Multi-Agent Product Comparison Bot 
This project is a web-based application that uses a team of specialized AI 
agents to generate detailed and insightful comparisons between any two 
products. The application is built with Python, Gradio, and the Google 
Generative AI API. 
Features 
• Detailed Comparisons: Get a full report including a side-by-side 
specification table, pros and cons for each product, and a final verdict. 
• AI-Powered: Utilizes the powerful Gemini 2.5 Pro model to provide 
accurate and up-to-date information. 
• Multi-Agent System: A sophisticated architecture where different agents 
collaborate to gather, analyze, and present the information, ensuring a 
high-quality report. 
• User-Friendly Interface: A simple and clean web UI built with Gradio, 
making it easy for anyone to use. 
• Loading Animation: A progress indicator shows that the report is being 
generated, improving the user experience. 
How It Works 
The bot uses a multi-agent system to handle user requests. Instead of a single 
AI trying to do everything, the task is broken down into a sequence of steps, 
each handled by a specialized agent: 
1. Info Extractor Agent : This agent's only job is to gather the raw 
specifications for each product. It is called once for Product A and once 
for Product B. 
2. Comparator Agent : This agent takes the raw data from the first agent 
and organizes it into a structured format. It creates the comparison table 
and the pros/cons lists. 
3. Recommender Agent : The final agent analyzes the structured 
comparison and provides a "Final Verdict," recommending one product 
over the other for a specific type of user. 
This separation of tasks makes the final report more reliable, structured, and 
accurate. 
Setup and Usage 
This project is designed to be run easily in a Google Colab notebook. 
Requirements 
You will need to install the following Python libraries: 
• gradio 
• google-generativeai 
Step-by-Step Instructions 
1. Install the Libraries Open a new cell in your Colab notebook and run the 
following command to install the required packages: 
2. !pip install -q -U gradio google-generativeai 
3. Set Up Your API Key This project requires a Google Generative AI API key. 
You must store it securely using Colab's "Secrets" feature. 
o In your Colab notebook, click the key icon ( ) on the left sidebar. 
o Click "Add a new secret". 
o For the Name, enter GEMINI_API_KEY. 
o In the Value field, paste your actual Gemini API key. 
o Make sure the "Notebook access" toggle is turned on. 
4. Run the Code 
o Copy the entire Python script (your_script_name.py) into a new 
cell in your Colab notebook. 
o Run the cell. 
5. Access the Application After running the script, a public URL will be 
generated in the output. Click on this URL to open the Gradio web 
interface in your browser and start comparing products! 
Technologies Used 
• Python: The core programming language. 
• Gradio: For creating the interactive web UI. 
• Google Generative AI: For the core AI and language model capabilities 
(Gemini 2.5 Pro). 
