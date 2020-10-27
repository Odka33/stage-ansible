# ANSIBLE

Depuis ici vous pouvez personaliser le lancement de ce playbook.

```ansible-playbook -i hosts site_d.yml --ask-sudo-pass ```


Il est possible de lancer les 3 playbooks sur un environnement débian 9.

- lamp classique.
- 1 allant mettre en place un site avec la page 404 de mon ancienne boite.
- de lancer les playbook avec wordpress en plus.
- de lancer un playbook avec synfony.

Les playbook vous mettre en place apache2 php mysql les vhost ainsi que d'autre tâche d'administration lié à debian et à la mise en place de site web et environnement de dévellopement.

Il est aussi possible de personnalisé de développement en changeant le contenus des fichiers racine yml "site" pour ajouter des roles à la suite.
