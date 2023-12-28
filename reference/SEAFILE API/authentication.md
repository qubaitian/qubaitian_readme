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
> An **Account-Token** authenticates an _account API request_ (=Account Operations) like add a new base, add a group member or list all collaborators of a base. The Account-Token can be generated with the account-credentials.

> Library-Token
>
> An **API-Token** is like a password to use the API requests of a single base. The main purpose of an API-Token is to generate a Base-Token.
> You can create as many API-Token per base as you want. Every API-Token can have different read or write permissions. This token is valid until you delete them.

