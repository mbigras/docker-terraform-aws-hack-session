# docker-terraform-aws-hack-session

> Alpine image with utilities for AWS and Terraform hack session

## Usage

```
docker run -itd --name terraform mbigras/terraform-aws-hack-session
for tool in {terraform,aws,lpass,jq}; do
	docker exec terraform $tool --version
done
docker rm -f terraform
```

## Build

```
docker build --tag mbigras/terraform-aws-hack-session .
```
