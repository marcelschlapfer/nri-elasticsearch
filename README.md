[![Community Plus header](https://github.com/newrelic/opensource-website/raw/master/src/images/categories/Community_Plus.png)](https://opensource.newrelic.com/oss-category/#community-plus)

# New Relic integration for elasticsearch

The New Relic integration for Elasticsearch captures critical performance metrics and inventory reported by Elasticsearch clusters. Data on the cluster, nodes, shards, and indices is collected.

Inventory data is obtained from the elasticsearch.yml file, and metrics and additional inventory data is obtained from the REST API.

## Installation and usage

For installation and usage instructions, see our [documentation web site](https://docs.newrelic.com/docs/integrations/host-integrations/host-integrations-list/elasticsearch-monitoring-integration).

## Compatibility

* Supported OS: No limitations
* elasticsearch versions: 5.0+

## Building

Golang is required to build the integration. We recommend Golang 1.11 or higher.

After cloning this repository, go to the directory of the Elasticsearch integration and build it:

```bash
$ make
```

The command above executes the tests for the Elasticsearch integration and builds an executable file called `nri-elasticsearch` under the `bin` directory. 

To start the integration, run `nri-elasticsearch`:

```bash
$ ./bin/nri-elasticsearch
```

If you want to know more about usage of `./bin/nri-elasticsearch`, pass the `-help` parameter:

```bash
$ ./bin/nri-elasticsearch -help
```

## Testing

To run the tests execute:

```bash
$ make test
```

## Support

Should you need assistance with New Relic products, you are in good hands with several support diagnostic tools and support channels.



> New Relic offers NRDiag, [a client-side diagnostic utility](https://docs.newrelic.com/docs/using-new-relic/cross-product-functions/troubleshooting/new-relic-diagnostics) that automatically detects common problems with New Relic agents. If NRDiag detects a problem, it suggests troubleshooting steps. NRDiag can also automatically attach troubleshooting data to a New Relic Support ticket.

If the issue has been confirmed as a bug or is a Feature request, please file a Github issue.

**Support Channels**

* [New Relic Documentation](https://docs.newrelic.com): Comprehensive guidance for using our platform
* [New Relic Community](https://discuss.newrelic.com): The best place to engage in troubleshooting questions
* [New Relic Developer](https://developer.newrelic.com/): Resources for building a custom observability applications
* [New Relic University](https://learn.newrelic.com/): A range of online training for New Relic users of every level
* [New Relic Technical Support](https://support.newrelic.com/) 24/7/365 ticketed support. Read more about our [Technical Support Offerings](https://docs.newrelic.com/docs/licenses/license-information/general-usage-licenses/support-plan).

## Privacy

At New Relic we take your privacy and the security of your information seriously, and are committed to protecting your information. We must emphasize the importance of not sharing personal data in public forums, and ask all users to scrub logs and diagnostic information for sensitive information, whether personal, proprietary, or otherwise.

We define “Personal Data” as any information relating to an identified or identifiable individual, including, for example, your name, phone number, post code or zip code, Device ID, IP address, and email address.

For more information, review [New Relic’s General Data Privacy Notice](https://newrelic.com/termsandconditions/privacy).

## Contribute

We encourage your contributions to improve this project! Keep in mind that when you submit your pull request, you'll need to sign the CLA via the click-through using CLA-Assistant. You only have to sign the CLA one time per project.

If you have any questions, or to execute our corporate CLA (which is required if your contribution is on behalf of a company), drop us an email at opensource@newrelic.com.

**A note about vulnerabilities**

As noted in our [security policy](../../security/policy), New Relic is committed to the privacy and security of our customers and their data. We believe that providing coordinated disclosure by security researchers and engaging with the security community are important means to achieve our security goals.

If you believe you have found a security vulnerability in this project or any of New Relic's products or websites, we welcome and greatly appreciate you reporting it to New Relic through [HackerOne](https://hackerone.com/newrelic).

If you would like to contribute to this project, review [these guidelines](./CONTRIBUTING.md).

To all contributors, we thank you!  Without your contribution, this project would not be what it is today.

## License

nri-elasticsearch is licensed under the [MIT](/LICENSE) License.
