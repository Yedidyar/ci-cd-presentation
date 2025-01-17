---
theme: default
background: https://source.unsplash.com/collection/94734566/1920x1080
class: text-center
highlighter: shiki
lineNumbers: false
drawings:
  persist: false
transition: slide-left
title: CI/CD - A Comprehensive Introduction
---

# Continuous Integration and Continuous Delivery (CI/CD)

How to Deliver Software Quickly and Reliably

---
layout: section
---

# The History of CI/CD & Motivation

---

# Early Software Development Practices

- Manual integrations at the end of long development cycles
- High risk of "integration hell"
- Waterfall model → long release cycles, less feedback

---
layout: image
image: https://musimorphic.com/wp-content/uploads/2022/10/home-alone-1024x768.jpg
backgroundSize: 50%
---

---

# Shift to Agile

<v-clicks>

- **Agile Methodologies:**
  - Frequent iterations (Sprints)
  - Quick, user-centric feedback
  - Closer collaboration among devs, testers, stakeholders

</v-clicks>

---

# Emergence of Continuous Integration

<v-clicks>

- **CI Origins:**
  - Influenced by Extreme Programming (XP) and ThoughtWorks
  - Frequent code commits, automated builds
  - Immediate feedback on build or test failures

</v-clicks>

---
layout: image-left
image: https://www.mabl.com/hubfs/CICDBlog.png
backgroundSize: 70%
---
# Continuous Delivery & Deployment

<v-clicks>

- **Definition:**
  - Continuous Delivery: Always in a deployable state
  - Continuous Deployment: Automatic deployment after CI success

- **Motivation:**
  - Faster time to market
  - Reduced risk
  - Ongoing, incremental releases

</v-clicks>

---

# Why It Matters

<v-clicks>

- **Benefits:**
  - Reduced "integration hell"
  - Shorter feedback loop
  - Higher confidence in new features
  - More stable, frequent releases

</v-clicks>

---
layout: section
---

# Developer Workflow from PR to Deployment

---

# Developer Workflow Overview

<v-clicks>

- Code & Commit
- Pull Request (PR)
- Automated CI Checks
- Merge & CD Pipeline
- Deployment to Production

</v-clicks>

---

# Creating a Pull Request

<v-clicks>

- **Purpose:**
  - Code Review
  - Shared Knowledge
  - Standardization (linting, style checks)

- **Automated Checks:**
  - Linting, security scans, static analysis

</v-clicks>

---

# Continuous Integration (CI) Stage

<v-clicks>

- **Build Process:**
  - Ensure code compiles and passes basic checks

- **Automated Testing:**
  - Runs unit tests, integration tests, coverage checks

- **Immediate Feedback:**
  - Developers see pass/fail quickly

</v-clicks>

---
layout: image
image: https://cdn.corporatefinanceinstitute.com/assets/range1.png
backgroundSize: 50%
class: text-center
---
# Confidence Range


---
layout: image-right
image: https://media.licdn.com/dms/image/v2/C5612AQH0h2q_mufjww/article-cover_image-shrink_720_1280/article-cover_image-shrink_720_1280/0/1595457832720?e=2147483647&v=beta&t=-7hk9T_lPwXB9jy3FanSKvtpq1RaFh5VYNTAw8e2ZIg
backgroundSize: 90%
---

# Types of Deployments

<v-clicks>

- **Blue-Green:**
  - Two identical environments (current = Blue, new = Green)
  - Easy rollback strategy

- **Rolling Updates:**
  - Incrementally replace old version with new
  - Zero downtime with careful orchestration

- **Canary Releases:**
  - Roll out new code to a small subset of users
  - Validate performance before full release

</v-clicks>

---
layout: section
---

# CI/CD Providers

---

# Overview of CI/CD Tools

<v-clicks>

- Self-Hosted
- Cloud-Hosted
- Hybrid Approaches

</v-clicks>

---

# Open-Source Solutions

<v-clicks>

- **Jenkins:**
  - Highly customizable, plugin-rich
  - Requires own server maintenance

- **GitLab CI/CD:**
  - Integrated with GitLab repos
  - .gitlab-ci.yml for pipeline config

- **GitHub Actions:**
  - Deeply integrated with GitHub repos
  - YAML-based workflows

</v-clicks>

---

# Testing in CI/CD

<div class="flex justify-center">
  <div class="w-64 h-64 relative">
    <div class="absolute bottom-0 w-full h-1/2 bg-blue-200 text-center py-4">
      Unit Tests
    </div>
    <div class="absolute bottom-1/2 w-3/4 h-1/3 bg-blue-300 left-1/2 transform -translate-x-1/2 text-center py-4">
      Integration Tests
    </div>
    <div class="absolute top-0 w-1/2 h-1/6 bg-blue-400 left-1/2 transform -translate-x-1/2 text-center py-2">
      E2E
    </div>
  </div>
</div>

---

# Unit Tests (UT)

<v-clicks>

- **Definition:**
  - Test smallest pieces of functionality

- **Tools:**
  - JUnit, pytest, Jest, etc.

- **Frequency:**
  - Run on every commit/pull request

</v-clicks>

---

# Integration Tests

<v-clicks>

- **Scope:**
  - Multiple modules or services interacting

- **Challenges:**
  - Environment setup
  - Mocks/stubs management

- **Value:**
  - Catch issues missed by unit tests

</v-clicks>

---

# Monitoring Overview

<v-clicks>

- **Application Performance Monitoring (APM):**
  - Datadog, New Relic
  - Track response times, throughput, error rates

- **Infrastructure Monitoring:**
  - Prometheus + Grafana
  - CPU, memory, network usage

- **Log Management:**
  - ELK stack, Splunk
  - Centralized logging

</v-clicks>

---
layout: center
class: text-center
---

# Thank You!

[Documentation](https://your-docs-link) · [GitHub](https://your-github-link) · [Slides](https://your-slides-link)