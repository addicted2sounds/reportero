Be sure to clone the repository with submodules:
`git clone --recurse-submodules -j8 git@github.com:addicted2sounds/reportero.git`
In order to test on local machine, be sure to add corresponding entries to your `/etc/hosts`:
```
127.0.0.1       news.local repatridor.local mailcatcher.local
```
Copy file `.secrets.example` to `.secrets` and fill that with valid data.
Run `bin/setup` to build necessary images and import required data.

`news.local` service allow you to login/signup via linkedin or use regular email/password authentication.
`repatridor.local` is reponsible for results delivery. You can edit liquid templates for email at:
http://repatridor.local/admin/email_templates

`mailcatcher.local` catches all outgoing emails, so you can check those.
