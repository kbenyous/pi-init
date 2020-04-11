
# init-pi

Playbook d'initialisation d'un Raspberry Pi sous Debian Buster

# Prérequis

* Un Raspberry Pi
* Une carte micro-SD avec une distro Raspbian récente (testé sur Buster)
* Le serveur SSH activé (créer un fichier vide 'ssh' à la racine de la partition 'boot' sur la carte SD)
* Le hostname ou l'adresse IP allouée par le serveur DHCP
* Ansible + Python sur le poste de développement
* sshpass sur le poste de développement

# Exécution

* Créer un fichier d'inventaire Ansible :

```(ini)
[pi]
ma_machine ansible_ssh_user=nouvel_utilisateur ansible_host=hostname_ou_adresse_ip
```
