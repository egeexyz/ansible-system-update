# ansible-system-update
This is the code I wrote for the Ansible video I did a while ago. If you want to run it yourself, you'll need:

* Ansible 2.0 or greater (install it via python-pip)
* A server (or five) to run it against. Localhost works fine too.

Remember that you'll need to create the file `/etc/ansible/hosts` and add entries for the servers you want to run updates against. Read more about the hosts file [here](https://docs.ansible.com/ansible/latest/user_guide/intro_inventory.html).

Once you have added your hosts, update the `hosts:` entry in the `main.yml` with the name of your host, and then run `ansible-playbook main.yml`. If your host is running Ubuntu, Debian, CentOS, or openSUSE Leap, Ansible will begin updating your system!

Note: If your host is running some other Linux distribution, you will need to add a new task to the `main.yml` file. Read more about Ansible packing modules [here]().
