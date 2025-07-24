<a name="readme-top"></a>

![GitHub CI - Tests](https://github.com/FIAP-SOAT-G20/fiap-tech-challenge-3-api/actions/workflows/test.yml/badge.svg)

# <p align="center"><b>Fast Food</b> <small>FIAP Tech Challenge 4 - Infrastructure Deploy (k8s)</small></p>

<p align="center">
    <img src="https://img.shields.io/badge/Tools-Kubernetes-informational?style=flat-square&logo=kubernetes&color=326CE5" alt="Kubernetes" />
</p>

<p align="center">
    <img src="docs/gopher.png" alt="Fast Food" />
</p>

## 💬 About

Repository for the [FIAP](https://postech.fiap.com.br/) Tech Challenge 4, focused on developing a microservice backend system for managing orders in a fast-food restaurant.

This service is composed of an `API` and a `Worker` that consumes messages from an AWS SQS queue.  
The API is responsible for handling HTTP requests, while the worker processes messages from the queue, such as order creation and updates.

## 🔗 Related Projects

This project is part of a larger system that includes:

- [Customer Service](https://github.com/FIAP-SOAT-G20/tc4-customer-service)
- [Payment Service](https://github.com/FIAP-SOAT-G20/tc4-payment-service)
- [Kitchen Service](https://github.com/FIAP-SOAT-G20/tc4-kitchen-service)
- [Infrastructure - Deploy (k8s)](https://github.com/FIAP-SOAT-G20/tc4-infrastructure-deploy)
- [Infrastructure -Terraform](https://github.com/FIAP-SOAT-G20/tc4-infrastructure-tf)


## 📚 Dictionary - Ubiquitous Language

- Customer (actor): Actor responsible for initiating the purchasing process
- Cook (actor): Actor responsible for preparing the customer's order
- Attendant (actor): Actor responsible for interacting with the customer, providing support for the order
- Identification method: Format in which the customer is identified on the platform: via CPF or anonymous.
- Identification: Customer identification on the platform
- Authorization: Grants permission to the customer to perform operations on the platform, such as placing an order, changing registration information
- Order: Represents all items selected by the customer in the store
- Order Status: Represents the stage of order preparation after payment is confirmed.

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

- [Kubernete](https://kubernetes.io/)

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
