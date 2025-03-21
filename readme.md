# RSS Proxy

This application creates a simple proxy server that fetches RSS feeds from NOS and returns them. It helps bypass CORS restrictions when accessing NOS feeds from a browser-based application.

This tool is only used during the code assignment for the hiring of our frontend developer position.

## Installation

1. Clone this repository
2. Install dependencies:

```bash
npm install
```

## Usage

1. Start the server:

```bash
node index.js
```

The server will run on port 3000 by default.

2. Access NOS feeds through the proxy:

```
[GET] http://localhost:3000/:feed
```

Where `:feed` is the name of the feed you want to access, for example:
- `nosnieuwsalgemeen` (General news)
- `nossportalgemeen` (Sports news)
- `nosnieuwseconomie` (Economic news)

Example:
```
http://localhost:3000/nosnieuwsalgemeen
```

You can find all feeds [here](https://nos.nl/feeds)