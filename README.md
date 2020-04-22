# MongoDB cookbook 🐱‍🚀

- This cookbook install mongodb from source.

- It creates it's own apt package and then installs it.

- The recipe also create the config files and the service file with dynamic input of variables.

## Installs:
 • MongoDB

## Option and setting variables
- changes are made in the attributes file.

-  Changing the port:

```
# attributes/default.rb

default['mongo']['port'] = <new_value_here>
```
## Commands

### Test Locally
- Running my unit test:
```
chef exec rspec
```
- Running integration tests and closing machine:

```
kitchen tests
```

## Tests in AWS
- Running integration tests in AWS

```
KITCHEN_YAML=kitchen_cloud.yml kitchen test
```
