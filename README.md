# URL Shortener

A simple URL shortener application that converts long URLs into short, shareable links.

## Features

* Shorten long URLs instantly
* Redirect users from short links to original URLs
* Generate unique short codes
* Basic URL validation
* Lightweight and easy to deploy

## Getting Started

### Prerequisites

* Node.js (or your preferred runtime)
* Database (MongoDB, PostgreSQL, etc.)

### Installation

```bash
git clone https://github.com/yourusername/url-shortener.git
cd url-shortener
npm install
npm start
```

### Usage

1. Submit a long URL through the API or web interface.
2. Receive a shortened URL.
3. Share the shortened link.
4. Users visiting the short URL are redirected to the original destination.

## API Endpoints

### Create Short URL

```http
POST /shorten
```

Request:

```json
{
  "url": "https://example.com/very/long/url"
}
```

Response:

```json
{
  "shortUrl": "https://short.ly/abc123"
}
```

### Redirect

```http
GET /:shortCode
```

Redirects to the original URL.

## Project Structure

```text
src/
├── controllers/
├── routes/
├── models/
├── services/
└── app.js
```

## Future Improvements

* Custom aliases
* Click analytics
* User authentication
* Link expiration
* QR code generation

## License

MIT License.
