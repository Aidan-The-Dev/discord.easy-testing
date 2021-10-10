



# ❓ How To Install

> 1)     You need Node.js version 12.0.0 or newer

<br>

> 2)     Use the install command in your terminal

### For npm use
```txt
npm install discord.easy-testing
```

 > For yarn use
```txt
yarn install discord.easy-testing
```
<br>

 # 🖥️ Setup
```javascript
const discord = require('discord.easy-testing')
const client = new discord.Client('your-bot-token-here')
```

# 💻 Example Code
```javascript
const discord = require('discord.easy-testing')
const client = new discord.Client('your-bot-token-here')
const prefix = '?'

client.once('ready', () => {
    console.log('Ready!')
})

client.on('message', message => {
    if(message.content === `${prefix}text`) {
        client.send(message.channelID, 'Hello World!')
    }
})

client.on('message', message => {
    if(message.content === `${prefix}embed`) {
        const embed = new discord.Embed()
        .setTitle('Hello!')
        .setColor('RANDOM')
        .setDescription('Hello World!')
        client.send(message.channelID, embed)
    }
})

client.connect()
```

<br><br><br>

# 👤 Support Server
**[https://discord.gg/XQawK6PTga](https://discord.gg/XQawK6PTga)**