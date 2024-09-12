K3s Cluster Setup with Ansible 🚀
## Welcome to the K3s Cluster Setup project! 
This project helps you set up a K3s cluster using Ansible. It supports all M1 devices on Parallels Desktop and can also work for ARM devices. Please note that this project is a work in progress. 🛠️

### Prerequisites 📋
- Ansible installed on your local machine
- Parallels Desktop for M1 devices
- ARM devices (if applicable)
- SSH access to all nodes

### Project Structure 📂
- inventory.ini
- playbook.yml
- roles/
  - labels/
    - tasks/
      - main.yml
  - master/
    - tasks/
      - main.yml
  - prerequisites/
    - tasks/
      - main.yml
  - purge/
    - tasks/
      - main.yaml
  - worker/
    - tasks/
      - main.yml
- templates/
  - motd.j2

### How to Run the Project 🏃‍♂️
1. Clone the repository:
```
git clone https://github.com/your-repo/alpine-arm-k3s.git
```
2. Change directory to `alpine-arm-k3s`.
3. Update the inventory file:
   - Edit the `inventory.ini` file to match your environment.
4. Run the playbook:
```
ansible-playbook -i inventory.ini playbook.yml
```

### Contributing 🤝
We welcome contributions! Please read our [Contributing Guidelines](link-to-contributing-guidelines) for more details.

### License 📜
This project is licensed under the MIT License. See the `LICENSE` file for details.

