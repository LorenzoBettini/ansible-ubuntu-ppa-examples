Some examples for installing Ubuntu software from PPAs.

First install the requirements:

```
ansible-galaxy install -r requirements.yml
```

```
ansible-playbook -i local -v playbook-ubuntu.yml -K
```

# Molecule testing

From the main directory

For checking idempotency

```
molecule test
```

To build an environment, have the playbook run inside it, then be able to log in and observe the environment, run:

```
molecule converge
```

And then, to log into the environment:

```
molecule login
```
