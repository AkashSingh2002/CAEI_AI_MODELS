
### FOLDER GEMINI
###  Gemini LLM Application

#### Purpose:
The purpose of the Gemini LLM (Large Language Model) application is to provide a conversational interface for users to interact with Google's Generative AI model, specifically the Gemini model.

#### Components:
1. **Environment Configuration**: The application imports the `load_dotenv` function from the `dotenv` module to load environment variables from a `.env` file. This is commonly used to manage sensitive information such as API keys.
   
2. **Streamlit Setup**: Streamlit is imported as `st`, providing a framework for building interactive web applications in Python. The application sets the page configuration with a title "PDF Q&A" using `st.set_page_config`.
   
3. **Generative AI Configuration**: The application imports the `genai` module from `google.generativeai` and configures it with an API key obtained from the environment variable `GOOGLE_API_KEY`. This configuration allows the application to access and utilize the Generative AI model provided by Google.
   
4. **Generative Model Initialization**: An instance of the GenerativeModel class named `model` is created using the Gemini Pro model (`gemini-pro`) to generate content based on user input.
   
5. **User Interaction**: The application provides a text input field labeled "Input" where users can type their questions or input. It also includes a button labeled "ask question" to submit the input for processing.
   
6. **Response Handling**: When the user submits a question by clicking the "ask question" button, the application calls the `get_gemini_response` function with the input question. This function utilizes the GenerativeModel instance (`model`) to generate a response based on the input question.
   
7. **Displaying Response**: The generated response is then displayed to the user under the subheader "THE RESPONSE IS", allowing users to view the AI-generated content.

#### Usage:
Users can interact with the application by typing their questions or input into the text input field and clicking the "ask question" button to receive AI-generated responses.

#### Conclusion:
The Gemini LLM application provides a simple yet effective interface for users to engage with Google's Generative AI model, enabling them to ask questions and receive AI-generated responses in real-time. This application can be further enhanced with additional features and optimizations to improve user experience and functionality.

### How to Run
To run the application, ensure you have all the required libraries installed. Then, execute the script using the following command:

streamlit run gen_app.py

### Screenshots 


### Report on PDF Expert Application

#### Purpose:
The PDF Expert application is designed to provide users with tools for analyzing PDF documents. It offers functionality to summarize the content of PDF files and extract important text along with keywords.

#### Components:
1. **Environment Configuration**: The application imports the `load_dotenv` function from the `dotenv` module to load environment variables from a `.env` file. This allows for secure storage and retrieval of sensitive information such as API keys.
   
2. **Streamlit Setup**: Streamlit is imported as `st`, providing a framework for building interactive web applications in Python. The application sets the page configuration with a title "PDF EXPERT" using `st.set_page_config`.
   
3. **User Interface**: The application presents a header labeled "PDF Q&A" using `st.header`. It includes a text area for users to input text for analysis (`st.text_area`) and a file uploader (`st.file_uploader`) to upload PDF files for analysis.
   
4. **PDF Analysis Functions**: 
    - **Input PDF Setup**: The `input_pdf_setup` function processes the uploaded PDF file, converting it into image data that can be analyzed by the Generative AI model.
    - **Generative AI Response**: The `get_gemini_response` function utilizes the Generative AI model (`gemini-pro-vision`) to generate a response based on the provided input, PDF content, and a predefined prompt.
   
5. **User Interaction**: The application includes two buttons labeled "Summarize the pdf" and "Important text & keywords" (`st.button`) to trigger the analysis based on user input.
   
6. **Analysis Prompt**: A predefined input prompt is provided to guide the analysis process. It instructs the user to summarize the PDF content and highlight important points and keywords.
   
7. **Response Display**: The generated response from the Generative AI model is displayed under the subheader "the response is" using `st.subheader` and `st.write`.

#### Usage:
Users can interact with the PDF Expert application by providing text input in the designated area and uploading PDF files for analysis. They can then click the appropriate button to trigger the analysis process and view the generated response.

#### Conclusion:
The PDF Expert application offers a convenient solution for analyzing PDF documents, providing users with insights such as summaries and important keywords extracted from the content. It leverages Generative AI technology to enhance the analysis process and deliver meaningful results to users. Further improvements and enhancements could be made to enrich the functionality and usability of the application.

### How to Run
To run the application, ensure you have all the required libraries installed. Then, execute the script using the following command:

streamlit run chat_pdf.py