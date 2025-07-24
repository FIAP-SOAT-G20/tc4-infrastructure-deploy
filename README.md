<a name="readme-top"></a>

# <p align="center"><b>Fast Food</b> <small>FIAP Tech Challenge 4 - Infrastructure Deploy (k8s)</small></p>

<p align="center">
    <img src="https://img.shields.io/badge/Tools-Kubernetes-informational?style=flat-square&logo=kubernetes&color=326CE5" alt="Kubernetes" />
</p>

<p align="center">
    <img src="docs/gopher.png" alt="Fast Food" />
</p>

## 💬 About

Repository for the [FIAP](https://postech.fiap.com.br/) Tech Challenge 4, focused on deploying a microservices architecture using Kubernetes.

## 🔗 Related Projects

This project is part of a larger system that includes:

- [Customer Service](https://github.com/FIAP-SOAT-G20/tc4-customer-service)
- [Order Service](https://github.com/FIAP-SOAT-G20/tc4-order-service)
- [Payment Service](https://github.com/FIAP-SOAT-G20/tc4-payment-service)
- [Kitchen Service](https://github.com/FIAP-SOAT-G20/tc4-kitchen-service)
- [Infrastructure -Terraform](https://github.com/FIAP-SOAT-G20/tc4-infrastructure-tf)

## 🏗️ Architecture

### K8s

![k8s](docs/k8s.jpg)

### :open_file_folder: Project Structure

```sh
.
├── configs
├── ingress
├── namespace
└── services
    ├── customer-service
    ├── kitchen-service
    │   ├── api
    │   └── worker
    ├── order-service
        ├── api
        └── worker
```

<p align="right">(<a href="#readme-top">back to top</a>)</p>


## :computer: Technologies

- [Kubernetes](https://kubernetes.io/)

## :scroll: Requirements

- Kubernetes cluster (minikube, kind, EKS, etc.)
- [kubectl CLI](https://kubernetes.io/docs/tasks/tools/)
- [AWS CLI](https://aws.amazon.com/cli/)

<p align="right">(<a href="#readme-top">back to top</a>)</p>

## :cd: Installation

```sh
git clone https://github.com/FIAP-SOAT-G20/tc4-infrastructure-deploy
```

```sh
cd tc4-infrastructure-deploy
```

<p align="right">(<a href="#readme-top">back to top</a>)</p>

## :runner: Running

```sh
make aws-eks-auth
```

```sh
make k8s-apply
```

<p align="right">(<a href="#readme-top">back to top</a>)</p>

## :clap: Acknowledgments

- [Kubernetes](https://kubernetes.io/)

<p align="right">(<a href="#readme-top">back to top</a>)</p>

## :busts_in_silhouette: Contributors

<div align="center">
  <table>
    <tbody>
      <tr>
        <td align="center" valign="top" width="14.28%"><a href="https://github.com/atomaz"><img src="https://github.com/atomaz.png" width="100px;" alt=""/><br /><sub><b>Alice Tomaz</b></sub></a><br />
        <td align="center" valign="top" width="14.28%"><a href="https://github.com/filipe1309"><img src="https://github.com/filipe1309.png" width="100px;" alt=""/><br /><sub><b>Filipe Bonfim</b></sub></a><br />
        <td align="center" valign="top" width="14.28%"><a href="https://github.com/hugokishi"><img src="https://github.com/hugokishi.png" width="100px;" alt=""/><br /><sub><b>Hugo Kishi</b></sub></a><br />
        <td align="center" valign="top" width="14.28%"><a href="https://github.com/marcos-nsantos"><img src="https://github.com/marcos-nsantos.png" width="100px;" alt=""/><br /><sub><b>Marcos Santos</b></sub></a><br />
        <td align="center" valign="top" width="14.28%"><a href="https://github.com/th3r4ven"><img src="https://github.com/th3r4ven.png" width="100px;" alt=""/><br /><sub><b>Matheus</b></sub></a><br />
      </tr>
    </tbody>
  </table>
</div>

<p align="right">(<a href="#readme-top">back to top</a>)</p>
