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
