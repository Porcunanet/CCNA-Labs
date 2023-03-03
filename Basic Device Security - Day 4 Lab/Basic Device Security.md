# Basic Device Security

1. Change the hostnames of the router and switch to the appropriate names (R1, SW1)
     * Use the 'hostname' command in global configuration mode

2.  Configure an unencrypted enable password of 'CCNA' on both devices
	```sh
		enable password CCNA
	```

3. Exit back to user EXEC mode and test the password

4.  View the password in the running configuration
	```sh
		do show run
	```

5. Ensure that the current password, and all future passwords, are encrypted
	```sh
		service password-encryption 
	```

6. View the password in the running configuration
	```sh
		do show run
	```

7. Configure a more secure, encrypted enable password of 'Cisco' on both devices
	```sh
		enable secret Cisco
	```

8. Exit back to user EXEC mode and then return to privileged EXEC mode.
    Which password do you have to use?
	secret password
9. View the passwords in the running configuration.
     What encryption type number is used for the encrypted 'enable password'?
		7
     What encryption type number is used for the encrypted 'enable secret'?
		5

10. Save the running configuration to the startup configuration
	```sh
		do wr
	```