# expo-serverless-push-notifications

Please read [Expo push notifications](https://docs.expo.io/versions/latest/guides/push-notifications.html) for more information.

Uses webpack with babel before pushing to AWS meaning that ES7/ES8 functionality can be used.

This will send the same notification to multiple users. Simply refactor the code if you want to support different messages for each recipient.

## Instructions

- clone and deploy to AWS
- test the function in Postman with some data in the following format:

```javascript
{
	"recipients": ["ExponentPushToken[EXAMPLEID]", "ExponentPushToken[EXAMPLEID2]"],
	"sound": "default",
	"title": "Notification title",
	"body": "Main content of the notification",
	"data": {
    "importantData": "you want to use in the app"
	}
}
```
