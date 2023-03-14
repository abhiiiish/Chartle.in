
# whatsapp-gpt

This is a Whatsapp chatbot that allows users to easily use AI services from Whatsapp. The motivation behind creating this bot was to provide an alternative way to access Chat-GPT instead of using official site. 

With Whatsapp GPT Bot, users can seamlessly communicate with the bot using natural language processing techniques to generate responses through the use of various AI models integrated with it, such as Whisper, DALL-E, and ChatGPT. Additionally, the bot provides text formatting features, accepts reviews on generated descriptions, and supports image generation abilities using DALL-E. 


## Dependencies

The following dependencies are required to run this project:

- Node.js (v14.17.3 or later)
- FFmpeg
- Puppeteer

To install Node.js, visit the official website [here](https://nodejs.org/en/), and download the latest version for your operating system.

To install FFmpeg, visit the official website [here](https://ffmpeg.org/), and follow the instructions for your operating system.

## Installation
To use the Whatsapp GPT Bot, you'll need to clone this repo and install the required dependencies. You'll also need to provide your own API keys for the AI models used in the bot.

```shell
git clone https://github.com/SabirKhanek/whatsapp-gpt.git
npm install
```


### Environment Variables

You need these environment variables for the working of the bot.

`openai_key`

Create a `.env` file in the root directory of the project and add the following line to it, replacing `YOUR_OPENAI_API_KEY` with your actual API key:

``` 
openai_key=YOUR_OPENAI_API_KEY
```

### Starting the bot
After installing dependencies and setting up environment variables run:

```shell
node index.js
```

Note: The chatbot is designed to run on a server, so you may need to deploy it to a cloud service or setup your own server to run the bot 24/7. You can use [heroku](https://heroku.com) or [render](https://render.com). On heroku you may have to install buildpack for puppeteer, However Render comes with puppeteer and ffmpeg support. 



To generate images with DALL-E you can write command as:
```whatsapp-gpt
Generate an image of beautiful landscape. A mountain and a river.
```


### Commands
The following commands are available:

- `%%clear` - Clear the chat history
- `%%help` - Display information about available commands

## Example
KEEP IN MIND to not to send any personal information as the backend is using whatsapp web on headless browser, Your conversation is maybe accessible to the author

## Contribution
If you'd like to contribute to this project, please fork the repository and submit a pull request. 
