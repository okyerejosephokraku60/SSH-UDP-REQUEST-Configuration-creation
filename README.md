# SSH-UDP-REQUEST-Configuration-creation
How to create an SSH UDP REQUEST Configuration using Termux, must have account details created by fastssh.com


Here are the steps to create an SSH UDP REQUEST configuration in Termux:

1. Install the "nano" text editor if not already installed by running the following command:
```
pkg install nano
```

2. Create a new configuration file using the "nano" text editor by running the following command:
```
nano /data/data/com.termux/files/home/.ssh/config
```

3. Enter the following configuration settings in the editor:
```
Host server-name
    HostName server-ip-address
    User username
    ProxyCommand nc -u -w 1 proxy-server-ip-address proxy-server-port
```

Note: Replace "server-name", "server-ip-address", "username", "proxy-server-ip-address", and "proxy-server-port" with the appropriate values for your configuration.

4. Save the configuration settings and exit the editor by pressing "Ctrl+X", then "Y", then "Enter".

5. Test the SSH connection using the UDP request configuration by running the following command:
```
ssh server-name
```

Note: Replace "server-name" with the name you assigned in the configuration file.

CREATION OF SSH UDP REQUEST CONFIGURATION FROM WEBSITE.

Visit "https://www.fastssh.com/page/ssh-udp-request/" to create any of the accounts available by entering preferred Username and Password.
