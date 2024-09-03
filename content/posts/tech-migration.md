---
title: "Implementing New Tech Stack"
description: "meta description"
date: 2024-09-04
image: "/images/posts/cover2.jpg"
categories: ["Architecture"]
authors: ["Adrian"]
tags: ["Migration"]
draft: false
---

This project aims at the constant improvement of the Fuel Design System documentation ecosystem, as a css style-oriented design system as a start.

The architecture proposal presented is based on an adequate and efficient work method which is the reuse of code and the parameterization of development processes, improving delivery times and scalability of the project.

![](./images/posts/diagram1.jpg)

## Technology stack (MSC Fuel Design System  V2)

**We have selected the following technologies:**

![](./images/posts/diagram2.jpg)

After the evaluation of the needs of the project this stack will work unified to make a stable and scalable ecosystem, working on a base with html, css and js through powerful frameworks with an active and strong community.

### Why React?

React was chosen as the basis of the project because of its versatility, as it allows customization of the frontend layers, for example, it allows the integration of libraries that facilitate daily work without the need to do a development from scratch.

Its large and strong community is of great support in the development of new libraries and useful features for use within the framework.

Now some benefits of using React.

1. **Component-Based Architecture:** React’s component-based structure allows developers to build encapsulated components that manage their own state, making it easier to develop and maintain complex user interfaces.

2. **Virtual DOM:** React uses a virtual DOM to optimize updates and rendering, which improves performance by minimizing direct manipulation of the actual DOM.

3. **SEO-Friendly:** React can be rendered on the server side, which helps in improving the SEO of web applications by making them more accessible to search engines.

4. **Reusable Code:** Components in React can be reused across different parts of an application, reducing redundancy and improving code maintainability.

5. **Fast Learning Curve:** React is relatively easy to learn, especially for developers familiar with JavaScript, making it accessible for new developers.

6. **Strong Ecosystem:** React has a vast ecosystem of libraries and tools that can be integrated to extend its functionality, such as Redux for state management and React Router for navigation.

7. **Cross-Platform Development:** React Native, a framework based on React, allows developers to build mobile applications for both iOS and Android using the same codebase.

8. **Active Community and Support:** The large and active community around React provides extensive resources, tutorials, and third-party libraries, which can be very helpful for developers.

### Why Storybook?

The main goal of Storybook is to make it easy to develop and test UI components in isolation. This means that you can build and display components without interacting with the rest of the application, resulting in a faster and more efficient development process.

Storybook works as a visual catalog of components, allowing developers to see how each component behaves in different configurations and states. In addition, it is compatible with several JavaScript libraries and frameworks, such as React, Vue, Angular, Svelte and Ember.js.

### Why Tailwind CSS?

The main goal of Tailwind CSS is to enable developers to create custom designs quickly and efficiently. It is a utility-first CSS framework, which means it provides a set of low-level utility classes that can be combined to build complex designs directly in your HTML. This approach allows for greater flexibility and faster development compared to traditional CSS frameworks that offer pre-designed components.

## MSC Shared Styles

The goal of making a design system is to reach as many platforms as possible as this will allow to have congruence between different developments using the same system for all projects that are developed for web and mobile.

### MSC CDN

Works as the primary provider of the styles of our Design System, it is the core of the main line of design.

![](./images/posts/diagram3.jpg)

## About the upgrades

![](./images/posts/diagram4.jpg)

### The problem with storybook

It is complicated to use vanilla and storybook as it is as if we were working double for everything. 

Creating a component would require creating it in vanilla with tailwind, but unlike React, with vanilla you have to make a series of adjustments and recreate the component so that storybook is able to display it.

With react and other frameworks better adapted to this type of work the component is deployed directly from the component created in react, resulting in a component with html and Tailwind CSS as output even though it is built with react.

Besides taking advantage of the super powers of react to make the code cleaner and being a showcase the functionality also becomes simpler and more scalable.

### Component Example

This is an example for the Alphabetical Pager, it shows the difference of using, react vs vanilla and how it makes better to support and the result on the final deployed page will be the same.

Maybe it will be some ways to doit with vanilla but we don´t need to create again something that already exist, and it is polished through the time.

##### Alphabetic Pager
![](./images/posts/alpha-pager.jpg)

#####  Code Difference:

<div className='flex gap-2'>
  <div className='flex-1'>
  <h5>HTML Code</h5>
  ![](./images/posts/code1.jpg)
  </div>
  <div className='flex-1'>
  <h5>React Code</h5>
  ![](./images/posts/code2.jpg)
  </div>
</div>