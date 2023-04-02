<div align="center">
<img src="./static/icon.svg" alt="preview"/>

<h1 align="center">ChatGPT Next Web</h1>

Deploy your private ChatGPT web application for free with one click. 7

One-Click to deploy your own ChatGPT web UI.
[Demo](https://chat-gpt-next-web.vercel.app/) / [Issues](https://github.com/TheColdPrince/ChatGPT-Next-Web/issues) ]

[![Deploy with Vercel](https://vercel.com/button)](https://vercel.com/new/clone?repository-url=https%3A%2F%2Fgithub.com%2FTheColdPrince%2FChatGPT-Next-Web&env=OPENAI_API_KEY&env=CODE&project-name=chatgpt-next-web&repository-name=ChatGPT-Next-Web)


![Main interface](./static/cover.png)

</div>


## Features

- **Deploy for free with one-click** on Vercel in under 1 minute
- Responsive design, and dark mode
- Fast first screen loading speed (~85kb)
- Awesome prompts powered by [awesome-chatgpt-prompts-zh](https://github.com/PlexPt/awesome-chatgpt-prompts-zh) and [awesome-chatgpt-prompts](https://github.com/f/awesome-chatgpt-prompts)
- Automatically compresses chat history to support long conversations while also saving your tokens
- One-click export all chat history with full Markdown support

## Roadmap
- System Prompt: pin a user defined prompt as system prompt Prompt [#138](https://github.com/TheColdPrince/ChatGPT-Next-Web/issues/138)
- User Prompt: user can edit and save custom prompts to prompt list
- Self-host Model: support llama, alpaca, ChatGLM, BELLE etc. 
- Plugins: support network search, caculator, any other apis etc. api [#165](https://github.com/TheColdPrince/ChatGPT-Next-Web/issues/165)

### Not in Plan
- User login, accounts, cloud sync
- UI text customize 

## Get Started

1. Get [OpenAI API Key](https://platform.openai.com/account/api-keys);
2. Click
   [![Deploy with Vercel](https://vercel.com/button)](https://vercel.com/new/clone?repository-url=https%3A%2F%2Fgithub.com%2FTheColdPrince%2FChatGPT-Next-Web&env=OPENAI_API_KEY&env=CODE&project-name=chatgpt-next-web&repository-name=ChatGPT-Next-Web);
3. Enjoy :)

If you have deployed your own project with just one click following the steps above, you may encounter the issue of "Updates Available" constantly showing up. This is because Vercel will create a new project for you by default instead of forking this project, resulting in the inability to detect updates correctly.

We recommend that you follow the steps below to re-deploy:

- Delete the original repo;
- Fork this project;
- Go to the Vercel dashboard, delete the original project, then create a new project and select the project you just forked to redeploy;
- Please manually add an environment variable named `OPENAI_API_KEY` and enter your API key as the value during the redeploy process.

This project will be continuously maintained. If you want to keep the code repository up to date, you can check out the [Github documentation](https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/working-with-forks/syncing-a-fork) to learn how to synchronize a forked project with upstream code. It is recommended to perform synchronization operations regularly.

You can star or watch this project or follow author to get release notifictions in time.

## Password

This project provides limited permission control functions. Please add an environment variable named `CODE` on the environment variable page of the Vercel project control panel, and the value is a custom password separated by English commas: 78

```
code1,code2,code3
```

After adding or modifying this environment variable, please **re-deploy** the project to make the changes take effect. 84

This project provides limited access control. Please add an environment variable named `CODE` on the vercel environment variables page. The value should be passwords separated by comma like this:

```
code1,code2,code3
```

After adding or modifying this environment variable, please redeploy the project for the changes to take effect.

## Environment Variables

### `OPENAI_API_KEY` (required)

OpanAI。

Your openai api key.

### `CODE` (optional)


Access passsword, separated by comma.

### `BASE_URL` (optional)

> Default: `api.openai.com`

OpenAI URL。

Override openai api request base url.

### `PROTOCOL` (optional)

> Default: `https`

> Values: `http` | `https`

OpenAI。

Override openai api request protocol.

## Development


[![Open in Gitpod](https://gitpod.io/button/open-in-gitpod.svg)](https://gitpod.io/#https://github.com/TheColdPrince/ChatGPT-Next-Web)


Before starting development, you must create a new `.env.local` file at project root, and place your api key into it:

```
OPENAI_API_KEY=<your api key here>
```

###  Local Development


1.  nodejs  yarn， ChatGPT；
2.  `yarn install && yarn dev` 。

### Local Deployment

```shell
bash <(curl -s https://raw.githubusercontent.com/TheColdPrince/ChatGPT-Next-Web/main/scripts/setup.sh)
```

###  Docker Deployment

```shell
docker pull yidadaa/chatgpt-next-web

docker run -d -p 3000:3000 -e OPENAI_API_KEY="" -e CODE="" yidadaa/chatgpt-next-web
```

##  Screenshots

![ Settings](./static/settings.png)

![ More](./static/more.png)


##  Special Thanks


###  Contributor

[Contributors](https://github.com/TheColdPrince/ChatGPT-Next-Web/graphs/contributors)

## LICENSE

[Anti 996 License](https://github.com/kattgu7/Anti-996-License/blob/master/LICENSE_CN_EN)
