# Intl Template Literals (concept)
Just an idea about how we could write intl components. Inspired by [styled-components](https://github.com/styled-components/styled-components)

## The problem with current Intl component

Currently Intl components often look like this:
```js
<FormattedMessage
    id="welcome"
    values={{name: <b>{name}</b>, unreadCount}}
/>
```
with somewhere else in you code the message:
```js
const messages = {
  'welcome': `Hello {name}, you have {unreadCount, number} {unreadCount, plural,
    one {message}
    other {messages}
  }`
};
```
The main problem here is that when you read you code, you don't really know what `id="welcome"` will render. If you want to know what it says, you have to find the message associated with it, which is quite anoying.

## Solution (maybe) : Template Literals

![]()
