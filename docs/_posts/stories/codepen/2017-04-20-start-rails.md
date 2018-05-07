---
layout: post
categories: codepen
title: Start Rails
tags: [codepen]
---

### Create a new Rails project (or use an existing one) and enter the project directory from a terminal prompt.


```
http://www.caseincms.com/

https://github.com/russellquinn/casein
```

```
rails new caseinfo
cd ./caseinfo
```

```
source 'http://gems.ruby-china.org/'
bundle install
```

```
An error occurred while installing nio4r (2.0.0), and Bundler cannot continue.
Make sure that `gem install nio4r -v '2.0.0'` succeeds before bundling.

gem install nio4r -v '2.0.0'
gem install bindex -v '0.5.0'
gem install puma -v '3.8.2'
```

```
Bundle complete! 12 Gemfile dependencies, 56 gems now installed.
Use `bundle show [gemname]` to see where a bundled gem is installed.
```
成功

### Add the Casein gem to your Gemfile:

```
gem 'casein', '~>5.2.0'
```

```
An error occurred while installing scrypt (1.2.1), and Bundler cannot continue.
Make sure that `gem install scrypt -v '1.2.1'` succeeds before bundling.

Bundle complete! 13 Gemfile dependencies, 65 gems now installed.
Use `bundle show [gemname]` to see where a bundled gem is installed.
```
成功

### If you have just created a new project — and don't want to use the default SQLite settings — then remember to add your database details to /config/database.yml at this point.

### To enable Casein notification emails (used for new users and forgotten passwords) then add your SMTP server information to your initializers. For development, you can use something cool like MailCatcher (mailcatcher.me)

```
https://mailcatcher.me/

How

gem install mailcatcher
mailcatcher
Go to http://localhost:1080/
Send mail through smtp://localhost:1025
```
Please don't put mailcatcher into your Gemfile. It will conflict with your applications gems at some point.


```
$ mailcatcher
Starting MailCatcher
~~> ERROR: Something's using port 1025. Are you already running MailCatcher?
==> smtp://127.0.0.1:1025
==> http://127.0.0.1:1080
```


```
netstat -ano
tasklist|findstr 636

>> winint.exe 系统核心进程，不能强制关闭

```

```
$ mailcatcher --smtp-port 1030
Starting MailCatcher
==> smtp://127.0.0.1:1030
==> http://127.0.0.1:1080
```
成功 but see nothing.

Rails

To set up your rails app, I recommend adding this to your environments/development.rb:

```
config.action_mailer.delivery_method = :smtp
config.action_mailer.smtp_settings = { :address => "localhost", :port => 1025 }
```


### Install Casein configuration files into your project. This should not be run more than once without backing up or merging the generated files, as your customisations will be overwritten:


```
$ rails g casein:install
*** WARNING - Generating configuration files. Make sure you have backed up any files before overwriting them. ***
      create  app/helpers/casein/config_helper.rb
      create  app/views/casein/layouts/_tab_navigation.html.erb
      create  app/views/casein/layouts/_top_navigation.html.erb
 ** Overwrite if you haven't yet modified your robots.txt, otherwise add disallow rules for /casein and /admin manually **
    conflict  public/robots.txt
<o/public/robots.txt? (enter "h" for help) [Ynaqdh]

```

Y - yes, overwrite
n - no, do not overwrite
a - all, overwrite this and all others
q - quit, abort
d - diff, show the differences between the old and the new
h - help, show this help

没反应，跳过

由bash切换到cmd

```
D:\GitHub\caseinfo>rails g casein:install
*** WARNING - Generating configuration files. Make sure you have backed up any f
iles before overwriting them. ***
   identical  app/helpers/casein/config_helper.rb
   identical  app/views/casein/layouts/_tab_navigation.html.erb
   identical  app/views/casein/layouts/_top_navigation.html.erb
 ** Overwrite if you haven't yet modified your robots.txt, otherwise add disallo
w rules for /casein and /admin manually **
    conflict  public/robots.txt
<o/public/robots.txt? (enter "h" for help) [Ynaqdh] Y
       force  public/robots.txt
      create  app/assets/stylesheets/casein/custom.scss
      create  app/assets/javascripts/casein/custom.js
      create  app/assets/stylesheets/casein/auth_custom.scss
      create  app/assets/javascripts/casein/auth_custom.js
      create  db/migrate/20170422161546_casein_create_admin_users.rb
```


```
$ rake db:create
Created database 'db/development.sqlite3'
Created database 'db/test.sqlite3'
```

```
rake casein:users:create_admin email=you@yourdomain.com [password=your_password]
rake casein:users:create_admin email=zypper@126.com [password=start520cms]
```

```
$ rake casein:users:create_admin email=zypper@126.com [password=start520cms]
rake aborted!
ActiveRecord::StatementInvalid: Could not find table 'casein_admin_users'

Tasks: TOP => casein:users:create_admin
(See full trace by running task with --trace)
```
错误

```
$ rake casein:users:create_admin email=zypper@126.com [password=start520cms]
rake aborted!
Don't know how to build task '[password=start520cms]' (see --tasks)

(See full trace by running task with --trace)
[Casein] Created new admin user with username 'admin' and password 'b6747582a522a8dc8b10f67dfb528ba8'

```


```
bin/rails server
```

```
$ bin/rails db:migrate
== 20170422161546 CaseinCreateAdminUsers: migrating ===========================
-- create_table(:casein_admin_users, {})
   -> 0.0056s
== 20170422161546 CaseinCreateAdminUsers: migrated (0.0057s) ==================
```

问题比较多，重启电脑


Dear zh-dp,

A new user account has been created for you at:

http://0.0.0.0:3000/casein

Username: zhang
Password: ed2ebf23c486244a6ee44b5605add1cf

From

Casein

参考

```
http://guides.rubyonrails.org/getting_started.html#creating-the-blog-application

http://www.caseincms.com/


https://github.com/russellquinn/casein


https://mailcatcher.me/


https://rubygems.org/gems/mailcatcher/versions/0.6.4


```


