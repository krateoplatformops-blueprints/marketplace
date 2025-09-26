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
| Blueprint Name | Blueprint Version | Blueprint Category | Krateo Supported Version | Blueprint Repository |
|----------------|-------------------|--------------------|---------------------------|-----------------------|
| azure-pricing-finops | [0.1.0](https://github.com/krateoplatformops-blueprints/azure-pricing-finops/tree/0.1.0) | <ul><li>finops</li></ul> | >= 2.5.1 | [https://github.com/krateoplatformops-blueprints/azure-pricing-finops](https://github.com/krateoplatformops-blueprints/azure-pricing-finops) |
| finops-azure-configuration | [1.0.0](https://github.com/krateoplatformops-blueprints/azure-configuration-finops/tree/1.0.0) | <ul><li>portal</li><li>finops</li></ul> | >= 2.5.1 | [https://github.com/krateoplatformops-blueprints/azure-configuration-finops](https://github.com/krateoplatformops-blueprints/azure-configuration-finops) |
| github-provider-kog | [1.0.0](https://github.com/krateoplatformops-blueprints/github-provider-kog/tree/1.0.0) | <ul><li>generator</li></ul> | >= 2.5.1 | [https://github.com/krateoplatformops-blueprints/github-provider-kog](https://github.com/krateoplatformops-blueprints/github-provider-kog) |
| github-provider-kog-collaborator | [1.0.0](https://github.com/krateoplatformops-blueprints/github-provider-kog/tree/main/github-provider-kog-collaborator-blueprint/tree/1.0.0) | <ul><li>generator</li></ul> | >= 2.5.1 | [https://github.com/krateoplatformops-blueprints/github-provider-kog/tree/main/github-provider-kog-collaborator-blueprint](https://github.com/krateoplatformops-blueprints/github-provider-kog/tree/main/github-provider-kog-collaborator-blueprint) |
| github-provider-kog-repo | [1.0.0](https://github.com/krateoplatformops-blueprints/github-provider-kog/tree/main/github-provider-kog-repo-blueprint/tree/1.0.0) | <ul><li>generator</li></ul> | >= 2.5.1 | [https://github.com/krateoplatformops-blueprints/github-provider-kog/tree/main/github-provider-kog-repo-blueprint](https://github.com/krateoplatformops-blueprints/github-provider-kog/tree/main/github-provider-kog-repo-blueprint) |
| github-provider-kog-runnergroup | [1.0.0](https://github.com/krateoplatformops-blueprints/github-provider-kog/tree/main/github-provider-kog-runnergroup-blueprint/tree/1.0.0) | <ul><li>generator</li></ul> | >= 2.5.1 | [https://github.com/krateoplatformops-blueprints/github-provider-kog/tree/main/github-provider-kog-runnergroup-blueprint](https://github.com/krateoplatformops-blueprints/github-provider-kog/tree/main/github-provider-kog-runnergroup-blueprint) |
| github-provider-kog-teamrepo | [1.0.0](https://github.com/krateoplatformops-blueprints/github-provider-kog/tree/main/github-provider-kog-teamrepo-blueprint/tree/1.0.0) | <ul><li>generator</li></ul> | >= 2.5.1 | [https://github.com/krateoplatformops-blueprints/github-provider-kog/tree/main/github-provider-kog-teamrepo-blueprint](https://github.com/krateoplatformops-blueprints/github-provider-kog/tree/main/github-provider-kog-teamrepo-blueprint) |
| github-provider-kog-workflow | [1.0.0](https://github.com/krateoplatformops-blueprints/github-provider-kog/tree/main/github-provider-kog-workflow-blueprint/tree/1.0.0) | <ul><li>generator</li></ul> | >= 2.5.1 | [https://github.com/krateoplatformops-blueprints/github-provider-kog/tree/main/github-provider-kog-workflow-blueprint](https://github.com/krateoplatformops-blueprints/github-provider-kog/tree/main/github-provider-kog-workflow-blueprint) |
| github-scaffolding | [1.0.0](https://github.com/krateoplatformops-blueprints/github-scaffolding/tree/1.0.0) | <ul><li>operations</li></ul> | >= 2.5.1 | [https://github.com/krateoplatformops-blueprints/github-scaffolding](https://github.com/krateoplatformops-blueprints/github-scaffolding) |
| github-scaffolding-with-composition-page | [1.0.0](https://github.com/krateoplatformops-blueprints/github-scaffolding-with-composition-page/tree/1.0.0) | <ul><li>operations</li><li>portal</li></ul> | >= 2.5.1 | [https://github.com/krateoplatformops-blueprints/github-scaffolding-with-composition-page](https://github.com/krateoplatformops-blueprints/github-scaffolding-with-composition-page) |
| portal | [1.0.0](https://github.com/krateoplatformops-blueprints/portal/tree/1.0.0) | <ul><li>portal</li></ul> | >= 2.5.1 | [https://github.com/krateoplatformops-blueprints/portal](https://github.com/krateoplatformops-blueprints/portal) |
| portal-admin-page | [1.0.0](https://github.com/krateoplatformops-blueprints/portal-admin-page/tree/1.0.0) | <ul><li>portal</li></ul> | >= 2.5.1 | [https://github.com/krateoplatformops-blueprints/portal-admin-page](https://github.com/krateoplatformops-blueprints/portal-admin-page) |
| portal-blueprint-page | [1.0.5](https://github.com/krateoplatformops-blueprints/portal-blueprint-page/tree/1.0.5) | <ul><li>portal</li></ul> | >= 2.6.0 | [https://github.com/krateoplatformops-blueprints/portal-blueprint-page](https://github.com/krateoplatformops-blueprints/portal-blueprint-page) |
| portal-blueprint-page | [1.0.4](https://github.com/krateoplatformops-blueprints/portal-blueprint-page/tree/1.0.4) | <ul><li>portal</li></ul> | >= 2.6.0 | [https://github.com/krateoplatformops-blueprints/portal-blueprint-page](https://github.com/krateoplatformops-blueprints/portal-blueprint-page) |
| portal-blueprint-page | [1.0.3](https://github.com/krateoplatformops-blueprints/portal-blueprint-page/tree/1.0.3) | <ul><li>portal</li></ul> | >= 2.5.1 | [https://github.com/krateoplatformops-blueprints/portal-blueprint-page](https://github.com/krateoplatformops-blueprints/portal-blueprint-page) |
| portal-blueprint-page | [1.0.2](https://github.com/krateoplatformops-blueprints/portal-blueprint-page/tree/1.0.2) | <ul><li>portal</li></ul> | >= 2.5.1 | [https://github.com/krateoplatformops-blueprints/portal-blueprint-page](https://github.com/krateoplatformops-blueprints/portal-blueprint-page) |
| portal-blueprint-page | [1.0.1](https://github.com/krateoplatformops-blueprints/portal-blueprint-page/tree/1.0.1) | <ul><li>portal</li></ul> | >= 2.5.1 | [https://github.com/krateoplatformops-blueprints/portal-blueprint-page](https://github.com/krateoplatformops-blueprints/portal-blueprint-page) |
| portal-blueprint-page | [1.0.0](https://github.com/krateoplatformops-blueprints/portal-blueprint-page/tree/1.0.0) | <ul><li>portal</li></ul> | >= 2.5.1 | [https://github.com/krateoplatformops-blueprints/portal-blueprint-page](https://github.com/krateoplatformops-blueprints/portal-blueprint-page) |
| portal-composition-page-generic | [1.0.0](https://github.com/krateoplatformops-blueprints/portal-composition-page-generic/tree/1.0.0) | <ul><li>portal</li></ul> | >= 2.5.1 | [https://github.com/krateoplatformops-blueprints/portal-composition-page-generic](https://github.com/krateoplatformops-blueprints/portal-composition-page-generic) |
| portal-composition-page-generic-finops | [1.0.0](https://github.com/krateoplatformops-blueprints/portal-composition-page-generic-finops/tree/1.0.0) | <ul><li>portal</li><li>finops</li></ul> | >= 2.5.1 | [https://github.com/krateoplatformops-blueprints/portal-composition-page-generic-finops](https://github.com/krateoplatformops-blueprints/portal-composition-page-generic-finops) |
| portal-finops-dashboard | [1.0.0](https://github.com/krateoplatformops-blueprints/portal-finops-dashboard/tree/1.0.0) | <ul><li>portal</li><li>finops</li></ul> | >= 2.5.1 | [https://github.com/krateoplatformops-blueprints/portal-finops-dashboard](https://github.com/krateoplatformops-blueprints/portal-finops-dashboard) |
| portal-finops-dashboard | [0.0.1](https://github.com/krateoplatformops-blueprints/portal-finops-dashboard/tree/0.0.1) | <ul><li>portal</li><li>finops</li></ul> | >= 2.5.1 | [https://github.com/krateoplatformops-blueprints/portal-finops-dashboard](https://github.com/krateoplatformops-blueprints/portal-finops-dashboard) |
| vm-azure | [0.1.2](https://github.com/krateoplatformops-blueprints/azure-vm-finops/tree/0.1.2) | <ul><li>finops</li></ul> | >= 2.5.1 | [https://github.com/krateoplatformops-blueprints/azure-vm-finops](https://github.com/krateoplatformops-blueprints/azure-vm-finops) |
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
