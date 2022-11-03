# Frontend Customization

## Requirements
1. NativeChat account (If you don't have one, you can register at https://bots.nativechat.com/register)

## How to change the appearance of a bot
1. Create new blank bot from https://bots.nativechat.com/bots/create
2. Replace the Cognitive Flow of the created bot with the content of the `cognitive-flow.json` file.
3. Publish it for the Web channel ([Publishing documentation](https://docs.nativechat.com/docs/1.0/publishing/web.html))
4. Set the `display.launcher.openIconUrl` and the `display.launcher.closeIconUrl` properties in the generated code snippet to the URLs of your desired icons (see example below) ([Display properties documentation](https://docs.nativechat.com/docs/1.0/publishing/web.html#display-required))
5. Add URLs to your CSS files in the `chat.css` property (see example below) ([Chat properties documentation](https://docs.nativechat.com/docs/1.0/publishing/web.html#chat-required))
> Note: You can create your own theme with the [Progress ThemeBuilder](https://themebuilderapp.telerik.com)

## Example web widget configuration
```JavaScript
var chatSettings = {
    bot: {
        id: "<bot-id>"
    },
    channel: {
        id: "<channel-id>",
        token: "<channel-token>"
    },
    googleApiKey: "your-google-maps-API-key",
    session: {
        clear: true
    },
    css: [
        "https://nativechat.github.io/accelerators/resources/Frontend%20Customization/style.css"
    ]
};

window.NativeChat.load({
    id: "kcChatWindow",
    origin: "",
    display: {
        mode: "modal",
        launcher: {
            openIconUrl: "https://nativechat.github.io/accelerators/resources/Frontend%20Customization/open-icon.svg",
            closeIconUrl: "https://nativechat.github.io/accelerators/resources/Frontend%20Customization/close-icon.svg"
        }
    },
    chat: chatSettings
});
```

## Before
<image src="../resources/Frontend%20Customization/before-open-icon.png" alt="Before Open Icon" style="width:25%;height:25%" /> <image src="../resources/Frontend%20Customization/before-chat.png" alt="Before Chat" style="width:25%;height:25%" />

## After
<image src="../resources/Frontend%20Customization/after-open-icon.png" alt="After Open Icon" style="width:25%;height:25%" /> <image src="../resources/Frontend%20Customization/after-chat.png" alt="After Chat" style="width:25%;height:25%" />
