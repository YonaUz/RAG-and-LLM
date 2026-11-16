/!\ README is under construction /!\

Generative modelling allows us to provide data that is similar to and inspired from existing data. In RAG and LLM, the existing data are texts. But text data nowadays exist under multiple forms, and file types (pdf, websites, code files like html, css, Python, Javascript...), and across thousands of subjects. The subject here chosen is Remote Sensing, and more particularly Sentinel 2 and Landsat 8 and 9 satellites. _Why this subject ?_ For many reasons, firstly to get started with one interesting subject, secondly because I started learning about them at work, and because it reveals traps and tricky questions to think about. 
Ready to start ? Welcome to the adventure! 

Generative modelling is based on observation: in language models, one observation may be that some words are usually associated to another; "Queen" goes to "She" while "King" goes to "He"; "The cat eats the mouse" or "The mouse is eaten by the cat", but rarely inverse. In image modelling, cars are located in the street and the sea is blue, while rarely pedestrians smile under the rain...  And so on the generated image will be, based on the probabilistic observed text or image. 


Notebooks are numerated, to follow a logic.

0. First start with `00_framing_and_fundamentals.ipynb` which details the subject and scope of the project. We will deal with Sentinel 2, Landsat 8 and 9 satellites, and read/ learn about Satellite missions, Sensors, Spectral bands, Spatial resolution, Spectral resolution, Temporal resolution, Spectral indices, Remote sensing applications, Data products and Processing methods. 
1. Notebook `01_document_ingestion.ipynb` defines and creates the folders needed for the project, distinguishing the raw documents from the processed files. The raw docs are Sentinel 2 and Landsat 8 and 9 data sheets. We use Langchain framework to load the files with PyPDFLoader library for PDF files. It allows reading the file, preview it and extract metadata. The processed files are those files stored in a JSONL file. To avoid having to reread and reload all the PDFs at each execution, we save the ingestion result in JSONL format in the processed subfolder. JSONL means JSON Lines: each line is an independent JSON object and contains a page loaded text with its metadata. 
2. 

# RAG-and-LLM
RAG and LLM comparison 
A Large Language Model (LLM) is built from thousand of multi-source information, and is up to date until the date is has been released, so it may create hallucinations, invente information. On the other side,  for some general information, a LLM can be really powerful and enough. It depends of the context and the accuracy needed. An interesting option for continuing with LLM with some accurate and tricky information is to provide access to some documentation and prohibit it to go ahead from the documentation provided. Another interesting tool is the RAG, Retrieval-Augmented Generation. 


