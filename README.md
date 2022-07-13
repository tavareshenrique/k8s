<h1 align="center">
  <img alt="k8s" title="k8s" src="https://raw.githubusercontent.com/tavareshenrique/k8s/main/assets/logo.png?token=GHSAT0AAAAAABTQB6NN2KZCWOWQ22DZD52WYWPHXGA" width="180px" />
</h1>

<p align="center">
  <img alt="Last commit on GitHub" src="https://img.shields.io/github/last-commit/tavareshenrique/k8s?color=2e6ce7">
  <img alt="Made by Henrique Tavares" src="https://img.shields.io/badge/made%20by-Henrique Tavares-%20?color=2e6ce7">
  <img alt="Project top programing language" src="https://img.shields.io/github/languages/top/tavareshenrique/k8s?color=2e6ce7">
  <img alt="Repository size" src="https://img.shields.io/github/repo-size/tavareshenrique/k8s?color=2e6ce7">
  <img alt="GitHub license" src="https://img.shields.io/github/license/tavareshenrique/k8s?color=2e6ce7">
</p>

<p align="center">
  Esse projeto foi desenvolvido durante os meus estudos no curso <b><a href="https://www.udemy.com/course/orquestracao-de-containers-com-kubernetes/">Orquestração de Containers com Kubernetes.</a></b>
</p>

---


# :information_source: Comandos Úteis

## Geral

> **Rodando uma aplicação K8S:**

```bash
kubectl run nome-da-aplicacao
```

> **Pegando informações de um Cluster:**

```bash
kubctl cluster-info
```

> **Listando todos os `Nodes` da Aplicação:**
>> 💡 **Node:** Um node é uma máquina, física ou virtual, onde o Kubernetes está instalado.
```bash
kubectl get nodes
```

> **Pegando informações de um Cluster:**

```bash
kubctl cluster-info
```

> **Listando todos dados de um cluster**
```bash
kubectl get all
```

## Trabalhando com Pod's

> **Criando um Pod (Supondo que criemos um Pod para o `nginx`):**

```bash
kubectl run nginx --image nginx
```

> **Litando Pod's:**

```bash
kubectl get pods
```

> **Mais informações do Pod (O pod do `nginx` que criamos acima)**
```bash
kubectl describe pod nginx
```

> **Criando Pod a parti de um arquivo YAML**
```bash
kubectl create -f pod.yaml
```

> **Deletando Pod**
```bash
kubectl delete pod nginx-2
```

## Trabalhando com Deployments

>💡 Um deployment é um conjunto de pods que são criados a partir de um arquivo YAML, e a vantagem dele é que podemos já trabalhar com vários recursos ao mesmo tempo, como o ReplciaSet. 

> **Criando Deployments**
```bash
kubectl create -f deployment.yaml
```

> **Listando Deployments**
```bash
kubectl get deployments
```

> **Removendo Deployments**
```bash
kubectl delete deployment `<nome>`
```