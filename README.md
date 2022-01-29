Ansible-роль, настраивающая связку nginx+php-fpm и выдающая при обращении к главной странице веб-сервера информацию о php (содержимое index.php — <?php phpinfo();?>).

```
ansible-playbook playbook.yml -K
```
