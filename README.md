# cka

Be ready with 2 IDs at the time of exam

1. Passport
1. Debit card


### Links which can be used during CKA Exam:

Resource | Link
--- | ---
Kubernetes Github | https://github.com/kubernetes/
Kubernetes Docs | https://kubernetes.io/docs/
Kubernetes Blog | https://kubernetes.io/blog/

---

### CKA Practice Labs & Tasks:

Kubernetes practice tasks https://www.katacoda.com/courses/kubernetes

Kubernetes Tasks https://kubernetes.io/docs/tasks/

practice environment similar to the actual exam https://github.com/arush-sal/cka-practice-environment


### CKA Certification Exam Candidate Resources

Resource | Link
--- | ---
CKA + CKAD Candidate Handbook | https://training.linuxfoundation.org/go/cka-ckad-candidate-handbook
CKA + CKAD Exam Tips | http://training.linuxfoundation.org/go//Important-Tips-CKA-CKAD
CKA + CKAD FAQ | http://training.linuxfoundation.org/go/cka-ckad-faq

Ref: https://training.linuxfoundation.org/cncf-certification-candidate-resources/

---

### Certified Kubernetes Administrator (CKA) Exam Curriculum:

https://github.com/cncf/curriculum

---

### Books to Read:

Books | Link
--- | ---
Kubernetes: Up and Running | https://azure.microsoft.com/en-in/resources/kubernetes-up-and-running
Managing Kubernetes | https://pages.cloud.vmware.com/managing-kubernetes-ebook
Kubernetes in Action |
Kubernetes The Hard Way (MUST READ) | https://github.com/kelseyhightower/kubernetes-the-hard-way

---

### Important links

[The Kubernetes Learning Resources List](https://docs.google.com/spreadsheets/d/10NltoF_6y3mBwUzQ4bcQLQfCE1BWSgUDcJXy-Qp2JEU/view)

Certified Kubernetes Administrator: https://www.cncf.io/certification/cka/

Exam Curriculum (Topics): https://github.com/cncf/curriculum

Exam Tips: http://training.linuxfoundation.org/go//Important-Tips-CKA-CKAD

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

### Generators v1.17

Resource | API group | kubectl command
--- | --- | ---
Pod	| v1	| kubectl run --generator=run-pod/v1
ReplicationController (deprecated)	| v1	| kubectl run --generator=run/v1
Deployment (deprecated)	| extensions/v1beta1	| kubectl run --generator=deployment/v1beta1
Deployment (deprecated)	| apps/v1beta1	| kubectl run --generator=deployment/apps.v1beta1
Job (deprecated)	| batch/v1	| kubectl run --generator=job/v1
CronJob (deprecated)	| batch/v2alpha1	| kubectl run --generator=cronjob/v2alpha1
CronJob (deprecated)	| batch/v1beta1	| kubectl run --generator=cronjob/v1beta1

Reference: https://kubernetes.io/docs/reference/kubectl/conventions/
