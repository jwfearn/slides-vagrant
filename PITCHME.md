#HSLIDE

`requirements.yml`:
```yml
service_name: stranger_forces
stack_name: stranger_forces
image: avvo/stranger_forces
facing: internal
services:
  - account
  - content
  - gnomon
  - ledger
  - quasi
  - solicitor
health_check: false
```

#HSLIDE?gist=399e71331ae0b05db854331dafffa7cb
