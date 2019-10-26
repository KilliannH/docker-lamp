install wordpress, make sure wordpress folder is owned by group www-data in php container.

in host sudo cmod 777 php/ -R for create / edit / delete container files without changing his group (www-data)

otherwise you'll keep doing "sudo chown {yout-user} /wordpress -R" from host
and "sudo chown www-data /wordpress -R" from your container
