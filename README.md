
# Hotmart Devops Challenge

![Logo](https://www.hotmart.com/images/hotmart-logo.svg)

## Run Locally

Clone the project

```bash
  git clone -b release git@github.com:lmascarenhas/hotmart-devops-challenge.git
```

Go to the project directory

```bash
  cd hotmart-devops-challenge
```

First you need to create a bucket using Terraform, but before run terraform you need:

- Install Terraform. Reference => https://learn.hashicorp.com/tutorials/terraform/install-cli#install-terraform
- Configure your AWS Credentials File. Reference => https://docs.aws.amazon.com/cli/latest/userguide/cli-configure-profiles.html

```bash
  cd terrraform
  terraform init
  terraform apply
```

Before you run this app you need to install `docker` and `docker-compose`

Setup .env to run App Locally
```bash
cd ..

tee app-desafio.env <<EOF
AWS_ACCESS_KEY_ID="<REPLACE_WITH_YOUR_CREDENTIALS_ACCESS_KEY>"
AWS_SECRET_ACCESS_KEY="<REPLACE_WITH_YOUR_CREDENTIALS_ACCESS_KEY_SECRET_ACCESS_KEY>"
EOF

mkdir app/uploads
```

Run App 

```bash
docker-compose build
docker-compose up -d
```

## Authors

- [Luiz Mascarenhas](https://luiz.mascarenhas.it/)


## Support

For support, email luiz@mascarenhas.it.

