ajax_django
===========

A simple wrapper written on top of jquery to make making AJAX requests to Django Servers easier. Django needs a csrf token to receive any POST request. The ajax_upload.js file has the functions to add csrf tokens to the header of the request. This allows easier and less time consuming Ajax requests.


How to Install
===============
Download ajax_upload.js file and add it to the head section of your html file (or at the end of the body section of your html) after you add your jquery file.

```
<html>
  <head>
    <script src="jquery.js"></script>
    <script src="ajax_upload.js"></script>
  </head>
  .
  .
  .
```


## Code inside ajax_upload.js file will 

- Get cookie called `csrftoken` 
- Add the cookie to the header `X-CSRFToken` every time an ajax call is made with jquery by utilizing beforeSend hook. 
