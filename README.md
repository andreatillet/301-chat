# BadgerBotGPT (and future CPA) - last updated Jan. 18, 2024

I am a GPT4-powered chat assistant to answer your questions about ACCT IS 301 at the Wisconsin School of Business. Ask me anything about your class. I am trained on your class syllabus, course schedule, and chapter summaries. I can help you study important course concepts and explain how to solve problems. Because I\'m AI, I don\'t need sleep, so I am here 24/7 to help you study for your class. Go Badgers! 😎

# Caveat Emptor
While AI chat assistants performing information retrieval from a knowledge base (known as retrieval augmented generation, or RAG) tend to perform more accurately, there's still a possibility of hallucination. That is, it will make stuff up. In addition to RAG using OpenAI's latest `gpt-4-1106-preview` model, I have also enabled OpenAI's code interpreter, which handles the calculations in its responses using Python. While I'm very excited about BadgerBotGPT's accuracy and performance in explaining accounting concepts and answering accounting questions/problems from the class, it's still just a language model...it's NOT a math model, NOT an accounting model. Just as you might be a bit skeptical about accounting advice from an English teacher, you should always verify BadgerBotGPT's responses with your course materials and syllabus. In cases where the Bot contradicts your course material, it should go without saying that your course material should be adhered to. If you encounter any egregious or unexpected errors, please let me know.

# Get started
To use BadgerBotGPT, you must use your own OpenAI API key to pay for your own usage. If you don\'t have an API key, go to [openai.com](openai.com) to create a new one ([here is a quick tutorial](https://youtu.be/UO_i1GhjElQ?si=7VvfWK8AXQG6vdcn)).

I would love nothing more than to find a rich benefactor to pay for the API costs related to running this app, but unfortunately I haven't found an accountingGPT sugar daddy yet, so we're stuck paying our own way here. However, OpenAI gives new users $5 in API credits for the first 90 days of an account (if you have an existing ChatGPT account, you might need to setup a new account to get the $5 credit) and the overall cost per user should be relatively inexpensive. This app uses the `gpt-4-1106-preview` model, which costs \$0.01/1K tokens for input and \$0.03/1K tokens for output (response). For reference, 1K tokens is equivalent to approximately 750 words. In addition to your prompt, the app will take as input its predefined instructions (~350 tokens) and any information it retrieves from its knowledge base (i.e., the class materials that I uploaded). To retain context, the app will also resubmit the entire conversation (i.e., thread), which increases the number of input tokens per prompt. You can reduce the number of input tokens by starting a new thread if the conversation gets too long--just click the "Start New Chat" button again. Learn more about [OpenAI's pricing here](https://openai.com/pricing). 

**Note:** Unlike the ChatGPT interface that you might be used to, this app does not retain your conversation history. Once you start a new chat or exit the page, your chats are gone forever, and there's no guarantee that it will ever reproduce the same response again. Therefore, if you find the information in your chats useful, consider copy-pasting the thread into your preferred text editor or note-taking app so that you can refer to it later.

## Prompting Advice for Students
- In general, you should be as specific as possible for the bot to respond with helpful answers.

- If it's having trouble recognizing your questions as part of the course content, start your prompt by asking it to refer to its knowledge base. 
    - For instance, "According to your notes, what is chapter 3 about?" or "According to your syllabus, what are Professor Tillet's office hours?"
- Ask it to refer to specific chapters
    - "According to Chapter 1, what are the objectives of financial reporting?"

- When asking it for help solving a specific problem, ask it to use step-by-step reasoning. For instance, you can copy-paste a question into the chat box then add the text "Explain your reasoning step-by-step" to the end of your prompt. It also helps to tell it what chapter the question comes from.
  The template that I have been using to ask it for help solving sample questions look something like this:

    > Here is an example problem from Chapter {N}. <br>
    > {PASTE problem text here} <br>
    > Please explain your reasoning step-by-step.

Note that for the example above, you might have to customize the problem from the class notes so that BadgerBotGPT has all the information it needs to solve the problem. In general, it will use fewer tokens (i.e., cost less) and provide better/more accurate responses if it doesn't have to guess on anything. That said, it could be a useful exercise for you to see how it reasons through problems with incomplete information.

- I don't know whether to say this first or last, but in general you should be polite to the AI. There's research shows kids who learn to speak with a voice assistant in their home, like Alexa or Google Assistant, grow up to be less polite to humans, in part because they grew up barking orders at a bot, without practicing how to say please or thank you. You will go on to correspond in writing in your professional lives and you don't want the way you communicate with AI to change the way you communicate with other humans. Also, just in case AI does ever become sentient, it's probably not bad for it to remember that you were one of the nice humans. 😂

## Known Issues:
- There might be issues with the sidebar loading properly when using Firefox. For now, switching to another browser should prevent this.
- The app interface looks strange and does not perform very well on an iPad or iPhone (based on my experimentation - any Android users out there want to give it a go?).
