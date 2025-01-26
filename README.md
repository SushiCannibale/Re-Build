# Re:Try

**Re:Try** is an open source project that helps students who wants to achieve the at Epita testing the code of their project over shared test suites.

> [!CAUTION]
> We advise to make your own tests and not rely entirely on the service.
> This is only meant to enhance your test suite, not replacing it !

> [!WARNING]
> 🚧 The project is still under development 🚧

## Usage
Well... not for now ;-;

## Roadmap
Here is a list of what we would like to implement as quickly as possible as a proof of concept.

**🔑 Auth:** Only allow students at EPITA Toulouse to use the service. \
**📛 Limitations:** One tag a week. This is meant to avoid abuses \
**📦 Test submission:** Students can submit test suites and review them. \
**🚢 Environments:** On-demand docker containers. (I know, no k8s cluster for now 😢) \
**🌍 Website:** To group the actions available to a student.
* Registering SSH keys
* Submitting a test suite for a project
* Seeing tests results

### 🚢 About environments 🚢
The idea is to setup a container for each tag request. The container will be built upon an image especially created for the selected project. After running the code, the container will send the results to the database and stop.

### 📦 About test suites 📦
The test suites are submitted by the students, for the students. So they are responsible of their operation.
Students can review and vote for a test suite. If a test suite reaches down votes limit, it is removed from the database.

> [!NOTE]
> Other students cannot modify your test suite, but they can comment it and/or down vote it.

## ✨ Enhancement ✨

#### Backend API
Maybe proposing an API the students can request from in order to get a summary of the tests they passed and failed.

## 💜 Contributing to the project 💜
You can fork the repo and open a pull request whenever you like.