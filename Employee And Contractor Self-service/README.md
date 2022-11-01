# Employee And Contractor Self-service

## Requirements
1. NativeChat account (If you don't have one, you can register at https://bots.nativechat.com/register)
2. Google Maps API key

## How to create bot
1. Create new blank bot from https://bots.nativechat.com/bots/create
2. Replace the Cognitive Flow of the created bot with the content of the `cognitive-flow.json` file.
3. Replace all occurrences of `__GOOGLE_API_KEY__` in the Cognitive Flow of the bot with your Google Maps API key.
4. Replace the training of the created bot with the content of the `entity-definitions.json` file. [Import training definitions documentation](https://docs.nativechat.com/docs/1.0/nlp-training/import-training-definition.html#import-training-definitions)
