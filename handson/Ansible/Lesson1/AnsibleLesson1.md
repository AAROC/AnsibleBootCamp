# Ansible Lesson 1

This contains the lesson plan for lesson 1. In this lesson, we will discover Ansible, using it on the command line, trying to get familiar with the way in which it works, how it compares to "usual" system adminstration and configuration tasks on the command line, and exploring a few Ansible modules.

# Checklist : Basics

Follow the steps and tick off tasks as you complete them.

  1. [ ] Set up the repository
    1. [ ] Create the local directory where you will be working - start a repo :

            mkdir bootcamp
            cd bootcamp
            git init

    1. [ ] Create the repository on github. Ensure that `README` and `LICENSE` are present
    1. [ ] link it to your local repo (`git remote add origin ...`)
    1. [ ] synchronise (`git pull`, merge the two)

  1. [ ] Create your inventory
    1. [ ] Add localhost to the inventory
    1. [ ] Add a host variable which will describe how to connect to it. [Reference](http://docs.ansible.com/ansible/intro_inventory.html#non-ssh-connection-types)
  1. [ ] Check the facts
    1. [ ] Which python version do you have ? How did you find that out (which command gave you the response ? )
    1. [ ] Where is Ansible installed ?
    1. [ ] Which version of Ansible do you have ? How did you find that out ?

  1. [ ] Run Ansible ad-hoc discommands on the terminal
    1. [ ] Ensure that python2.7 is installed with `raw`
    1. [ ] Check that the host is responding : `ansible all -i <inventory> -m ping`
    1. [ ] ensure that `ansible` user is present
    1. [ ] ensure ssh key is generated
    1. [ ] ensure that ntp is installed and running
