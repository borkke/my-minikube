Error log from `init` container
>disable Setup Wizard/var/jenkins_config/apply_config.sh: 4: /var/jenkins_config/apply_config.sh: cannot create /var/jenkins_home/jenkins.install.UpgradeWizard.state: Permission denied

Reproducing issue
```bash
kubectl create namespace jenkins
helm install minikube . -n jenkins
```