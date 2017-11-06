## Server Setup
```bash
$ pip install Flask
$ export FLASK_APP=api.py
$ flask run
 * Running on http://localhost:5000/
```

## API
#### Request
`http://127.0.0.1:5000/uid/[uid]`
#### Response Example
##### Success
`response code: 200`
```json
[
  {
    "path": "[local relative path]",
    "size": "[size in bytes]"
  },
  {
    "path": "target/assets/sketches/2mCaPnNc/heb_o_rav_2017-10-03_lesson_bs-pticha_n1_p2_pic01.jpg",
    "size": 308258
  }
]
``` 
##### Error
`response code: 400`
```json
{"error": "[error message]"}
``` 
