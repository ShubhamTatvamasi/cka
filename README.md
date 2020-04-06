# cka

Be ready with 2 IDs at the time of exam

1. Passport
1. Debit card
> Second ID is only needed if your name is not in english on your first ID.

You are allowed only transparent drinks with transparent bottle during the exam.

Get comfortable using **vim** and **tmux** for exam, as you will only have one terminal.

**Multiple monitors usage is also allowed** — use one for k8s docs on 1 monitor and exam on the other monitor. ( you will be asked to share both screens ).


### Links which can be used during CKA Exam:

Resource | Link
--- | ---
Kubernetes Github | https://github.com/kubernetes/
Kubernetes Docs | https://kubernetes.io/docs/
Kubernetes Blog | https://kubernetes.io/blog/

---

### CKA Certification Exam Candidate Resources:

Resource | Link
--- | ---
CKA + CKAD Candidate Handbook | https://training.linuxfoundation.org/go/cka-ckad-candidate-handbook
CKA + CKAD Exam Tips | http://training.linuxfoundation.org/go//Important-Tips-CKA-CKAD
CKA + CKAD FAQ | http://training.linuxfoundation.org/go/cka-ckad-faq

Ref: https://training.linuxfoundation.org/cncf-certification-candidate-resources/

---

### CKA CLUSTERS

Cluster | Members | CNI | Description
--- | --- | --- | ---
k8s | 1 master, 2 worker | flannel | k8s cluster
hk8s | 1 master, 2 worker | calico | k8s cluster
bk8s | 1 master, 1 worker | flannel | k8s cluster
wk8s | 1 master, 2 worker | flannel | k8s cluster
ek8s | 1 master, 2 worker | flannel | k8s cluster
ik8s | 1 master, 1 base node | loopback | k8s cluster − missing worker node

> At the start of each task you'll be provided with the command to ensure you are on the correct cluster to complete the task.

---

### Certified Kubernetes Administrator (CKA) Exam Curriculum:

### https://github.com/cncf/curriculum

---

### Books to Read:

Books | Link
--- | ---
Kubernetes: Up and Running | https://azure.microsoft.com/en-in/resources/kubernetes-up-and-running
Managing Kubernetes | https://pages.cloud.vmware.com/managing-kubernetes-ebook
Kubernetes in Action | https://www.yunforum.net/pdf/kubernetes-in-action.pdf
Kubernetes The Hard Way (MUST READ) | https://github.com/kelseyhightower/kubernetes-the-hard-way

---

### Practice all Tasks & understand all Concepts:

Resource | Link
--- | ---
Kubernetes Tasks | https://kubernetes.io/docs/tasks/
Kubernetes Concepts | https://kubernetes.io/docs/concepts/

---

### Online Resources:

Resource | Link
--- | ---
The Kubernetes Learning Resources List | https://docs.google.com/spreadsheets/d/10NltoF_6y3mBwUzQ4bcQLQfCE1BWSgUDcJXy-Qp2JEU/view
CKA-Prep-List | https://docs.google.com/spreadsheets/d/1mYzfkxu1Iaup3KgO7zhbz7C4nFadSEvogo-lDaFIXK0/view

---

alias for doing things quickly
```bash
alias k='kubectl'

alias ke='k edit'

alias kd='k describe'

alias ka='k apply'
alias kaf='ka -f'

alias kdl='k delete'
alias kdlf='kdl -f'

alias kg='k get'
alias kga='kg all'
alias kgs='kg svc'
alias kgp='kg pods'
alias kgn='kg nodes'
alias kgd='kg deploy'
alias kgc='kg componentstatuses'

alias kc='k config'
alias kcg='kc get-contexts'
alias kcu='kc use-context'
alias kcc='kc current-context'
```
---

### Pro Tips (things to know before exam)

#### OpenSSL

comfortable generating certificates (.key, .crt, .csr, x509)

#### systemctl

managing services (status/start/stop/restart/enable/reload)

working with unit files (cat/show/edit)

#### journalctl

view logs for service
```bash
journalctl -u kubelet
```

#### kubectl command (create a Pod YAML spec)
```bash
kubectl run "pod_name" --image=nginx -o yaml --dry-run --generator=run-pod/v1 > save_to_pod_file.yml
```

#### kubectl command (create a Deployment YAML spec)
```bash
kubectl run "deployment_name" --image=nginx -o yaml --dry-run > save_to_deployment_file.yml
```

