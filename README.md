# A small Rails/Sinatra/rack-ready playbook for Ansible

It installs:

- nginx
- Puma (jungle)
- Ruby 2.0.0-p247
- PostgreSQL
- memcached
- Redis (for Sidekiq)

Change the app name, host and deploy directory in `vars/defaults.yml`

To run:

Create the Vagrant box:
  
    $ vagrant up

Then run the Ansible playbook:

    $ ansible-playbook ruby-webapp.yml -i hosts
