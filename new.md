# AWS VPC Project

## Objective

Create a production-style AWS VPC with public and private subnets.

## Architecture

```text
Internet
    |
Internet Gateway
    |
Public Subnet
    |
NAT Gateway
    |
Private Subnet
```

## Components Used

| Component        | Purpose                            |
| ---------------- | ---------------------------------- |
| VPC              | Network Isolation                  |
| Public Subnet    | Internet Facing Resources          |
| Private Subnet   | Internal Resources                 |
| Internet Gateway | Internet Access                    |
| NAT Gateway      | Outbound Access for Private Subnet |

## Implementation Steps

### Step 1: Create VPC

CIDR Block:

```text
10.0.0.0/16
```

### Step 2: Create Subnets

Public Subnet:

```text
10.0.1.0/24
```

Private Subnet:

```text
10.0.2.0/24
```

### Step 3: Configure Route Tables

* Public Route Table
* Private Route Table

### Step 4: Attach Internet Gateway

Attach IGW to the VPC and update routes.

## Validation

* Public instances can access the internet.
* Private instances access the internet through NAT Gateway.

## Outcome

Successfully created a secure and scalable VPC architecture.
