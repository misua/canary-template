
# Gateway API in GKE

Purpose of this is to use gw api, to replace ingress + svc mesh, to provision and use 1 load balancer for all environments, Live,dev and canary, saving load balancer costs

#### gatewayClassName: gke-l7-global-external-managed

`needed gatewayClassName to be able to do cross namespace routing in GKE`


#### Namespace live-store

`This is where the "Live" site will run in /live if merged from dev`


#### Namespace dev

`this is where the "dev" site will run in /dev if deployed/merged from feature/branch`


#### Canary deployment scenario wherein you are rolling out new features `(slowly / by weight)`


### TODO
`considering using flagger or argo rollouts/argo cd for drift detection`
`setting up prometheus+grafana+ loki to completely cover and monitor ALL deployments`

---

## Authors

- [@misua](https://www.github.com/misua)



`Badges`


[![MIT License](https://img.shields.io/badge/License-MIT-green.svg)](https://choosealicense.com/licenses/mit/)
[![GPLv3 License](https://img.shields.io/badge/License-GPL%20v3-yellow.svg)](https://opensource.org/licenses/)
[![AGPL License](https://img.shields.io/badge/license-AGPL-blue.svg)](http://www.gnu.org/licenses/agpl-3.0)

![Terraform](https://img.shields.io/badge/terraform-%235835CC.svg?style=for-the-badge&logo=terraform&logoColor=white)
![Static Badge](https://img.shields.io/badge/Charles-Pogi-blue)

## Network infrastructure overview



![Logo](https://github.com/misua/progressive-deployment-template/blob/main/base.drawio.png)




