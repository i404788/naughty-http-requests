# naughty-http-requests
A list of naughty HTTP requests, revealing commonly unpatched issues

## How to use/read
In general it's a file with newline-delimited strings each containing one requests.
Commented lines start with `#`.

Some requests are simplified by their regex, however we don't have any scripts to parse them yet so things can change.

## How does it work?
We run many http servers with full logs of which requests were made.
We go through the logs (mainly 404 requests) and check their content.
Since our servers won't allow requests which don't have a specific destination it's relatively easy to filter through.

## Sponsored by
* https://devdroplets.com
