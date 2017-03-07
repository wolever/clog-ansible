Manual setup:

1. Create droplet, make sure your SSH key has root access
2. Setup DNS
3. From your droplet, run::

    apt-get update
    apt-get install ansible

4. Run ``cp hosts-example.txt hosts``
5. Edit ``hosts`` filling in your hostname and email (the other defaults are probably safe)
6. Run::

    ansible-playbook -i hosts deploy.yaml
