A PYTORCH CHAT BOT 

 

Project Summary: AI Chatbot using PyTorch and Bag-of-Words 

Overview: 

Built an intent-based AI chatbot from scratch using PyTorch and NLP techniques. The chatbot understands and responds to user queries by predicting intent categories trained on a custom intents.json file. 

 Key Features: 

Conversational Interface via terminal and web (Gradio) 

Intent Recognition using a neural network trained on tokenized sentence patterns 

Bag-of-Words Encoding for text vectorization 

Fully Trained Model using CrossEntropyLoss and Adam optimizer 

Interactive Web UI built using Gradio with support for real-time chatting and “quit” to auto-close 

 Technical Stack: 

Language: Python 

Libraries: PyTorch, NumPy, NLTK, Gradio 

ML Model: Feedforward Neural Network 

Training Technique: Supervised learning on stemmed, tokenized inputs with intent tags 

Data: Custom intents.json containing tags, patterns, and responses 

 Workflow: 

Data Preparation 

Loaded and parsed intents.json → tokenized and stemmed patterns → encoded into Bag-of-Words vectors. 

Model Building & Training 

Defined a simple neural network (input → hidden → output) 

Trained on intent-tagged patterns using CrossEntropyLoss 

Saved model with torch.save for future inference 

Chatbot Deployment 

Built interactive command-line chat loop 

Upgraded to a web-based interface using Gradio’s ChatInterface 

Added a quit trigger to auto-close the chatbot session 

 Sample Intents: 

Greeting: “Hi”, “Hello”, “Hey” 

Goodbye: “Bye”, “See you later” 

PlayMusic: “Play a song”, “Start music” 

Thanks: “Thank you”, “Thanks” 

 Output: 

The chatbot responds with relevant replies based on intent 

Rejects unknown queries with a fallback message 

Accessible via localhost or public shareable Gradio link 
