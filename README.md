# Chatty

Chatty is a jQuery add-on that creates a chatbot-like experience from a json question format. [Live Demo](https://jsfiddle.net/wfuchs/6svdqpce/29/)

## Setup

Add the style and javascript files to your html markup

```html
<link rel="stylesheet" href="chatbot/chat-style.css">
<script src="./chatbot/chatModule.js" type="text/javascript"></script>
```

## Usage

```javascript
var tags = [
    {
        type: "input",
        tag: "text",
        "chat-msg": "Hello, World! What is your name?",
        name: "name",
        placeholder: "Snazzy McChatbot"
    },
    {
        type: "msg",
        "chat-msg": "Nice to meet you, {{name}}! Welcome to Chatty"
    }
];

$(document).ready(function () {
    Chat.start($('#chat-context'), tags);
});
```

## Dependencies

Chatty relies on the following:

* [Velocity.js](https://github.com/julianshapiro/velocity)
* [jQuery](https://jquery.com/)


## Documentation

Full documentation lives in the repo wiki. [Check it out!](https://github.com/WiFuchs/chatty/wiki)

## Contributing
Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.
