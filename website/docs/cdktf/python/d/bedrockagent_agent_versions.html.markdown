---
subcategory: "Bedrock Agents"
layout: "aws"
page_title: "AWS: aws_bedrockagent_agent_versions"
description: |-
  Terraform data source for managing an AWS Amazon BedrockAgent Agent Versions.
---


<!-- Please do not edit this file, it is generated. -->
# Data Source: aws_bedrockagent_agent_versions

Terraform data source for managing an AWS Amazon BedrockAgent Agent Versions.

## Example Usage

### Basic Usage

```python
# DO NOT EDIT. Code generated by 'cdktf convert' - Please report bugs at https://cdk.tf/bug
from constructs import Construct
from cdktf import Token, TerraformStack
#
# Provider bindings are generated by running `cdktf get`.
# See https://cdk.tf/provider-generation for more details.
#
from imports.aws.data_aws_bedrockagent_agent_versions import DataAwsBedrockagentAgentVersions
class MyConvertedCode(TerraformStack):
    def __init__(self, scope, name):
        super().__init__(scope, name)
        DataAwsBedrockagentAgentVersions(self, "test",
            agent_id=Token.as_string(aws_bedrockagent_agent_test.agent_id)
        )
```

## Argument Reference

The following arguments are required:

* `agent_id` - (Required) Unique identifier of the agent.

## Attribute Reference

This data source exports the following attributes in addition to the arguments above:

* `agent_version_summaries` - List of objects, each of which contains information about a version of the agent. See [Agent Version Summaries](#agent-version-summaries)

### Agent Version Summaries

* `agent_name` - Name of agent to which the version belongs.
* `agent_status` - Status of the agent to which the version belongs.
* `agent_version` - Version of the agent.
* `created_at` - Time at which the version was created.
* `updated_at` - Time at which the version was last updated.
* `description` - Description of the version of the agent.
* `GuardrailConfiguration` - Details aout the guardrail associated with the agent. See [Guardrail Configuration](#guardrail-configuration)

### Guardrail Configuration

* `guardrail_identifier` - Unique identifier of the guardrail.
* `guardrail_version` - Version of the guardrail.

<!-- cache-key: cdktf-0.20.8 input-e8636da2e6a3484a7889e96812691570a2397695de11688fd63667f1878a7793 -->