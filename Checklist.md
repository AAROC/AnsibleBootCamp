# Bootcamp Checklist

This is an attempt at documenting the things necessary for the preparation of the Bootcamp. Inspired by [the Software Carpentry workshop operations checklist](http://software-carpentry.org/workshops/operations/)

  1. In the weeks leading up to the event

    1. Reach out to participants
      - [] Assessment - conduct a poll of knowledge and comfort with various technologies
      - [] Decide on a use case
      - [] Provide background learning materials
    1. Discuss the organisation
      - [] Start a topic on the forum
      - [] Secure funding and facilitators

  1. One month before the event
    - [] Decide on the date and venue
    - [] Set up the event page on indico
    - [] Configure registration page


# Just before the event

  - [] Register attendees and collect necessary info in the checklist template below
  - Attendee checklist template.
    - [] Github account name
    - * SSH keys :
        * [] [Add ssh key to your account](https://help.github.com/articles/adding-a-new-ssh-key-to-your-github-account/)
        * [] Check that your key is publihsed at https://github.com/<username>.keys
  - [] Build the learning environment:
      - [] Deploy Virtual Machines - one per student and one each per facilitator.
      - [] Create your inventory file for the event. Add the learner machines to `training-lab` group.
      - [] Run the `training-lab.yml` playbook against the training lab group : `ansible-playbook -i inventories/<event-inventory>.ini -l training-lab training-lab.yml`
