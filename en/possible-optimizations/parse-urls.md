# Parse URLs

We need to find an efficient way to recognize and parse local paths and web urls.

#### Categories:

* Local Absolute Path for Unix-like OS
* Local Absolute Path for Windows OS
* Local Relevant Path for both Windows and Unix-like OS
* HTTP Web URLs
* HTTPS Web URLs
* FTP Web URLs
* MySQL / MariaDB Access URLs
* PostgreSQL Access URLs
* MongoDB Access URLs
* ......

#### Goal

1. Recognize if a given string is a local path or a web URL, because they will be treated in very different ways.
2. When you know that is a web URL, find out what protocol it uses, that is to say, the type of URL.
3. What are differences between web URLs and database URLs?

#### Relevant Methods:

```cpp
parse_path()
```
