## Callbacks

### new_message

```js
visitorApi.on('new_message', (newMessage) => {
    console.log(newMessage)
})
```
Response:

| param      | type    | description                   |
| ---------- | ------- | ----------------------------- |
| messageId  | string  | Message Id                    |
| authorId   | string  | Message author Id             |
| timestamp  | number  | Timestamp added by server     |
| text       | string  | Message text                  |
| chatId     | string  | Message chat id               |
| history    | boolean | Is event retrieved as history |

### visitor_banned - not implemented yet

```js
visitorApi.on('visitor_banned', (data) => {
    console.log(data)
})
```

Feature description: [Visitor banning](https://www.livechatinc.com/features/chat-tools/#Chat-tools-other-features)

### chat_started

```js
visitorApi.on('chat_started', (chatData) => {
    console.log(chatData)
})
```

### visitor_queued - not implemented yet

```js
visitorApi.on('visitor_queued', (queueData) => {
    console.log(queueData)
})
```

### new_file - not implemented yet

```js
visitorApi.on('new_file', (newFile) => {
    console.log(newFile)
})
```

Feature description: [File sharing](https://www.livechatinc.com/features/chat-tools/#File-sharing)

### agent_changed

```js
visitorApi.on('agent_changed', (newAgent) => {
    console.log(newAgent)
})
```

### typing_indicator - not implemented yet

```js
visitorApi.on('typing_indicator', (typingData) => {
    console.log(typingData)
})
```

### message_seen - not implemented yet

```js
visitorApi.on('message_seen', (messageData) => {
    console.log(messageData)
})
```

Feature description: [Delivery status](https://www.livechatinc.com/features/chat-tools/#Delivery-status)
