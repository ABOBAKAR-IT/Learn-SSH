# SSH key setup for remote server

1) Generate a new SSH key pair
```bash
ssh-keygen
```

- When you're prompted to "Enter a file in which to save the key," press Enter. This accepts the default file location.
- At the prompt, type a secure passphrase. For more information, see "Working with SSH key passphrases. For default press Enter.


2) Copy the public key to your remote server
```bash
ssh-copy-id username@remote_host
```
- If face Error try this..

```bash
ssh-copy-id -i ~/.ssh/id_rsa.pub USERNAME@IP_ADDRESS
```

3) Test the connection
```bash
ssh username@remote_host
```
