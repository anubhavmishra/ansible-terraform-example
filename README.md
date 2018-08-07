# ansible-terraform-example
Example Ansible playbook to showcase the Terraform module.

## Usage

Run Ansible playbook

```bash
cd ansible-terraform-example/
```

```bash
ansible-playbook -i inventory/hosts main.yml
```

Expected output

```bash

PLAY [main] ****************************************************************************************************************************************************************************************************

TASK [plan] ****************************************************************************************************************************************************************************************************
 [WARNING]: Could not get Terraform outputs. This usually means none have been defined. stdout:  stderr: The state file either has no outputs defined, or all the defined outputs are empty. Please define an
output in your configuration with the `output` keyword and run `terraform refresh` for it to become available. If you are using interpolation, please verify the interpolated value is not empty. You can use
the  `terraform console` command to assist.

ok: [127.0.0.1]

TASK [apply] ***************************************************************************************************************************************************************************************************
changed: [127.0.0.1]

TASK [destroy] *************************************************************************************************************************************************************************************************
changed: [127.0.0.1]

PLAY RECAP *****************************************************************************************************************************************************************************************************
127.0.0.1                  : ok=3    changed=2    unreachable=0    failed=0
```
