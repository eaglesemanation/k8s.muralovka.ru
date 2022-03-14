# fluxcd

Installs FluxCD on a K8s cluster

## Requirements

Host needs to have access to K8s cluster

## Role Variables

| Variable                 | Description                                                           | Default Value |
| ------------------------ | --------------------------------------------------------------------- | ------------- |
| `fluxcd_state`           | State of FluxCD deployment: installed                                 | installed     |
| `fluxcd_git_url`         | Git repository URL                                                    | undefined     |
| `fluxcd_deployment_path` | Path relative to Git repository root used for cluster synchronization | undefined     |
| `fluxcd_ssh_key_file`    | Path to a private SSH key with write permissions to Git repository    | undefined     |

## Example Playbook

```yaml
- hosts: localhost
  roles:
    - role: eaglesemanation.fluxcd
```

## License

GPL 2.0 or later
