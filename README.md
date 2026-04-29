# Jenkins DevSecOps Pipeline (Mock)

## Overview

This repository contains a mock Jenkins pipeline created for an academic assignment. The pipeline demonstrates a typical DevSecOps workflow integrated with GitHub, where changes to the repository automatically trigger the pipeline.

## Purpose

The purpose of this project is to simulate a continuous integration and DevSecOps pipeline using Jenkins and GitHub.
The pipeline is a mock implementation and does not perform real builds or deployments; instead, it prints the tasks and tools used at each stage.

## Pipeline Stages

The pipeline consists of the following 7 stages:

1. **Build**

   * Task: Compile and package the application
   * Tool: Maven

2. **Unit and Integration Tests**

   * Task: Execute tests to verify functionality
   * Tool: JUnit

3. **Code Analysis**

   * Task: Analyse code quality and enforce standards
   * Tool: SonarQube

4. **Security Scan**

   * Task: Identify vulnerabilities in dependencies
   * Tool: OWASP Dependency-Check

5. **Deploy to Staging**

   * Task: Deploy application to staging environment
   * Tool: AWS EC2

6. **Integration Tests on Staging**

   * Task: Validate application in a production-like environment
   * Tool: JUnit

7. **Deploy to Production**

   * Task: Deploy application to production environment
   * Tool: AWS EC2

## Automation

The pipeline is automatically triggered using Jenkins Poll SCM. Jenkins periodically checks the repository for new commits and runs the pipeline when changes are detected.

## Notes

* This is a **mock pipeline** created for demonstration purposes only
* No actual build, testing, or deployment is performed
* All stages output messages to the Jenkins console
