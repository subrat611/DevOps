## Table of contents

- [What is YAML](#what-is-yaml)
- [Docker](#docker)
- [Docker Runtime](#docker-runtime)
- [Docker Container Image](#docker-container-image)

---

## What is YAML

- YAML - YAML Ain't Markup Language
- YAML is a human-readable data serialization format that is often used for configuration files, data exchange between languages, and defining structured data.

> Data Serialization
>
> Is the process of converting structured data into a format that can be easily stored, transmitted, or reconstructed later. It involves representing the data in a standardized and platform-independent manner.
>
> When data is serialized, its structure and values are converted into a sequence/stream of bytes or characters that can be written to a file, transmitted over a network, or stored in a database. This serialized representation can be later deserialized, or reconstructed, to retrieve the original data structure and values.
>
> Other commonly used serialization formats include JSON (JavaScript Object Notation), XML (eXtensible Markup Language), and Protocol Buffers.

- YAML files are commonly used in conjunction with tools and frameworks like Ansible, Kubernetes, Docker Compose, and CI/CD (Continuous Integration/Continuous Deployment) systems like Jenkins or GitLab CI/CD.

- ```YAML
  name: John Smith
  age: 30
  address:
    street: 123 Main Street
    city: Anytown
    country: USA
  skills:
    - Python
    - Docker
    - Kubernetes
  ```

- YAML is collection of documents
- document are separate with --- and ending with ...

```yml
# lists
- apple
- mango
- banana
---
# key value
cities:
  - new delhi
  - mumbai
  - jaipur
---
"apple": "I am a fruit"
1: "I am a Id"
```

### Where it is used?

- Configuration files
- Infrastructure as Code (IaC) - Kubernetes, Docker Compose, or Ansible
- Continuous Integration/Continuous Deployment (CI/CD)
- Data interchange

### Benefits

- Simple and easy to read
- It has a strict syntax (indentation)
- Easily converted to JSON, XML
- Most languages use YAML
- More powerful when representing complex data
- Parsing is easy i.e reading is easy

## Sparse sequence

- A sparse sequence refers to a list or array where the elements are not necessarily contiguous or consecutive. It allows you to have gaps or missing elements within a sequence.

```yml
fruits:
  - apple
  -
  - orange
  -
  - banana
```

🚀[Back to top](#table-of-contents)

---

## Docker

- A container is a lightweight and isolated runtime environment that packages an application and its dependencies together.

- Ensuring that they work the same way across different systems.

- Containers utilize operating system-level virtualization to isolate processes and resources, allowing multiple containers to run on a single host machine.

<img src="https://www.docker.com/wp-content/uploads/2021/11/docker-containerized-and-vm-transparent-bg.png" />

- Containers provide a lightweight and efficient way to package and run applications, sharing the host kernel and resources. They offer portability, scalability, and a rich ecosystem of tools. Virtual machines, on the other hand, provide stronger isolation but come with higher resource overhead and slower startup times.

## Docker Runtime

- It start/stop the containers. Docker run time refers to the duration or execution time of a Docker container. It represents the period during which a container is running and performing its designated tasks.

<img src="https://www.docker.com/wp-content/uploads/2021/10/Docker-Website-2018-Diagrams-071918-V5_a-Docker-Engine-page-first-panel.png" />

- Also known as runc.

- **containerd** manage the **runc**. Containerd is an open-source container runtime that provides a lightweight and consistent interface for managing container lifecycle, image management, and low-level container runtime operations

- **Orchestration** in Docker refers to the management and coordination of multiple Docker containers within a distributed system. It involves automating various tasks related to container deployment, scaling, networking, and service discovery to ensure the efficient and reliable operation of containerized applications.

## Docker Container Image

- A Docker container image is a lightweight, standalone, and executable software package that includes everything needed to run a piece of software, including the code, runtime, system tools, libraries, and dependencies. `It is the building block for creating and running Docker containers.`

- A Docker image is created based on a specific configuration defined in a Dockerfile, which specifies the instructions for building the image.

- The Dockerfile typically includes details such as the base image, application code, environment variables, network ports, and any additional software or configurations required.

- **`Docker file -> Image -> Container`**
- Think in oops Image is **Class** and container is **Object**

🚀[Back to top](#table-of-contents)

---
