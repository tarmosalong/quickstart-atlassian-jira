# quickstart-atlassian-jira
## Jira Software and Jira Service Desk Data Center on the AWS Cloud

Use this Quick Start to deploy one of the following Jira products from Atlassian on the AWS Cloud:

* Jira Software Data Center
* Jira Service Desk Data Center

This Quick Start uses the [Atlassian Standard Infrastructure (ASI)](https://fwd.aws/xYyYy) as a foundation. You can choose to build a new ASI for your deployment or deploy Jira into your existing ASI. You can also deploy Bitbucket Data Center and Confluence Data Center within the same ASI.

![Quick Start architecture for Jira on AWS](https://d0.awsstatic.com/partner-network/QuickStart/datasheets/jira-on-aws-architecture.png)

For architectural details, best practices, step-by-step instructions, and customization options, see the 
[deployment guide](https://fwd.aws/Wz3Qb).

### Network prerequisites

You need to create the required AWS networking infrastructure
(VPC, subnets) by using the [ASI Quick Start](https://fwd.aws/xYyYy), or by deploying Jira with a new ASI.
For details, see the [deployment guide](https://fwd.aws/Wz3Qb).

### Contributing & issues

Please note that issues are disabled for this repository, because it is a
downstream repository that is not actively supported.
We welcome pull requests, issues, and comments in the **[upstream repository](https://bitbucket.org/atlassian/atlassian-aws-deployment/src/master/quickstarts/)**.

If you'd like to submit code for this Quick Start, please review the [AWS Quick Start Contributor's Kit](https://aws-quickstart.github.io/). 

## Development notes

### Pre-commit hook

It is recommended that you install the hooks under `submodules/quickstart-atlassian-services/scripts/hooks/`; this will
ensure that the metadata tags in the templates are automatically updated on
commit. The simplest method of doing this is:

    git config --add core.hooksPath submodules/quickstart-atlassian-services/scripts/hooks/

Alternatively you can invoke
`submodules/quickstart-atlassian-services/scripts/hooks/update-tags.py`
manually.
