# KN03: Cloud-init und AWS
## A) Cloud-init Datei Verstehen
```#cloud-config                        

users:                                  # Benutzerkonfiguration
  - name: ubuntu                        # Benutzername
    sudo: ALL=(ALL) NOPASSWD:ALL        # sudo-regeln für diesen benutzer
    groups: users, admin                # Benutzer ist Mitglied in den Gruppen "users" und "admin"
    home: /home/ubuntu                  # Benutzerverzeichnis: /home/ubuntu
    shell: /bin/bash                    # Verwendete Shell: /bin/bash
    ssh_authorized_keys:                # SSH-öffentlicher Schlüssel zur Authentifizierung
      - ssh-rsa AAAAB3NzaC1yc2EAAAADAQABAAABAQC0WGP1EZykEtv5YGC9nMiPFW3U3DmZNzKFO5nEu6uozEHh4jLZzPNHSrfFTuQ2GnRDSt+XbOtTLdcj26+iPNiFoFha42aCIzYjt6V8Z+SQ9pzF4jPPzxwXfDdkEWylgoNnZ+4MG1lNFqa8aO7F62tX0Yj5khjC0Bs7Mb2cHLx1XZaxJV6qSaulDuBbLYe8QUZXkMc7wmob3PM0kflfolR3LE7LResIHWa4j4FL6r5cQmFlDU2BDPpKMFMGUfRSFiUtaWBNXFOWHQBC2+uKmuMPYP4vJC9sBgqMvPN/X2KyemqdMvdKXnCfrzadHuSSJYEzD64Cve5Zl9yVvY4AqyBD aws-key    # Öffentlicher SSH-Schlüssel
ssh_pwauth: false                       # SSH-Passwort-Authentifizierung ist deaktiviert
disable_root: false                     # Das Deaktivieren des Root-Benutzers ist deaktiviert
package_update: true                    # Paketaktualisierungen werden durchgeführt
packages:                               # Zusätzliche Pakete, die installiert werden
  - curl                                # Paket: curl
  - wget                                # Paket: wget
```
<<<<<<< HEAD

## B)
![Alt text](ssh-pem-1-1.png)
![Alt text](ssh-pem-2-1.png)
![Alt text](which-key-used-1.png)
![Alt text](cloud-init-log-1.png)
## C)
Durchgeführt
## D)
### DB-Server
![Alt text](mysql-1.png)
![Alt text](telnet-1.png)

### Web-Server
![Alt text](index-1.png)
![Alt text](info-1.png)
![Alt text](mysql-1.png)
![Alt text](db-1.png)
![Alt text](adminer-1.png)
=======
## B) SSH-Key und Cloud-init
![which-key-used](https://github.com/nussbaumerv/m346/assets/112619659/f5aa7f0e-8784-4748-8dbf-495f45154eeb)
![ssh-pem-1](https://github.com/nussbaumerv/m346/assets/112619659/50953e75-a546-4b99-b459-8334973913d5)
![ssh-pem-2](https://github.com/nussbaumerv/m346/assets/112619659/61bae914-e61b-40bc-97d8-9d82e18a1cd0)
![cloud-init-log](https://github.com/nussbaumerv/m346/assets/112619659/296ef2c6-f55e-4e68-b4e2-e01d6fde1690)
>>>>>>> 6b30efb6ec97774bf6b7b514e67298828c44021d
