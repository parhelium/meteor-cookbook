## Deploying multiple meteor apps to one server

### Error : Uploading bundle: FAILED

```
[xx.xx.xx.xx] - Uploading bundle
[xx.xx.xx.xx] x Uploading bundle: FAILED
	No such file
```

For every app always run `mup setup` before running `mup deploy`.

### Error : Cannot connect to localhost:PORT

Always check what is logged by app :

```
mup logs -fn 400
```
