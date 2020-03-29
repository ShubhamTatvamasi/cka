# cka

Be ready with 2 IDs at the time of exam

1. Passport
1. Debit card
> Second ID is only needed if your name is not in english on your first ID.

You are allowed only transparent drinks with transparent bottle during the exam.

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


---

alias for doing things quickly
```bash
alias k='kubectl'

alias ke='k edit'

alias kd='k describe'

alias kdl='kubectl delete'
alias kdlf='kubectl delete -f'

alias kg='k get'
alias kga='k get all'
alias kgs='k get svc'
alias kgp='k get pods'
alias kgn='k get nodes'
alias kgd='k get deploy'
alias kgc='k get componentstatuses'

alias kcg='k config get-contexts'
alias kcu='k config use-context'
alias kcc='k config current-context'
```
---

### Pro Tips (things to know before exam)

#### OpenSSL

comfortable generating certificates (.key, .crt, .csr, x509)

#### systemctl

managing services (status/start/stop/restart/enable/reload)

working with unit files (cat/show/edit)

#### journalctl

view logs for service (journalctl -u kubelet)

#### kubectl command (create a Pod YAML spec)
```bash
kubectl run "pod_name" --image=nginx -o yaml --dry-run --generator=run-pod/v1 > save_to_pod_file.yml
```

#### kubectl command (create a Deployment YAML spec)
```bash
kubectl run "deployment_name" --image=nginx -o yaml --dry-run > save_to_deployment_file.yml
```
---

### Bookmarks for exam

Resource | Link
--- | ---
Conventions | https://kubernetes.io/docs/reference/kubectl/conventions/
