# emqx-test
Testing tool for EMQ X.

It'll include test cases for both load testing and feature testing.

## Load testing

```shell
# Start a load test using config file from '~/test/loadtest.toml'
./emqxt --mode=loadtest -c ~/test/lt.toml 
```
## Feature testing

```shell
# Start the test case verifying the issue described in https://github.com/emqx/emqx/issues/1874
./emqxt -t ft_emqx_issue_1874
```

## Design

- Loadtest should support configuring the test scenarios in the config file:
  - Define how many subscribers will be started and there test model.
  - Define how many publishers will be started and there test model.
- Emqxt should provide a DSL for writing test cases.

## Elixir

Utilize the fantasic metaprogramming ability of Elixir.

