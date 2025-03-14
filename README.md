# titan-AI
data analyses at your finger tip
"I want to create an AI-powered data analysis tool called 'Titan AI,' inspired by Julius AI, with a strong emphasis on a user-friendly chat-based UI. Titan AI should allow users to upload structured data (e.g., Excel, CSV, Google Sheets, or database files), analyze it, generate visualizations, perform advanced statistical modeling, and provide insights—all through a conversational interface. Below are the requirements, with a detailed UI specification:

Core Features:
Data Upload and Parsing: Support uploading and parsing CSV, Excel (.xls, .xlsx), Google Sheets (via API), and optionally PostgreSQL database connections. Detect file structure (headers, multi-tab spreadsheets) and store data for analysis.
Natural Language Processing (NLP): Interpret plain English queries (e.g., 'What’s the average sales by region?' or 'Plot revenue trends over time') and map them to data analysis or visualization tasks.
Data Analysis: Perform descriptive statistics (mean, median, etc.) and advanced analyses (regression, forecasting, clustering) using pandas, NumPy, scikit-learn, and statsmodels.
Visualization: Generate charts (bar, line, histogram, scatter) using Matplotlib, Seaborn, or Plotly, with downloadable outputs (PNG, SVG).
Export Capabilities: Export results (tables, charts) as CSV, Excel, or PNG.
Technical Requirements:
Backend: Use Python with Flask or FastAPI for the server, handling file uploads, query processing, and analysis.
Frontend: Build a responsive, chat-based UI using HTML, CSS, and JavaScript (preferably with React for dynamic updates, but plain JS is fine if simpler).
NLP Backend: Use a pre-trained model (e.g., Hugging Face Transformers) or a rule-based system to process queries.
Dependencies: Include pandas, NumPy, scikit-learn, Matplotlib, Seaborn, Plotly, openpyxl, and Flask/FastAPI libraries.
File Structure: Modular design with data_parser.py, analysis_engine.py, visualization.py, nlp_processor.py, app.py, and a frontend/ folder.
UI Specification:
Design Goals: Clean, modern, intuitive, resembling a messaging app (e.g., WhatsApp or Slack) with a focus on data interaction.
Components:
Header: A fixed top bar with the title 'Titan AI' and a tagline (e.g., 'Your Personal Data Analyst').
Chat Window: A scrollable central area displaying the conversation:
User messages appear on the right (blue bubbles).
Titan AI responses appear on the left (gray bubbles), including text, tables, or embedded visualizations.
Visualizations (e.g., charts) are rendered inline with a 'Download' button below each.
Input Area: A bottom section with:
A file upload button (drag-and-drop support for CSV/Excel files).
A text input field for typing queries (e.g., 'Show me a pie chart of sales by product').
A 'Send' button to submit queries.
Status Bar: A small area below the input showing upload progress (e.g., 'Processing file...') or analysis status (e.g., 'Generating chart...').
Styling:
Use a light theme with a sans-serif font (e.g., Roboto or Arial).
Responsive design: Works on desktop and mobile (chat window adjusts to screen size).
Smooth animations for message loading (e.g., fade-in effect for Titan AI responses).
Interactivity:
Clicking a visualization opens a larger view in a modal window.
Real-time feedback: Typing in the input field triggers a subtle 'Titan AI is typing...' indicator in the chat window.
Error messages (e.g., 'Invalid file format') appear as red-text bubbles in the chat.
Example Workflow:
User drags a CSV file (columns: Date, Region, Sales) into the upload area.
Chat shows: 'User: Uploaded sales_data.csv' and 'Titan AI: File processed successfully. Ask me anything!'
User types: 'Plot sales trends by region.'
Titan AI responds with a line plot (embedded in the chat) and a 'Download PNG' button.
Stretch Goals:
Add a dark mode toggle in the header.
Support live previews of uploaded data (e.g., a table preview before querying).
Implement voice input for queries using the Web Speech API.
Project Deliverables:
Scaffold a project with:
app.py: Flask/FastAPI server with endpoints for file uploads and query processing.
frontend/index.html: Chat UI structure.
frontend/style.css: Styling for the UI.
frontend/script.js: JavaScript for handling user input, file uploads, and displaying responses.
Supporting Python files (data_parser.py, etc.).
Sample code for integrating backend and frontend (e.g., AJAX calls to the server).
A requirements.txt file and setup instructions.
Start by generating the frontend/index.html, style.css, and script.js files for the UI, then build the app.py server to connect it. Name the tool 'Titan AI' consistently. Guide me step-by-step after each component is created.
