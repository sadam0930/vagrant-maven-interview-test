A vagrant environment with centOS 7, Java 8, and Maven 3.5

To run:
1. Download and install virtualbox and vagrant for your OS
2. From a command line run 
    1. `vagrant box add viniciusfs/centos7 https://atlas.hashicorp.com/viniciusfs/boxes/centos7/`
    2. choose virtualbox as the provider
    3. Clone the repo into some directory on your computer: https://github.com/sadam0930/vagrant-maven-interview-test
    4. cd into the directory that was cloned
    5. Run `vagrant up && vagrant ssh`
3. After several minutes this should terminate without errors (a bunch of red in the middle is ok and expected). You should now be in the virtual machine and see `vagrant@localhost` in the cmd line
4. Run`cd /vagrant`
5. Run `ls -la`
6. Notice that the file hello from the repository is listed here. You can edit the files on your local file system and see them in the vagrant VM.
7. Complete the tutorial from https://maven.apache.org/guides/getting-started/maven-in-five-minutes.html
8. When finished run`exit` and then `vagrant halt`