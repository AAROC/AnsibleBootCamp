# Bootcamp Checklist
<!-- TOC depthFrom:1 depthTo:6 withLinks:1 updateOnSave:1 orderedList:0 -->

- [Bootcamp Checklist](#bootcamp-checklist)
	- [How to use this Checklist](#how-to-use-this-checklist)
- [Initial discussion](#initial-discussion)
- [Just before the event](#just-before-the-event)
	- [Learners](#learners)
	- [Facilitators](#facilitators)
- [Checklist for <event name>](#checklist-for-event-name)

<!-- /TOC -->
This is an attempt at documenting the things necessary for the preparation of the Bootcamp. Inspired by [the Software Carpentry workshop operations checklist](http://software-carpentry.org/workshops/operations/).

## How to use this Checklist

These checklists are separated into tasks for learners and facilitators. The most important checklist is that of the [facilitator tasks](#facilitators) just prior to the event.

# Initial discussion

  1. In the weeks leading up to the event

    1. Reach out to participants
      - [ ]  Assessment - conduct a poll of knowledge and comfort with various technologies
      - [ ]  Decide on a use case
      - [ ]  Provide background learning materials
    1. Discuss the organisation
      - [ ]  Start a topic on the forum
      - [ ]  Secure funding and facilitators

  1. One month before the event
    - [ ]  Decide on the date and venue
    - [ ]  Set up the event page on indico
    - [ ]  Configure registration page


# Just before the event

In order to run the event successfully, the facilitators should be able to communicate efficiently with the learners, and the learning environmnet should be set up and configured for them.

## Learners

  - [ ]  Register attendees and collect necessary info in the checklist template below
  - Attendee checklist template.
    - [ ]  Github account name
    - SSH keys :
      - [ ]  [Add ssh key to your account](https://help.github.com/articles/adding-a-new-ssh-key-to-your-github-account/)
      - [ ]  Check that your key is publihsed at https://github.com/<username>.keys
    - [ ]  Join the [discussion forum](http://discourse.sci-gaia.eu) and log in
      - If your national federation is available:
        - select it; if  not : use one of the Catch-All federations (GrIDP, UbuntNet eduID, WACREN eduID)
      - if your institute's identity provider is available, use it to log in; if not, use the catch-all IdP of the federation.
      -  Report any issues to discourse-support@sci-gaia.eu


## Facilitators

Pre-event preparation starts here. For each event, create an issue in the repo for the event, and paste the checklist into it. Then, use this issue to track the development of the preparation, until it is closed on the day of the event.

Copy below this line
-----
```
# Checklist for <event name>

  - [ ]  Start the "getting to know you" topic on the forum.
  - [ ]  Build the learning environment:
      - [ ]  Deploy Virtual Machines - one per student and one each per facilitator.
      - [ ]  Add student ssh keys to the event
        - [ ]  student 1
        - [ ]  student 2
        - [ ]  etc
      - [ ]  Create your inventory file for the event. Add the learner machines to `training-lab` group.
			- [ ] Create the `group_vars` and passwords file. You will use this to save sensitive variables.
				- [ ] The group variables for the event should be created using the location of the event, e.g. `entebbe.yml`. Put this in `group_vars`
				- [ ] The passwords should have the same name, prefixed with "passwords-", _e.g._ : `passwords-entebbe.yml`
      - [ ]  Run the `training-lab.yml` playbook against the training lab group : `ansible-playbook -i inventories/<event-inventory>.ini -l training-lab training-lab.yml`
```
----
Copy above this line

### Using Ansible to build the lab

A playbook is provided for you to set up the lab.

### Feedback

- [ ] Ensure that there is some kind of feedback form.

# During the event

  - [ ] Ensure that the attendees have registered to the event so that you have a clear idea of who actually participated
	- [ ] Remind the attendees that there is feedback survey

## Day 1

  - [ ] Ensure that the slides are up to date
	- [ ] Checkup on the git lesson repos
		-	[ ] user 1
		- [ ] user n
	- [ ] Checkup on repo for the bootcamp
		- Lesson 1 :
			- Task 1 : Add inventory
			- Task 2 : Add group in inventory
			- Task 3 : Add `ansible.cfg`
		- Lesson 2 :
			- Task 1 : Playbook with basic plays, no  roles.

## Day 2

	- [ ] Don't forget to be Awesome.

# After the event

 - [ ]
