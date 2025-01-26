# Re-Build

**Re-Build** is an open source project that helps students who wants to achieve the at Epita testing the code of their project over shared test suites.

> [!CAUTION]
> We advise to make your own tests and not rely on those proposed by other students.
> This is only meant to show you the edge cases you might have missed.

> [!WARNING]
> 🚧 The project is still under development 🚧

## Usage
Well... not for now ;-;

## Roadmap
Here is a list of what we would like to implement as quickly as possible as a proof of concept.

#### Auth:
Only allow students at EPITA Toulouse to interact with the service.
#### Limitations:
Only permit a tag per week.
#### Test submission:
Students can submit test suites and review them.
#### Contained environment:
On-demand docker containers. (I know, no k8s cluster for now 😢)
#### Website:
To group the actions available to a student.
* Registering SSH keys
* Submitting a test suite for a project
* Tests results

### About environments:
The idea is to setup a container for each tag request. The container will be built upon an image specially created for the selected project. After running the code, the container will send the results to the database and stop.

### About test suites:
The test suites are submitted by the students, for the students. So they are responsible of their operation.
Students can review and vote for a test suite. If a test suite reaches down votes limit, it is removed from the database. Be aware that other students cannot modify your test suite. But they can comment it and ask you to review it.

### Enhancement
One day, maybe...

#### Backend API
Maybe proposing an API the students can request from in order to get a summary of the tests they passed and failed.

## Contributing to the project
You can fork the repo and open a merge request whenever you like.