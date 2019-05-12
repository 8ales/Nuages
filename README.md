# Nuages
A modular C2

## Introduction

Nuages aims at being a C2 framework in which back end elements are open source, whilst implants and handlers must be developed ad hoc by each user. It does not provide a way to generate implants, but an open source framework to develop and manage compatible implants that can leverage all the back end resources already developed.

Although Nuages is functionning, it is still a work in progress and contribution are welcome, wether it is solely testing, or development of new modules and compatible clients.

For testing and refererence, an example implant and handler are provided on this repo.

## Architecture
![Nuages](https://user-images.githubusercontent.com/19682240/56617113-ffcfb380-65ec-11e9-99ca-fc0e674d4dcd.PNG)

**Nuages C2:** It is the core of the C2 and manages the implants, it is open source and should not need to be customized.

**Implants:** Custom code to run on the target devices, they can communicate with handlers over custom protocol or directly with the Nuages API.

**Handlers:** Custom code acting as a proxy between Implants and the Nuages API, to implemenet custom communication protocols (DNS tunneling, domain fronting, IRC etc...).

**Clients:** Clients rely on the Nuages API and can be implemented in any form such as cli or web application.

## Disclaimer
This project is intended for security researchers and penetration testers and should not be used for any illegal activities.
