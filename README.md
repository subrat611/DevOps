## Table of contents

- [What is YAML](#what-is-yaml)

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
...
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

🚀[Back to top](#table-of-contents)
