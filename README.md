# SmolPC
SmolPC is a collection of AI powered apps that are suited for business users and travellers with Intel laptops. They may run on CPU, GPU and NPU and have distinct advantages for offline and privacy safe AI operations on useful Open Source projects. Created as part of an Industry Exchange Network (IXN) collaboration between UCL and Intel.

## Summer 2025

### AI Assistant for LibreOffice

**Author:** Ben Thompson  
**Contact:** [bthompsondev24@gmail.com](mailto:bthompsondev24@gmail.com)

The AI Assistant for LibreOffice app integrates local AI with LibreOffice Writer and Impress. It allows you to create and edit documents and presentations using a chat interface. You can simply send it a message and it will carry out your request. 

e.g. “Please create me a sales pitch presentation for the new Intel laptops”

The app also offers voice transcription using Whisper, allowing users to interact with the AI without typing. 
All AI models are run locally on-device, so it does not need an internet connection and keeps all data completely secure. It integrates an MCP Server which gives the AI direct access to LibreOffice functionality.

**Main Application:** [LibreOfficeAI](https://github.com/bthompson-dev/LibreOfficeAI)  
**MCP Server:** [libre-office-mcp](https://github.com/bthompson-dev/libre-office-mcp)

### AI Assistant for TextLocator

**Author:** Jinshuo Liu  
**Contact:** [liujinshuo3@gmail.com](mailto:liujinshuo3@gmail.com)

The AI Assistant for TextLocator integrates local AI into the open-source desktop search app [TextLocator](https://github.com/liulei901112/TextLocator) (WPF/.NET Framework). It lets you type a natural-language request, automatically extracts 3–5 core keywords on-device, and runs a classic Lucene search—so you can find files by meaning, not just exact terms.

e.g. “Find recent presentations about blockchain pilots with supply-chain traceability in the R&D folder”

The app also offers voice transcription via Whisper (OpenVINO), so you can speak instead of typing.
All models run fully offline on your PC (Granite for keywording, Distil-Whisper for ASR), keeping data private and usable without internet.

**Main Application:** [TextLocator AI Assistant](https://github.com/FierceWind1287/ai-textlocator)  (WPF UI, Lucene.Net + Jieba.NET)  
**Keyword Service:** KeywordService.exe (LlamaSharp + Granite 3.3 2B, local keyword extraction)  
**ASR Bridge:** WhisperBridge.dll (OpenVINO + Distil-Whisper, called via WhisperNative.cs)  

### AI Assistant for Excel

**Author:** Clara Cen  
**Contact:** claracenn@gmail.com  

The AI Assistant for Excel brings natural-language interaction directly into spreadsheets. Instead of navigating cells or recalling formulas, you can simply ask questions or request summaries, and the assistant will generate clear, contextual answers within Excel.  

The add-in also supports detailed explanations of financial formulas, voice input through integrated speech transcription, a history view for revisiting past queries, and adjustable verbosity modes for concise or in-depth answers. All processing runs locally, ensuring that the data remains private and accessible without an internet connection.  
  
**Main Appliation** [FinLite ExcelAddIn](https://github.com/claracenn/FinLite-ExcelAddIn)  
**MSI Installer**: [Download Here](https://liveuclac-my.sharepoint.com/my?id=%2Fpersonal%2Fucabbce%5Fucl%5Fac%5Fuk%2FDocuments%2Fsetup%2Ezip&parent=%2Fpersonal%2Fucabbce%5Fucl%5Fac%5Fuk%2FDocuments)  

*To install: unzip the archive and double-click `setup.msi`.*  

### AI Assistant for Generating Voiceover of Storybooks - ReadinTime (Voice) V1.5

**Author:** Jiawei Tan    
**Contact:** [jiaweitan531@gmail.com](mailto:jiaweitan531@gmail.com)

The AI Assistant to turn story text into audio, with customized voice narrative. It can run on CPU of Intel machine, offering personalized reading experience. This project is based on arBooks application of previous UCL computer science students (Pranay Vaka et al.)

**Main Application:** [ReadinTime (Voice) V1.5](https://github.com/Jack5316/ReadinTime-V1.5)        
**Zip-Folder:**[Zip-Folder](https://drive.google.com/file/d/1GHYxul1Gc1pv5ShVM1Gv2ZDf713Xo6q_/view?usp=sharing)


### AI Assistant for Texteditor

**Author:** Zihong Song

**Contact:** songzihong222@gmail.com

The AI Assistant for Texteidtor integrates local AI into the open-source desktop text editing app QOwnNotes (MFC Framework). It helps you editing text contents such as text summarizing, polishing, translating. You can also ask any related questions in terms of the fields the text contents involved. 
e.g. “summary the above deep learning article and explain what does the term segmentation mean? Can you give me an additional example of the segmentation”
The app also offers voice transcription via Distil-Whisper (OpenVINO), so you can speak instead of typing. All models run fully offline on your PC (Granite for dealing with the question asked by the users, keeping data private and usable without internet.
It also offers RAG（Retrieval-Augmented Generation）to improve the local interaction with the LLM model.

**Main Appliation:** [Local AI Assistant for TextEditor](https://github.com/szh123-ucl/Msc-Computer-Science-project-OSS-Pilots-AI-PC-app-and-source-code)(MFC)

**Zip-Folder:**[Download Here](https://github.com/szh123-ucl/Msc-Computer-Science-project-OSS-Pilots-AI-PC-app-and-source-code/releases)
