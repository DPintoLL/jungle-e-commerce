# Jungle

> Mini e-commerce application built with Rails and Stripe

Jungle is a full-stack Rails app made to mimic a real e-commerce app. With complete CRUD operations implemented, users can register, login, logout, add items to their cart, and use Stripe to make simulated purchases. Admins can view a dashboard with information about customers and products, as well as add and remove items, categories, and sales to and from the database.

## Table of contents

- [Usage](#usage)
- [Getting started](#getting-started)
  - [Prerequisites](#prerequisites)
  - [Installing and running](#installing-and-running)
- [Running the Tests](#running-the-tests)
- [Built with](#built-with)
- [Contributing](#contributing)
- [Meta](#meta)
- [Known issues / bugs](#known-issues-/-bugs)
- [Feature roadmap](#feature-roadmap)
  - [In the works](#in-the-works)
  - [Planned](#planned)
- [Acknowledgements](#acknowledgements)

## Usage

![Jungle]()

## Getting started

These instructions will get you a copy of the project up and running on your local machine for development and testing purposes.

### Prerequisites

You need Ruby and Rails installed, specifically Ruby 2.3.5x and Rails 4.2.x.

### Installing and Running

1. Run `bundle install` to install dependencies
2. Create `config/database.yml` by copying `config/database.example.yml`
3. Create `config/secrets.yml` by copying `config/secrets.example.yml`
4. Create `.env` by copying example and providing an elephantsql database URL
5. Run `bin/rake db:reset` to create, load and seed db
6. Sign up for a Stripe account
7. Put Stripe (test) keys into appropriate .env vars
8. Run `bin/rails s -b 0.0.0.0` to start the server

**NOTE: You may need to add `ruby` infront of binstub commands**

## Running the Tests

Use Credit Card # 4111 1111 1111 1111 for testing success scenarios.

More information in their docs: <https://stripe.com/docs/testing#cards>

To run the tests:

```sh
bin/rspec
```

## Built with

- [Rails 4.2.x]() - Front-end framework
- [Stripe]() - Payment API
- [PostgreSQL 9.x]() - open source SQL database
- [Bootstrap]() - css framework
- [Capybara]() - end-to-end testing framework

## Contributing

1. Fork it (<https://github.com/DPintoLL/jungle-e-commerce/fork>)
2. Create your feature branch (`git checkout -b feature/fooBar`) or issue branch (`git checkout -b issue/brokenThing`)
3. Commit your changes (`git commit -m 'Add some fooBar'`)
4. Push to the branch (`git push origin feature/fooBar`)
5. Create a new PR

## Meta

Diogo Pinto – [diogopinto.dev](https://github.com/DPintoLL/) – diogosmp@gmail.com

## Known issues / bugs

- Bugs? What bugs?

_To add an issue, start a new one [here.](https://github.com/DPintoLL/jungle-e-commerce/issues)_

## Feature roadmap

### In the works

- Deploy
- Have sales properly affect prices, accounting for multiple simultaneous sales

### Planned

- More tests
- Auto fill forms based on logged in user data
- Restyle

_If you'd like to add a feature yourself, please see the [Contributing](#contributing) guidelines._

## Acknowledgements

- This was done as a project for Lighthouse Labs
