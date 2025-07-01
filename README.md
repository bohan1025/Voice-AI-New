# Voice-AI-New
User inputs via voice → Converts to text → GPT extracts information (name, phone number, real estate information) → Searches for real estate → Voice feedback (specific information about real estate) → Cloud storage information


Technique：
0. Front end (Including the app, the button which user click to speak)
1. Speech——recognition + Google API / Whisper （Convert what users said into text）
2.  Large Language model / GPT ai: Extract the key information from the generated text (Client name+Client phone number+property Address)
3. SQlite / Python: Search through database on any matched dataset, and give reponse to the client about the full information of the property via message & email & Voice (pyttsx3)
4. Updating all the client information on to the online database
