# ansible-jenkin

Jenkins Deployment on AWS

PREREQUISITES

- Two instances on AWS, one for the Agent machine and one for the JenkinsHost machine.

STEPS

- Log into the Agent machine via SSH and navigate to the folder that has been synchronized with rsync.

- Within the shared folder, locate the playbook files necessary for this project.

- Make sure you are in the shared folder directory and then run the following command:

    "ansible-playbook -v jenkins.yml -i inventory.txt"

- Once the command has completed execution, access the Jenkins application by using the JenkinsHost machine's public IP and entering it into your web browser, followed by ":8080" for port access.

- The Jenkins application will now be loaded in your browser.

Note: The above steps are meant to serve as a general guideline. Please ensure that you have a complete understanding of the setup and the commands being used before proceeding.

![Preview](./media/ansible.gif)