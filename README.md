# Voice-AI-New

User inputs via voice → Converts to text → GPT extracts information (name, phone number, real estate information) → Searches for real estate → Voice feedback (specific information about real estate) → Cloud storage information

AI's mission
Hi how can I help you?
2. Can i have your name again? (Get data)
3. Can I get your phone number? (Get data)
4. Can I get the address? (Get data,sending out the address)
5. Thank you have a good day
6. Gather and push the data onto the cloud database




Front End and BAck End Are can contribute seperate -> build connections

Technique：
0. Front end (Including the app, the button which user click to speak) 和客户的实时互动 -> 然后用API链接将客户讲的东西 语音转文本
Button website -> sending information to backend (flask) Azure docker container apps 
1. Speech——recognition + Google API / Whisper （Convert what users said into text） 语音转文本 这个也是要用API交互的 (Speech services with the Azure ) speech services
2.  Large Language model / GPT ai: Extract the key information from the generated text (Client name+Client phone number+property Address) 转文本之后提取关键信息 (Azure open AI based Chatgpt)
3. Interact with the client and sending out the property information  （这里需要转换变回语音信息 连接到backend）
4. Updating all the client information on to the online database 上传关键信息到Azure SQL database / Azure Table



Important library:
pip install openai-whisper


要实现用户交互 （比如用户如何实现说话交互）+在交互的时候实时语音转文本 然后提取关键信息 + push data到数据库



Conpare:
cost
performance（speed and latency）
<<<<<<< HEAD



前端 (index.html) 
    ↓ (音频文件)
后端 API (voice_bot_backend.py)
    ↓
1. 音频转文本 (Whisper)
    ↓
2. 信息提取 (OpenAI GPT-3.5)
    ↓
3. 房产信息查询 (SQLite)
    ↓
4. 生成回复文本
    ↓
5. 文本转语音 (pyttsx3)
    ↓
6. 保存到数据库
    ↓
返回结果给前端
=======
Memory Storage
>>>>>>> 5dee65e2d9dd3cab315e8cc383ee9ce107349008
