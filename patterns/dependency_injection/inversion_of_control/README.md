
1. Run `make setup` from this directory. This will create
   a network and a subnet for you use.

1. It will generate a file in `network/terraform.tfstate`. The state
   file includes some JSON metadata that includes the network name.

1. Run `python main.py` to generate the `main.tf.json` file. This
   should include the network's name.

1. Run `terraform apply` and enter `yes` to create the server.

1. Run `make clean` to delete the server and the network.
