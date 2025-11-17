# 🏷️ Repository Naming Convention and Style Guide

This standard is mandatory for **all new repositories** created under our organization. It ensures consistency, improves searchability, and helps every team member (including junior developers) quickly identify the purpose and ownership of a repository.

## 📏 Naming Convention Format

All repository names must follow this structure:

$$[PREFIX]-[SPECIFIC-ENTITY]-[DESCRIPTION]$$

### Style Rules

1.  **Case:** Must be **all lowercase**.
2.  **Separator:** Must use **hyphens (`-`)** to separate words.
3.  **No Special Characters:** Avoid underscores, periods, or spaces.

---

## 1. 🔑 Required Prefixes

Start every repository name with one of the following prefixes. This is the **most important** rule for organization and filtering.

| Prefix | Category | Purpose | Example Name |
| :--- | :--- | :--- | :--- |
| `client` | **Client Projects** | External, contracted work for a paying customer. | `client-acme-fraud-detection-api` |
| `template` | **Boilerplates** | Standard starter kits, project structures, or common configurations. | `template-mlops-aws-sagemaker` |
| `tool` | **Internal Tools/Apps** | Software used internally by our consultants (e.g., dashboards, billing scripts). | `tool-resource-planner-dashboard` |
| `poc` | **Research & Sandbox** | Proofs-of-concept (PoC), R&D, or non-client experimental work. | `poc-llm-fine-tuning-approach` |
| `infra` | **Infrastructure/Ops** | Shared configuration for CI/CD, Terraform, Kubernetes, etc. | `infra-gcp-setup-staging` |

---

## 2. 🎯 Specific Entity

This part identifies the primary owner or technology:

* **For `client` repositories:** Use the client's short, hyphenated name (e.g., `acme-`, `globo-`).
* **For other categories:** Use the primary function or technology (e.g., `billing-`, `python-api-`, `deployment-`).

## 3. 📝 Project Description

A concise, clear description of the repository's main deliverable or function.

---

## ✅ Quick Reference Examples

| Correct Name | Category | Explanation |
| :--- | :--- | :--- |
| `client-acme-invoice-parser` | Client Project | Work for Acme, focused on invoice parsing. |
| `template-python-api-fastapi` | Boilerplate | A Python API template using FastAPI. |
| `tool-consultant-time-tracker` | Internal Tool | The internal application for tracking consultant time. |
| `poc-yolo-v9-benchmark` | R&D | Proof-of-Concept testing a benchmark for YOLO v9. |

| ❌ **Incorrect Names** | ❓ **Why It's Wrong** |
| :--- | :--- |
| `ACME_Project_v1` | Wrong case, wrong separator, missing prefix. |
| `data-ingestion-script` | Missing required prefix (`tool-` or `client-`). |
| `test-repo-delete-later` | Not descriptive, uses discouraged `test-` prefix. |
