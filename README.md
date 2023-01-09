## IaC - Patterns

Patterns for InfrastructureAsCode
- ADAPTOR Transform metadata from one resource for compatability with another
- BUILDER Create resource(s) based on inputs, same process creates different representations
- COMPOSITE Compose resources in a hierarchal structure for automation
- DEPENDENCY_INJECTION 
    Inversion of Control high level resource calls low level for attributes
    Dependency Inversion expressing high & low level resources through abstraction
- FACADE Reference a unified interface for attributes
- FACTORY Inputs to create resources with specific configuration
- MEDIATOR Organizes dependencies btwn resources and creates/deletes objects as needed
- PROTOTYPE Specify creation resources and create others by copying
- SINGLETON Single instance which applies to rarely changed resources

### Creating Resources

1. Run Python.
   ```shell
   $ python main.py
   ```

1. You should have a set of files with `*.tf.json`. Then, you can
   execute Terraform to initialize the plugin.
   ```shell
   $ terraform init
   ```

1. Apply Terraform and make sure to enter "yes" to create the resources.
   ```shell
   $ terraform apply
   ```

### Removing Resources

You can delete resources by changing the working directory
of the code listing and destroying resources with Terraform.

```shell
$ terraform destroy
```