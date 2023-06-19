---
author: Mart Anthony Salazar
pubDatetime: 2023-06-18T07:56:55.309Z
title: "Ngenly CLI: Streamlining API Development Like Never Before!"
postSlug: ngenly-cli
featured: true
draft: false
tags:
  - Nodejs
  - Npm
  - CRUD
  - REST-API
ogImage: "https://github.com/mart-anthony-stark/Ngenly-CLI/blob/main/image-3.png?raw=true"
description: A powerful Node.js CRUD API generator that streamlines the development process by automating the creation of CRUD operations, enabling developers to focus on other aspects of their projects.
---

Developing CRUD APIs can be a time-consuming and repetitive task for Node.js developers. Manually writing boilerplate code, configuring routes, and handling common security concerns can slow down the development process and hinder productivity. There is a need for a tool that simplifies API development, automates repetitive tasks, and promotes efficiency without compromising flexibility and security.

As the creator of Ngenly CLI, I am thrilled to present this game-changing tool that will revolutionize your API development process. Ngenly CLI is born out of my own experience as a Node.js developer, seeking a way to simplify and accelerate the creation of CRUD APIs.

With Ngenly CLI, I aimed to eliminate the mundane and repetitive aspects of API development. I wanted to provide developers with an intuitive and efficient solution that would free up their time and energy to focus on building unique features and delivering exceptional user experiences.

## Ngenly CLI

[![https://nodei.co/npm/ngenly.png?downloads=true&downloadRank=true&stars=true](https://nodei.co/npm/ngenly.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/ngenly)

A node project boilerplate generator

- [Installation](#installation)
- [Commands](#commands)
- [Create New Project](#create-a-new-project)
- [Generate CRUD files](#generate-crud-files)
- [GUI](#ngenly-gui)

## Installation

Install the package globally using yarn or npm

```console
npm install -g ngenly
```

## Usage

- execute in terminal
  ngenly [command]

## Commands

| Command                             | Description                                      |
| ----------------------------------- | ------------------------------------------------ |
| `ngenly new`                        | Generates a new project                          |
| `ngenly upgrade`                    | Installs the latest version of ngenly globally   |
| `ngenly [-g / generate]`            | Starts generating project or crud using menu     |
| `ngenly -v`                         | Returns cli version                              |
| `ngenly --version`                  | Returns cli version                              |
| `ngenly -g [crud] [library] [name]` | Generates crud files (Model, Controller, Router) |
| `ngenly --gui`                      | Opens the browser for ngenly GUI                 |

## Create a new project

```console
ngenly new
```

![Ngenly Create Project](https://github.com/mart-anthony-stark/Ngenly-CLI/blob/main/image-1.png?raw=true)

- Project Boilerplate will be created with its own folder
  ![Alt text](https://github.com/mart-anthony-stark/Ngenly-CLI/blob/main/image-2.png?raw=true)
  > You can also generate project boilerplate with one-liner command
  > Usage: ngenly -g project [expressjs | expressts | fastifyjs | fastifyts] [projectName]

```console
ngenly -g project expressjs School-Management-API
```

## Generate CRUD files

> Usage: ngenly -g crud [expressjs | expressts | fastifyjs | fastifyts] [model_name]

```
ngenly -g crud expressjs user
```

![Generate CRUD](https://github.com/mart-anthony-stark/Ngenly-CLI/blob/main/image.png?raw=true)

## Ngenly GUI

Ngenly GUI is a new feature introduced in version 3.0.0 of the Ngenly CLI tool. It provides a graphical user interface (GUI) for easier interaction with Ngenly and its functionalities.

As of now, the Ngenly GUI primarily includes the "Create Project" feature, allowing users to generate a new project with a few simple steps through the graphical interface. However, please note that additional features, such as creating models, routes, and controllers are planned to be added in future updates. These enhancements will further empower developers to efficiently generate and manage their projects using the Ngenly CLI tool.

Stay tuned for updates as more features are incorporated into the Ngenly GUI to enhance your development experience.

- Command for starting gui local server
  > You need to be in an empty directory (your desired new project directory).

```
ngenly --gui
```

- Or you can also just enter `ngenly` command and the GUI will start
  ![Alt text](https://github.com/mart-anthony-stark/Ngenly-CLI/blob/main/image-3.png?raw=true)

> Note: Creating a new project with Ngenly requires an internet connection as it involves cloning a boilerplate from a hosted git repository. However, generating CRUD files (Model, Route, Controller) can be done offline without the need for an internet connection.
