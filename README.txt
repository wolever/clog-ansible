Manual setup:
- Create droplet, make sure your SSH key has root access
- Setup DNS
- SSH into your droplet and run:

    droplet $ apt-get update
    droplet $ apt-get install ansible

- Run `cp hosts-example.txt hosts`
- Edit `hosts`
- Run:

    $ ansible-playbook -i hosts [-l hostname] deploy.yaml
