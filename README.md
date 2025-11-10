## How to access this website

The link to the website is: https://cf-ai-text-rewriter.eduardcojocaru2016.workers.dev/

## How to use the website

Using the website is very simple. All you have to do is enter some text that you want rewritten, select a tone then either press enter or the button to the right of the input bar and then you will get the output text.

## Project Report

For this project I decided to make an AI text rewriter where you simply enter the text that you want to rewrite, select the tone and then enter. Then the AI will rewrite the text with that tone in mind and output it in the chat section. 

I made this by firstly using the LLM Chat App template on Cloudflare where I then removed most of the frontend and replaced it with my own version which has the tones on the left that you can select and on the bottom you have the input bar. I also seperated the styling from the main HTML page for more readable code. I adapted the code to make it that you need both the tone and prompt before you can send the message. Then I expanded on the error detection logic where if the user doesn't enter a prompt or a tone, a message will appear to enter that. For the AI, I had to change the prompt many times as the AI would sometimes respond as if we are having a conversation and not rewrite the text.

## Project Structure

```
/
├── public/             # Static assets
│   ├── index.html      # Chat UI HTML
│   ├── style.css       # Chat UI CSS
│   └── chat.js         # Chat UI frontend script
├── src/
│   ├── index.ts        # Main Worker entry point
│   └── types.ts        # TypeScript type definitions
├── test/               # Test files
├── wrangler.jsonc      # Cloudflare Worker configuration
├── tsconfig.json       # TypeScript configuration
└── README.md           # This documentation
```