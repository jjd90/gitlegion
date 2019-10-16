The following is documentation on how to run the Ansible Playbook and the task that the playbook will perform.

1. In order to first run the playbook; Ansible must be installed on the server via the following commands (installation for Ubuntu):

          $ sudo apt update
          $ sudo apt install software-properties-common
          $ sudo apt-add-repository --yes --update ppa:ansible/ansible
          $ sudo apt install ansible
          
2. After installing Ansible copy/create the playbook.yml file onto the server in the desired location.

3. Run the following command to start the playbook. The steps for each task and its status will be displayed. 

4. The following task are performed by the Ansible Playbook.

        Tasks:
          - Installation of Apache2.
          - Start of Apache2 service.
          - Installation of PHP and its dependencies.
          - Restart of Apache 2 service.
          - Copying of the customized 000-default.conf file into the "/etc/apache2/sites-available" directory.
          - Copying of the index.html file into the "/var/www/html" directory.
          - Activation of the Apache2 SSL module.
          - Restart of the Apache2 service.
          
Note: CertBot must be ran after the playbook runs in order to generate the certificate for the webserver to run on port 443 (HTTPS).
