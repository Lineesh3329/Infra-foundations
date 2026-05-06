# Remote Command Execution

- This runs commands on another machine (Remote server) from our local machine inorder to make the process run automate.
- To execute this we need- SSH access, Username, IP Address, Password or SSH Key
- It uses SSH- we connect to a remote server and execute commands.

          ssh user@remote_ip "command"
          ssh ec2_user@192.168.1.10 "uptime"                                    Output: shows uptime

  Passwordless SSH
  -
  Passwodless SSH uses key-based authentication to securely connect to remote systems without a password.

  1.Generate Key pair
  -
  
  `ssh-keygen` used to generates key pairs, which creates private and public keys.

          ~/.ssh/id-rsa      (private key)  ---------> stores in our local system
          ~/.ssh/id-rsa.pub   (public key)  ---------> stores in server (remote)

  2.Copy public Key to Remote Server.
  -
          ssh-copy-id user@remote_ip -----------------------> ~/.ssh/authorized_keys
                                       *adds key to local*


   3.Login
  -
          ssh user@server_ip --------------------> Login without password
          ssh user@server "deploy.sh" -----------> Runs automatically without password

    Note:
    -

    - Keep private keys safely.
    - Use correct permissions `chmod 600 ~/.ssh/id-rsa`
    - `crontab -e`is used to run ccron jobs in bash scripting.                                      
