<p align="center">
    <a href="https://github.com/pyrogram/pyrogram">
        <img src="https://docs.pyrogram.org/_static/pyrogram.png" alt="Pyrogram" width="128">
    </a>
    <br>
    <b>Telegram MTProto API Framework for Python</b>
    <br>
    <a href="https://pyrogram.org">
        Homepage
    </a>
    •
    <a href="https://docs.pyrogram.org">
        Documentation
    </a>
    •
    <a href="https://docs.pyrogram.org/releases">
        Releases
    </a>
    •
    <a href="https://t.me/pyrogram">
        News
    </a>
</p>

## Pyrogram (fixed fork, no ban)

> Elegant, modern and asynchronous Telegram MTProto API framework in Python for users and bots

``` python
from pyrogram import Client, filters

app = Client("my_account")


@app.on_message(filters.private)
async def hello(client, message):
    await message.reply("Hello from Pyrogram!")


app.run()
```

> Example of client (user-bot)
``` python
from pyrogram import Client, filters

app = Client(
    "pyrogram",
    api_id = 2496, # set any
    api_hash = "8da85b0d5bfe62527e5b244c209159c3", # set any
    app_version = "1.9.6", # set any
    device_model= "Safari 16.4", # set any
    system_version = "1.9.6 (418)", # set any
    system_lang_code = "en" # if client is PC it should be en-US or something like it
    lang_code = "en", # set any
    lang_pack = "tdesktop" # different apps (official) have different langpacks
    )


@app.on_message(filters.private)
async def hello(client, message):
    await message.reply("btw i use pyro.")


app.run()
```

> Examples of official apps
``` python
# TDesktop
api_id = 2040
api_hash = "b18441a1ff607e10a989891a5462e627"
device_model = "Desktop"
system_version = "Windows 11"
system_lang_code = "en-US"
app_version = "5.0.1 x64"
lang_code = "en"
lang_pack = "tdesktop"

# Android
api_id = 6
api_hash = "eb06d4abfb49dc3eeb1aeb98ae0f581e"
device_model = "Samsung SM-G998B"
system_version = "SDK 31"
system_lang_code = "en"
app_version = "10.9.1 (4464)"
lang_code = "en"
lang_pack = "android"

# Android X
api_id = 21724
api_hash = "3e0cb5efcd52300aec5994fdfc5bdc16"
device_model = "Samsung SM-G998B"
system_version = "SDK 31"
system_lang_code = "en"
app_version = "8.4.1 (2522)"
lang_code = "en"
lang_pack = "android"

# IOS
api_id = 8
api_hash = "7245de8e747a0d6fbe11f7cc14fcc0bb"
device_model = "iPhone 15 Pro Max"
system_version = "16.8.1"
system_lang_code = "en"
app_version = "10.0.3 (26855)"
lang_code = "en"
lang_pack = "ios"

# MacOS
api_id = 9
api_hash = "3975f648bb682ee889f35483bc618d1c"
device_model = "MacBook Pro"
system_version = "macOS 12.0.1"
system_lang_code = "en"
app_version = "4.0.1"
lang_code = "en"
lang_pack = "macos"

# Web_A
api_id = 2496
api_hash = "8da85b0d5bfe62527e5b244c209159c3"
device_model = "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/124.0.0.0 Safari/537.36"
system_version = "Win32"
app_version = "10.9.5"
lang_code = "en"
system_lang_code = "en"
lang_pack = "webk"

```

**Pyrogram** is a modern, elegant and asynchronous [MTProto API](https://docs.pyrogram.org/topics/mtproto-vs-botapi)
framework. It enables you to easily interact with the main Telegram API through a user account (custom client) or a bot
identity (bot API alternative) using Python.

### Support

If you'd like to support Pyrogram, you can consider:

- [Become a GitHub sponsor](https://github.com/sponsors/delivrance).
- [Become a LiberaPay patron](https://liberapay.com/delivrance).
- [Become an OpenCollective backer](https://opencollective.com/pyrogram).

### Key Features

- **Ready**: Install Pyrogram with pip and start building your applications right away.
- **Easy**: Makes the Telegram API simple and intuitive, while still allowing advanced usages.
- **Elegant**: Low-level details are abstracted and re-presented in a more convenient way.
- **Fast**: Boosted up by [TgCrypto](https://github.com/pyrogram/tgcrypto), a high-performance cryptography library written in C.  
- **Type-hinted**: Types and methods are all type-hinted, enabling excellent editor support.
- **Async**: Fully asynchronous (also usable synchronously if wanted, for convenience).
- **Powerful**: Full access to Telegram's API to execute any official client action and more.

### Installing

``` bash
pip3 install pyrogram
```

### Resources

- Check out the docs at https://docs.pyrogram.org to learn more about Pyrogram, get started right
away and discover more in-depth material for building your client applications.
- Join the official channel at https://t.me/pyrogram and stay tuned for news, updates and announcements.
