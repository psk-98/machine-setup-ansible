# Machine Setup Ansible

Ansible playbook to set up a laptop with tools I use

## Usage

```bash
ansible-playbook debian-laptop.yml
```

Run with specific tags:
```bash
ansible-playbook laptop.yml --tags "bun,docker"
```

## Tags

Use tags to run specific parts of the playbook:

- `packages` - Core apt packages
- `nvm` / `node` - Node.js via nvm
- `docker` - Docker installation
- `github-cli` / `gh` - GitHub CLI
- `hashicorp` - Vault, Terraform, Packer
- `kubectl` - Kubernetes CLI
- `chrome` - Google Chrome
- `microsoft` - VS Code, Edge
- `snap` - Snap packages
- `flatpak` - Flatpak packages
- `updates` - System update/upgrade
