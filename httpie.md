```python
pip install httpie
```

---

```python
http http://127.0.0.1:8000/snippets/
```

```shell
HTTP/1.1 200 OK
Content-Length: 354
Content-Type: application/json
Date: Thu, 02 Jul 2020 04:19:12 GMT
Server: WSGIServer/0.2 CPython/3.7.3
X-Content-Type-Options: nosniff
X-Frame-Options: DENY

[
    {
        "code": "foo = \"bar\"\n",
        "id": 1,
        "language": "python",
        "linenos": false,
        "style": "friendly",
        "title": ""
    },
    {
        "code": "print(\"hello, world\")\n",
        "id": 2,
        "language": "python",
        "linenos": false,
        "style": "friendly",
        "title": ""
    },
    {
        "code": "print(\"hello, world\")",
        "id": 3,
        "language": "python",
        "linenos": false,
        "style": "friendly",
        "title": ""
    }
]
```

---

```python
http http://127.0.0.1:8000/snippets/2
```

```shell
HTTP/1.1 200 OK
Content-Length: 120
Content-Type: application/json
Date: Thu, 02 Jul 2020 04:19:28 GMT
Server: WSGIServer/0.2 CPython/3.7.3
X-Content-Type-Options: nosniff
X-Frame-Options: DENY

{
    "code": "print(\"hello, world\")\n",
    "id": 2,
    "language": "python",
    "linenos": false,
    "style": "friendly",
    "title": ""
}
```