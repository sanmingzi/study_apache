# Config Ruby CGI on Apache2

- config root path

```sh
# /etc/apache2/sites-enabled/000-default.conf

DocumentRoot /workspace/study_javascript/demo/todo

<Directory /workspace/study_javascript/demo/todo>
        Options +ExecCGI
        AddHandler cgi-script .rb
        DirectoryIndex index.html
        Require all granted
</Directory>
```

- enable mod cgi

```sh
sudo ln -s /etc/apache2/mods-available/cgi.load /etc/apache2/mods-enabled/
```

- change your fire to excutable

```sh
sudo chmod -R 777 /workspace/study_javascript/demo/todo
```
