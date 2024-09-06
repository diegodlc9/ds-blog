---
title: "New DS Architecture"
description: "meta description"
date: 2024-08-26
image: "/images/posts/site-arch.jpg"
categories: ["WIP"]
authors: ["Diego"]
tags: ["Site Architecture"]
draft: false
---

We’re excited to unveil our new design system architecture. We’ll dive into the details of how the architecture is structured, the key components involved, and the benefits it brings to our workflow. We’ll also discuss the motivations behind this change and how it will enhance our design and development processes. Whether you’re a designer, developer, or stakeholder, this new system is designed to streamline our efforts and foster better collaboration across teams.

## Motivation

Given the different goals within the Design System (DS), it is necessary to separate each one into different projects to achieve better organization and efficiency in the workflow. This approach also makes the system more maintainable and scalable. As the project grows, it becomes increasingly difficult to manage the main project. Therefore, we propose this new site architecture where each site has its own specific goal.

The idea is to separate each goal into a different site so that each one focuses solely on its specific objective. We will start with the main design system site, which will serve as the starting point to link to the other sites.

## Single Responsibility

The “Single Responsibility” concept is widely used in the software field and is applied in different areas. In this case, we are applying it to each of the goals within the Design System (DS). While all the goals collectively aim towards a final objective, the development of each one is somewhat different. Although everything can be maintained within the main project, concentrating everything in one place can impact many aspects of the workflow. If one thing fails, everything fails.

That’s why we propose separating each goal into a different site. Although it may seem like more work, it isn’t; it’s exactly the same amount of work. The only difference will be in the management of the DS project. The main advantages will be improved internal organization (development and maintenance).

## New Architecture

**Here is a diagram illustrating how the new architecture will work:**

![](./images/posts/site-arch-1.jpg)

- **Design system site:** This is the main site where the goal is to showcase the components with the necessary code for developers, written in a human-friendly way so that everyone who accesses it can understand it.
- **Storybook Site:** This project will contain all the components, documented in a developer-centric way for those who want to see all the component details.
- **DS Blog:** The goal of this site is to contain all the information regarding the entire DS project, such as _release notes_, _fix notes_, _WIP information_, etc.

This is the best way to manage a complex project and ensure everything runs smoothly. This would be version 1.0, as it can continue to grow, in the future, we might want to integrate Figma to complement the DS documentation or simply improve the documentation, which could require additional resources. However, for now, this is a very good approach and a solid starting point to build the **Fuel Design System**.