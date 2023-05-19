# Python Minecraft-Monitoring API

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

[![PyPi Version](https://img.shields.io/pypi/v/mmon-api.svg)](https://pypi.org/project/mmon-api/)

This is a reverse engineered API wrapper for [Minecraft-Monitroing.ru](https://monitoringminecraft.ru), which allow you automate the process.

## Features:
------------
- Log in with token (authautologin cookie)
- Add new server
- Remove exist server
- Edit exist server
- Display server list
- Support markdown
- Helpful params

## Documentation:
-----------------
Examples can be found in the /examples directory. To run these examples, replce `auth_token` in your token.

```python
client = Client('your_auth_token_here')
```

### Finding Your Token:
Log into [Minecraft-Monitroing.ru](https://monitoringminecraft.ru) on any browser, then open your browser's developer tools (also known as "inspect") and look for the value of the `authautologin` cookie in the following menus:
- Chromium: Devtools > Application > Cookies > monitoringminecraft.ru
- Firefox: Devtools > Storage > Cookies
- Safari: Devtools > Storage > Cookies

### Using the Client:
To use this library, simply import mmonitoring and create a mmonitoring.Client instance. The Client class accepts the following arguments:
```
authautologin - The token to use.

user_agent - The user agent.
```

Regular Example:
```python 
from mmonitoring import Client

client = Client('auth_token')
```

## Copyright:
-------------
This program is licensed under the MIT.

### Copyright Notice:
```
MIT License

Copyright (c) 2023 Xpos587

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
```