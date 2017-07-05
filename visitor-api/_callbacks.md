## Callbacks

Callbacks let you bind a custom JavaScript function to an event. For example, your function can be invoked every time agent's message was received.

### new_message

```js
visitorApi.on('new_message', (newMessage) => {
    console.log(newMessage)
})
```
Payload:

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
Payload:

| param  | type    | description |
| ------ | ------- | ----------- |
| chatId | string  | New chat id |

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

### agent_changed - not implemented yet

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
