# Enterprise AI Stack Blueprint Studio

This repository contains the target configuration and SRE runtime files compiled by the **Enterprise AI Stack Blueprint Studio** dashboard module.

## 🚀 Description
Design and export your enterprise-grade AI architecture blueprint. Select standard components across 16 infrastructure layers and generate declarative deployment models.

## 🛠️ Specification Matrix
- **Primary Configuration File**: `/deploy/architecture/stack_blueprint.yaml`
- **Execution Command**: `kubectl apply -f stack_blueprint.yaml`
- **Validation Command**: `kubectl get aistackblueprints`

## 📋 How to Run & Validate

1. **Clone the repository:**
   ```bash
   git clone https://github.com/Pradeeptalari14/tp-enterprise-ai-stack.git
   cd tp-enterprise-ai-stack
   ```

2. **Run Execution Target:**
   ```bash
   kubectl apply -f stack_blueprint.yaml
   ```

3. **Verify Runtime Stability:**
   ```bash
   kubectl get aistackblueprints
   ```

## 🔐 Security & Best Practices
* **Secret Isolation**: Use organization-level secrets (or SSM parameter hooks) rather than hardcoded environment variables inside files.
* **Pull Request Lifecycles**: Protect default branch merges with validation checks before merging code changes.
