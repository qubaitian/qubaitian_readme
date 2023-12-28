---
title: Authentication
excerpt: The authentication flows of SeaTable.
category: 658bc87fd352d6004fe43f8f
isReference: true
---

There are two ways to authenticate with the Seafile API:


All other API-requests require an authorization header that looks like this, where different tokens can be used.

`Authorization: Bearer {{Account-Token, Library-Token}}`

## The two tokens

> Account-Token
>
> An **Account-Token** is generated when you login to Seafile. Generally, there is no need to generate an Account-Token manually.
> Seafile websites will automatically generate an Account-Token for you and store it in your browser's local storage. This token is valid until you logout.
> Almost your operations require an Account-Token.

> Library-Token
>
> An **Library-Token** is like a password to use the API requests of a single library. 
> You can create as many API-Token per base as you want. Every Library-Token can have read or write permissions. This token is valid until you delete them.
> If the user only needs to manipulate the contents of a specific database, it is more secure to use the library API token.


