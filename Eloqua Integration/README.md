# Eloqua Integration

## Requirements
1. NativeChat account (If you don't have one, you can register at https://bots.nativechat.com/register)
2. Eloqua blind form submit link

## How to create bot
1. Create new blank bot from https://bots.nativechat.com/bots/create
2. Replace the Cognitive Flow of the created bot with the content of the `cognitive-flow.json` file.
3. Replace all occurrences of `__ELOQUA_BLIND_FORM_SUBMIT_LINK__` in the Cognitive Flow of the bot with your Eloqua blind form submit link.
4. Replace the training of the created bot with the content of the `entity-definitions.json` file.
