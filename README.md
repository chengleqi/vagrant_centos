## Vagrant Command

```bash
# manages boxes: installation
vagrant box add centos/7 LocalBoxPath
```

```bash
# initializes a new Vagrant environment by creating a Vagrantfile
vagrant init centos/7
```

```bash
# starts and provisions the vagrant environment
vagrant up
```

```bash
# suspends the machine
vagrant suspend
```

```bash
# resume a suspended vagrant machine
vagrant resume
```

```bash
# stops the vagrant machine
vagrant halt
```

```bash
# stops and deletes all traces of the vagrant machine
vagrant destroy
```

```bash
# restarts vagrant machine, loads new Vagrantfile configuration
vagrant reload
```

```bash
# connects to machine via SSH
vagrant ssh
```

## Materials

- [vagrant boxes](https://app.vagrantup.com/boxes/search)

- [a great Vagrant Crash Course on youtube](https://youtu.be/vBreXjkizgo)