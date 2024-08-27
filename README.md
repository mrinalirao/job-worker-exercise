# job-worker-exercise

## Requirements

The project is broken down into 3 components:

A reusable library implementing the functionality for working with jobs.
An API server that wraps the functionality of the library.
A command line interface (CLI) that communicates with the API server.
Level 1

#### Library

Worker library with methods to start/stop/query status and get the output of a job.

#### API

HTTPS API to start/stop/get status of a running process.
Use HTTP Basic Authentication.
Use a simple authorization scheme.

#### CLI

CLI should be able to connect to worker service and start, stop, get status, and output of a job.

## Notes

#### Design Doc

Before writing any actual code, we ask that you write a brief design document. The design document should cover: design approach, scope, proposed API, security considerations, CLI UX, and implementation details where appropriate. Start with a brief doc that covers the edge cases and design approach.

Be sure to cover the following in your design:

CLI user experience: a couple examples of what it may look like to invoke a command. This allows us an opportunity to envision how we will run the program.

#### Implementation

Split your code submission into roughly 3-5 Pull Requests.

#### Testing

Add a couple of high quality tests that cover happy and unhappy scenarios.

Do not try to achieve full test coverage. This will take too long. Take two key components, e.g. authentication/authorization layer and networking and implement one or two test cases that demonstrate your approach to testing.

#### Dependencies

Please write as much of your own code as possible. Avoid relying on third party dependencies for key components of the challenge(cgroups, output streaming, authorization). The server should also not rely on any shell scripts, external binaries or use containers to execute jobs.

You may use any components from the standard library, gRPC, and whichever CLI library you are most familiar with.

