## Generate ssh keys

```
ssh-keygen -t rsa -b 4096 -C "your_email@example.com"
```

## Add SSH key after creating a droplet
```
cat ~/.ssh/id_rsa.pub | ssh USER@IP.ADDRESS "cat >> ~/.ssh/authorized_keys"
```

Or you can create file `~/.ssh/config` with text:

```
Host NAME
	Hostname 999.999.999.99
    User root
```

```
cat ~/.ssh/id_rsa.pub | ssh NAME "cat >> ~/.ssh/authorized_keys"
```