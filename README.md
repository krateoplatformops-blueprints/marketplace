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

### 🔹 Portal
Blueprints related to the Krateo user interface and experience.
- Examples: UI components, dashboard extensions, approval flows

### 🔹 Operations
Blueprints that support day-to-day platform operations.
- Examples: ArgoCD, external secrets management, cluster tooling

### 🔹 FinOps
Blueprints for cost tracking, reporting, and optimization.
- Examples: resource usage dashboards, quota controllers

### 🔹 Generator
Blueprints that dynamically generate Kubernetes controllers from an OpenAPI schema.
- Examples: controller generators, middlewares to handle APIs

Each Blueprint will be listed under one of these categories with:
- A short description
- A link to its implementation repository
- A Helm chart reference (as part of this registry)

---

## 📘 Available Blueprints

<!-- Available Blueprints START -->
<!-- This section is automatically updated. Do not edit manually. -->

| Blueprint Name | Blueprint Version | Blueprint Category | Blueprint Repository | Blueprint Description |
|----------------|-------------------|---------------------|-----------------------|------------------------|
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
