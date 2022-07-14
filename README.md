# SDK Take Home Challenge

## Instructions

The goal is simple. Build an importable client-side library that helps a
developer run operations against a remote server. It will allow you to
understand the challenges we face at Forage and to demonstrate your skills.

1. The language will be determined by you and the hiring manager.
1. Clone this repository.
1. Complete the coding challenge.
1. Push your code changes to a private repository hosted by you on github. 
1. Email your hiring manager to invite them to your private repo and to schedule a code review.
1. Do a live code review with the hiring manager(s). 


### Required solution

- [ ] Create a visual component that allows an end-user to enter their EBT card number and submit it to the remote server.
- [ ] The component should submit the card number to the development server. The development server code lives in [./server/](./server/). Read [./server/README/md](./server/README.md) for instructions on how to run the server in your local dev environment.
- [ ] The component should be importable.
- [ ] The component should be mountable.
- [ ] The component should accept a callback function for succesful requests. The callback function expects a receipt of the response.
- [ ] Documentation on how to use the component.

### Extra credit solutions

- [ ] Accompanying unit tests.
- [ ] The client library is installable via a popular package manager.
- [ ] The component accepts a callback function for validation errors.

### About the server

We have created a development server and included it in this repository. You can find it in the directory `./server/`. 

## Prerequisites

- Docker
- Docker Compose

