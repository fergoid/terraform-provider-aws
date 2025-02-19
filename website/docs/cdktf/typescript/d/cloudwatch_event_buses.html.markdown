---
subcategory: "EventBridge"
layout: "aws"
page_title: "AWS: aws_cloudwatch_event_buses"
description: |-
  Terraform data source for managing an AWS EventBridge (Cloudwatch) Event Buses.
---


<!-- Please do not edit this file, it is generated. -->
# Data Source: aws_cloudwatch_event_buses

Terraform data source for managing an AWS EventBridge Event Buses.

## Example Usage

### Basic Usage

```typescript
// DO NOT EDIT. Code generated by 'cdktf convert' - Please report bugs at https://cdk.tf/bug
import { Construct } from "constructs";
import { TerraformStack } from "cdktf";
/*
 * Provider bindings are generated by running `cdktf get`.
 * See https://cdk.tf/provider-generation for more details.
 */
import { DataAwsCloudwatchEventBuses } from "./.gen/providers/aws/";
class MyConvertedCode extends TerraformStack {
  constructor(scope: Construct, name: string) {
    super(scope, name);
    new DataAwsCloudwatchEventBuses(this, "example", {
      name_prefix: "test",
    });
  }
}

```

## Argument Reference

The following arguments are optional:

* `namePrefix` - (Optional) Specifying this limits the results to only those event buses with names that start with the specified prefix.

## Attribute Reference

This data source exports the following attributes in addition to the arguments above:

* `event_buses` - This list of event buses.

### `event_buses` Attribute Reference

* `arn` - The ARN of the event bus.
* `creationTime` - The time the event bus was created.
* `description` - The event bus description.
* `lastModifiedTime` - The time the event bus was last modified.
* `name` - The name of the event bus.
* `policy` - The permissions policy of the event bus, describing which other AWS accounts can write events to this event bus.

<!-- cache-key: cdktf-0.20.8 input-edc68a47cdadc6ea17720030205db67bdcde4de355a2ff487a2754598fadec7e -->