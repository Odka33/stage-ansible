# Ansible

###### Introduction :

Ansible est une plate-forme logicielle libre pour la configuration et la gestion des ordinateurs. Elle combine le déploiement de logiciels multi-nœuds, l'exécution des tâches ad-hoc, et la gestion de configuration. Elle gère les différents nœuds par-dessus SSH et ne nécessite l'installation d'aucun logiciel supplémentaire à distance sur eux.

###### Objectif :

L'objectif de ce projet est la mise en place d'un cadre de travail pour développeur. La technologie Ansible permettant l'automatisation de tâche et l'installation de service ainsi que leur configuration.

###### Fonctionnalités :

- Installation des packet.
- Mise en place d'un cadre de travail. (Front-end)
- Réalisation des services de base de donnée ainsi que des technologies de programmation. (Back-end)

###### Architecture des scripts Yaml:

.

├── ansible.test.apache

├── ansible.test.borg

├── ansible.test.common

├── ansible.test.mix

├── ansible.test.multi

├── ansible.test.mysql

├── ansible.test.php

###### Recommandation :

Il est recommandé d'avoir travaillé sur ansible avant de commencer à utilisé se code.

C'est playbook ont été testé uniquement sous debian 8. Cependant, ils sont suseptibles de fonctionner sûr d'autre distribution telle que debian , kali, ubuntu possédant un gestionnaire APT.

Installation d'Ansible :

`sudo apt install ansible -y`

Example:

Fichier hosts:

[hosts] Changer avec le nom que vous désirez.

0.0.0.0   Changer avec l'ip de la machine à gérer.

Fichier group_vars:

Afin de faire fonctionner le script correctement il faut remplacer les variable selon votre configurations serveur et local.

###### Utilisation :

Prérequi: génération de clé ssh entre la machine hote et cible.

Cloner mon répertoire :

`git clone https://github.com/Odka33/STAGE-Ansible`

Pour tester les scripts il suffit de modifier les variables "hosts" pour désigner les machines sur laquelles travailler ainsi que "remote_user" l'utilisateur de la machine qui va executer les tâches.

Ensuite placer vous dans le répertoire à tester et executer :

`ansible-playbook test_01.yaml --ask-sudo-pass`


 A venir :

 - Ajout de Playbook
 - Mise à jour du README.
 - Mise à jour des playbook de Base.
