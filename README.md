# Krateo Blueprints Marketplace

Welcome to the **Krateo Blueprints Marketplace** – the central hub where you can discover, request, and contribute to reusable infrastructure components built as Helm Charts.

> 🧭 **This repository acts as the Helm Registry for the Blueprint Marketplace.**  
> It **lists all available Blueprints** and provides links to the **dedicated repositories** where each Blueprint is implemented and maintained.

---

## 📦 What is a Blueprint?

A **Blueprint** is a reusable Helm Chart that includes a `values.schema.json` file. This schema allows Krateo to automatically generate user-friendly forms and validation rules in the Krateo Composable Portal, making complex configurations accessible and safe.

Here’s how it works:
- If a Helm Chart **already exists but lacks a schema**, we wrap it in a new chart that includes it as a dependency and add the `values.schema.json` file.
- Every Blueprint (also referred to as a *Composition*) is designed to be:
  - **Composable** – can be combined with others
  - **Declarative** – clear and configuration-driven
  - **Reusable** – works across multiple environments and use cases

---

## 🗂 Blueprint Categories

Blueprints are organized by purpose into the following categories:

| Category   | Description                                                                 | Examples                                                                 |
|------------|-----------------------------------------------------------------------------|--------------------------------------------------------------------------|
| **Portal** | Blueprints related to the Krateo user interface and experience              | UI components, dashboard extensions, approval flows                     |
| **Operations** | Blueprints that support day-to-day platform operations                    | ArgoCD, external secrets management, cluster tooling                    |
| **FinOps** | Blueprints for cost tracking, reporting, and optimization                   | Resource usage dashboards, quota controllers                            |
| **Generator** | Blueprints that dynamically generate Kubernetes controllers from OpenAPI schemas | Controller generators, API-handling middlewares                          |


Each Blueprint will be listed under one of these categories with:
- A short description
- A link to its implementation repository
- A Helm chart reference (as part of this registry)

---

## 📘 Available Blueprints

<!-- Available Blueprints START -->
| Blueprint Name | Blueprint Version | Blueprint Category | Blueprint Repository | Blueprint Description |
|----------------|-------------------|---------------------|-----------------------|------------------------|
| github-scaffolding | [0.0.1](https://github.com/krateoplatformops-blueprints/github-scaffolding/tree/0.0.1) | operations | [https://github.com/krateoplatformops-blueprints/github-scaffolding](https://github.com/krateoplatformops-blueprints/github-scaffolding) | This is a template used to scaffold a toolchain to host and deploy a fully functional frontend App. This Template implements the following steps: - Create an empty Github repository (on github.com) - Push the code from the skeleton to the previously create repository - A Continuous Integration pipeline (GitHub workflow) will build the Dockerfile of the frontend app and the resulting image will be published as a Docker image on the GitHub Package registry - An ArgoCD Application will be deployed to listen to the Helm Chart of the frontend app and deploy the chart on the same Kubernetes cluster where ArgoCD is hosted - The frontend App will be deployed with a Service type of NodePort kind exposed on the chosen port.  |
| portal | [0.0.1](https://github.com/krateoplatformops-blueprints/portal/tree/0.0.1) | portal | [https://github.com/krateoplatformops-blueprints/portal](https://github.com/krateoplatformops-blueprints/portal) | A Blueprint for Krateo Composable Portal |
| portal-blueprint-page | [0.0.1](https://github.com/krateoplatformops-blueprints/portal-blueprint-page/tree/0.0.1) | portal | [https://github.com/krateoplatformops-blueprints/portal-blueprint-page](https://github.com/krateoplatformops-blueprints/portal-blueprint-page) | A Blueprint for Krateo Composable Portal Blueprint page |
| portal-composition-page-generic | [0.0.1](https://github.com/krateoplatformops-blueprints/portal-composition-page-generic/tree/0.0.1) | portal | [https://github.com/krateoplatformops-blueprints/portal-composition-page-generic](https://github.com/krateoplatformops-blueprints/portal-composition-page-generic) | A Blueprint for Krateo Composable Portal Composition page with a generic approach |
<!-- Available Blueprints END -->

---

## ✨ How to Contribute

We’d love your help in growing and improving the Blueprint Marketplace!

You can:
- 🔧 **Request a new Blueprint** for something not yet available
- 📥 **Suggest improvements** to an existing Blueprint
- 🐛 **Report issues** with the behavior or structure of current Blueprints

To get started, open one of the following issues:

- [🚀 Feature Request](../../issues/new?assignees=&labels=enhancement&template=feature_request.yml) — Propose a new Blueprint or improvement  
- [🐞 Report an Issue](../../issues/new?assignees=&labels=bug&template=report_composition_issue.yml) — Report a bug or problem with an existing Blueprint

---

## 📁 What’s in This Repository?

This repository acts as both a Helm Registry and a coordination point for the Marketplace. Here you'll find:

- ✅ A categorized list of available Blueprints
- 🔗 Links to their source repositories
- 📌 Templates to propose new ideas or report problems

---

## 📄 License

This repository is open source and available under the [Apache 2.0 License](LICENSE).
