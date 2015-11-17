# Ansible project to manage Jenkins

[jenkins URL](https://ci.beta.digitalmarketplace.service.gov.uk/)

We use Jenkins job builder for managing jobs. The best documentation for this is [here](https://jenkins-job-builder.readthedocs.org/en/latest/index.html)

## To setup

* Create a virtualenv and pip install
* You may need to deactivate and reactivate the virtualenv before the `ansible-playbook` command is available.



## To deploy

Run all ansible tasks
```bash
$ ./scripts/provision.sh <path to digitalmarketplace-credentials>
````

Run just tasks tagged as `jobs`
```bash
$ ./scripts/provision.sh <path to digitalmarketplace-credentials> -t jobs
```