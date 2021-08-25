### info
Responses are compressed when the following criteria are all met:

- The response body is larger than 1400 bytes.
- The Accept-Encoding request header contains gzip.
- The response is not already compressed, i.e. the Content-Encoding response header is not already set.

If the Content-Type header is not defined, or empty, the compress middleware will automatically detect a content type. It will also set the Content-Type header according to the detected MIME type.
