# Ansible Bootcamp Course prep README

This is the README file for the Ansible Bootcamp course preparation. This directory contains the playbooks and other files necessary to set up the environment which will be used for the course

# Course Requirements

These are the software and physical requirements to run the course - not the knowledge requirements which the students should have.

The course is by default run on a clean learning environment, which has been appropriately set up by the facilitators. This environment can take the form of a farm of VM's, physical machines (such as the learner's own laptop), etc. We only detail the case of a farm of VM's

## Dedicated, clean virtual machine

In order to complete the course, the learner should have ssh access to a dedicated virtual machine - it should not be shared with other people working on it, as this could cause issues, and confuse the learner unnecessarily. Depending on the use case for the bootcamp, the resource requirements of the VM may vary slightly, but a good common denominator is :

  * single CPU
  * 4 GB RAM
  * 120 GB disk

# Setting up the learning environment

The learning environment is created before the bootcamp is run, and it is assumed that all of the machines which are used by the learners are in the same state. In order to ensure this, we provide a playbook for creating this state. The tools necessary for  this are in the [Ansible](Ansible) subdirectory.

In order to set up the environment for a new bootcamp, you need to provide an inventory specific for the

## Learning environment playbook
