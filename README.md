# 🌟 **Named Entity Recognition (NER) Application**

This Flask-based web application allows users to categorize and tag named entities in any text input. It includes user authentication and a text entry page where users can input text and receive categorized entity recognition results.


## **Features:**
- 🔒 **User Authentication**: Secure login and registration system.
- 🧠 **Text Analysis**: Integration with the Edinai API for Named Entity Recognition (NER).
- ✨ **Automatic Tagging**: Categorizes and tags named entities such as organizations, locations, and people in the input text.

## **How to Use:**
1. 📝 **Register/Login**: Create an account or log in securely.


    ![Login Page](https://private-user-images.githubusercontent.com/112764699/347789819-d7921c48-951f-4df6-8598-3ca0691d7b6e.png?jwt=eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpc3MiOiJnaXRodWIuY29tIiwiYXVkIjoicmF3LmdpdGh1YnVzZXJjb250ZW50LmNvbSIsImtleSI6ImtleTUiLCJleHAiOjE3MjA2OTU3MzIsIm5iZiI6MTcyMDY5NTQzMiwicGF0aCI6Ii8xMTI3NjQ2OTkvMzQ3Nzg5ODE5LWQ3OTIxYzQ4LTk1MWYtNGRmNi04NTk4LTNjYTA2OTFkN2I2ZS5wbmc_WC1BbXotQWxnb3JpdGhtPUFXUzQtSE1BQy1TSEEyNTYmWC1BbXotQ3JlZGVudGlhbD1BS0lBVkNPRFlMU0E1M1BRSzRaQSUyRjIwMjQwNzExJTJGdXMtZWFzdC0xJTJGczMlMkZhd3M0X3JlcXVlc3QmWC1BbXotRGF0ZT0yMDI0MDcxMVQxMDU3MTJaJlgtQW16LUV4cGlyZXM9MzAwJlgtQW16LVNpZ25hdHVyZT03NzdjNjI0NzZiNzMwODFlYzUzZWE3MDhkMzljZWFlMWExZGYxMjcxOGNjODBjMzA5NzFjMTYyNDZhNDBmOGMxJlgtQW16LVNpZ25lZEhlYWRlcnM9aG9zdCZhY3Rvcl9pZD0wJmtleV9pZD0wJnJlcG9faWQ9MCJ9.AZe9YDnJ-FcyBR0zJ8T9718U-pIZLrOqycRheirIrBw)
   ![Register/Login Page](https://private-user-images.githubusercontent.com/112764699/347789791-a23c32d5-a6a2-4755-97db-0f3b9d311619.png?jwt=eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpc3MiOiJnaXRodWIuY29tIiwiYXVkIjoicmF3LmdpdGh1YnVzZXJjb250ZW50LmNvbSIsImtleSI6ImtleTUiLCJleHAiOjE3MjA2OTU3MzIsIm5iZiI6MTcyMDY5NTQzMiwicGF0aCI6Ii8xMTI3NjQ2OTkvMzQ3Nzg5NzkxLWEyM2MzMmQ1LWE2YTItNDc1NS05N2RiLTBmM2I5ZDMxMTYxOS5wbmc_WC1BbXotQWxnb3JpdGhtPUFXUzQtSE1BQy1TSEEyNTYmWC1BbXotQ3JlZGVudGlhbD1BS0lBVkNPRFlMU0E1M1BRSzRaQSUyRjIwMjQwNzExJTJGdXMtZWFzdC0xJTJGczMlMkZhd3M0X3JlcXVlc3QmWC1BbXotRGF0ZT0yMDI0MDcxMVQxMDU3MTJaJlgtQW16LUV4cGlyZXM9MzAwJlgtQW16LVNpZ25hdHVyZT00YWJjYzRmODZkZWM1YjlkZDM3MDE0OWI0ODY0MjBkYzUxZDk5MWFiMTY3ZDY1YmJkZmQ5Yjg4ZjFiZDU0MDg4JlgtQW16LVNpZ25lZEhlYWRlcnM9aG9zdCZhY3Rvcl9pZD0wJmtleV9pZD0wJnJlcG9faWQ9MCJ9.hiQUFJuIQwaq7GannShGD_-Reltk3t-36uxolv6DtJ8) <!-- Replace with your register/login page image path -->
3. 💬 **Enter Your Text**: Navigate to the text entry page and input your text.

   ![Text Entry Page](https://private-user-images.githubusercontent.com/112764699/347789806-7d1e8dd8-b1a8-432c-adf2-860c2877ace5.png?jwt=eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpc3MiOiJnaXRodWIuY29tIiwiYXVkIjoicmF3LmdpdGh1YnVzZXJjb250ZW50LmNvbSIsImtleSI6ImtleTUiLCJleHAiOjE3MjA2OTU3MzIsIm5iZiI6MTcyMDY5NTQzMiwicGF0aCI6Ii8xMTI3NjQ2OTkvMzQ3Nzg5ODA2LTdkMWU4ZGQ4LWIxYTgtNDMyYy1hZGYyLTg2MGMyODc3YWNlNS5wbmc_WC1BbXotQWxnb3JpdGhtPUFXUzQtSE1BQy1TSEEyNTYmWC1BbXotQ3JlZGVudGlhbD1BS0lBVkNPRFlMU0E1M1BRSzRaQSUyRjIwMjQwNzExJTJGdXMtZWFzdC0xJTJGczMlMkZhd3M0X3JlcXVlc3QmWC1BbXotRGF0ZT0yMDI0MDcxMVQxMDU3MTJaJlgtQW16LUV4cGlyZXM9MzAwJlgtQW16LVNpZ25hdHVyZT0yMWYzMDRlMmZmZjE1MjEzODRmZTIxNmNkNzY1ZDExMWJlMGE1ZGNhMTgzODBkMWI1ZWRkYWE4MjhjODgxYjNkJlgtQW16LVNpZ25lZEhlYWRlcnM9aG9zdCZhY3Rvcl9pZD0wJmtleV9pZD0wJnJlcG9faWQ9MCJ9.JmgkV8D5iaNeMD2imaEBw26odfkatkHbLRBDVBspaKw) <!-- Replace with your text entry page image path -->
5. 🔍 **Analyze Text**: Click on the "Perform NER" button to automatically categorize and tag named entities.

6. 📄 **View Results**: See the results with categorized named entities highlighted.

   ![Results Page](https://private-user-images.githubusercontent.com/112764699/347789806-7d1e8dd8-b1a8-432c-adf2-860c2877ace5.png?jwt=eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpc3MiOiJnaXRodWIuY29tIiwiYXVkIjoicmF3LmdpdGh1YnVzZXJjb250ZW50LmNvbSIsImtleSI6ImtleTUiLCJleHAiOjE3MjA2OTU3MzIsIm5iZiI6MTcyMDY5NTQzMiwicGF0aCI6Ii8xMTI3NjQ2OTkvMzQ3Nzg5ODA2LTdkMWU4ZGQ4LWIxYTgtNDMyYy1hZGYyLTg2MGMyODc3YWNlNS5wbmc_WC1BbXotQWxnb3JpdGhtPUFXUzQtSE1BQy1TSEEyNTYmWC1BbXotQ3JlZGVudGlhbD1BS0lBVkNPRFlMU0E1M1BRSzRaQSUyRjIwMjQwNzExJTJGdXMtZWFzdC0xJTJGczMlMkZhd3M0X3JlcXVlc3QmWC1BbXotRGF0ZT0yMDI0MDcxMVQxMDU3MTJaJlgtQW16LUV4cGlyZXM9MzAwJlgtQW16LVNpZ25hdHVyZT0yMWYzMDRlMmZmZjE1MjEzODRmZTIxNmNkNzY1ZDExMWJlMGE1ZGNhMTgzODBkMWI1ZWRkYWE4MjhjODgxYjNkJlgtQW16LVNpZ25lZEhlYWRlcnM9aG9zdCZhY3Rvcl9pZD0wJmtleV9pZD0wJnJlcG9faWQ9MCJ9.JmgkV8D5iaNeMD2imaEBw26odfkatkHbLRBDVBspaKw) <!-- Replace with your results page image path -->

## **Setup:**
To run the application locally:

1. 📂 Clone the repository.
2. 📦 Install dependencies: `pip install -r requirements.txt`
3. 🔧 Set up environment variables for API keys and Flask configuration.
4. ▶️ Run the application: `python app.py`
5. 🌐 Access the application at `http://127.0.0.1:5000/`
![Access the webpage from](https://private-user-images.githubusercontent.com/112764699/347792437-c237b484-9a84-458e-8240-5d32d243d9ea.png?jwt=eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpc3MiOiJnaXRodWIuY29tIiwiYXVkIjoicmF3LmdpdGh1YnVzZXJjb250ZW50LmNvbSIsImtleSI6ImtleTUiLCJleHAiOjE3MjA2OTYxMjAsIm5iZiI6MTcyMDY5NTgyMCwicGF0aCI6Ii8xMTI3NjQ2OTkvMzQ3NzkyNDM3LWMyMzdiNDg0LTlhODQtNDU4ZS04MjQwLTVkMzJkMjQzZDllYS5wbmc_WC1BbXotQWxnb3JpdGhtPUFXUzQtSE1BQy1TSEEyNTYmWC1BbXotQ3JlZGVudGlhbD1BS0lBVkNPRFlMU0E1M1BRSzRaQSUyRjIwMjQwNzExJTJGdXMtZWFzdC0xJTJGczMlMkZhd3M0X3JlcXVlc3QmWC1BbXotRGF0ZT0yMDI0MDcxMVQxMTAzNDBaJlgtQW16LUV4cGlyZXM9MzAwJlgtQW16LVNpZ25hdHVyZT1lMjc5ZmJkOGFkM2ExNGJhYzc4NzMxOTQ3ODNlOWFkNGJhZTcwNzQ2YTczNjZjMGE3ZDc2YzMwZmI0MTk3NDVhJlgtQW16LVNpZ25lZEhlYWRlcnM9aG9zdCZhY3Rvcl9pZD0wJmtleV9pZD0wJnJlcG9faWQ9MCJ9.eR7ZC5YTEsU_JxTwq2EV4eHf2_2nnp0ZB3Md48hHqME)

## **Technologies Used:**
- 🖥️ Flask
- 🐍 Python
- 🔗 Edinai API for Named Entity Recognition

## **Contributing:**
Contributions are welcome! Fork the repository and submit a pull request with your improvements.

## **License:**
This project is licensed under the MIT License - see the LICENSE file for details.
