# KMK DevOps Coding Challenge App

This is small flask app. This app will show request headers and client ip
address in JSON format.

## Installation

Clone the repository, then install required python modules (see requirements.txt).
Then, you can run this app using this command

```
./app.py
```

It will listen on all interface on port 5000.

## Example output

Using curl, assuming app listen on ip address 10.10.10.20. and curl running on
host with ip address 10.10.10.2

```
curl http://10.10.10.20:5000/
```

output

```
{
  "headers": {
    "Accept": "*/*",
    "Content-Length": "",
    "Content-Type": "",
    "Host": "localhost:5000",
    "User-Agent": "curl/7.51.0"
  },
  "origin": "10.10.10.2"
}
```
