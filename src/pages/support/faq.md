# Adobe I/O Runtime: Frequently Asked Questions


## Getting Access
**How can I get access to I/O Runtime?**  
I/O Runtime is offering production service level since June 2019. You can find [here](../guides/overview/getting_access.md) information about how to get access.

## Supported Programming Languages
**Which languages are supported in I/O Runtime?**  
For now, Adobe I/O Runtime only supports Node.js. We might add support for other languages in the future.

### Node version 14 - Default Image
The NPM modules available with this image can be found [here](../guides/reference/runtimes.md#nodejs-v14).

We encourage you to always update your actions to the latest version in order to take advantage of pre-warm containters feature.

### Older Versions
When a new Node version is added to the system, the [old versions](../guides/reference/runtimes.md) are still available. This means that your actions will still work. We encourage you to always update your actions to the latest version in order to take advantage of pre-warm containers feature.

## What ports are open
**Are there any restrictions when it comes to ports and outbound connections?**

When retrieving data from some external systems your code might need to connect to a SFTP server, SMTP server, or HTTP service. As long as that system uses one of following ports, your code should work fine:

`21, 22, 25, 53, 80, 123, 143, [200-299], 389, 443, 445, 465, 587, 636, 1433, [2000-2999], 3000, 3306, 4242, 4317, 4343, 5400, 5432, 5671, 5672, 6061, 6062, 6379, 6380, 6651, 8000, 8020, 8080, 8085, 8088, 8089, 8300, 8500, 8600, 9090, 9092, 9093, 9094, [9096-9352], 9354, [10000-20000], 27016, 27017, 27018, 27019, 30303, 50010, 60020`.

If you have a need for a port that is not in this list, please share with us the use case.

## Price
**What does it cost to use Adobe I/O Runtime?**  
There are two ways you can get access to I/O Runtime: commercial offering and free trial. If you want to buy, please work with your Adobe account manager. If you are interested in the trial, check this [page](../guides/overview/getting_access.md).

## Usage Quotas
**What usage quotas are in place for Adobe I/O Runtime?**  
There are presently no usage quotas on Adobe I/O Runtime.

## Multiple Region Support
**Where we execute your actions**
I/O Runtime runs in Azure in multiple regions. We deploy your code in all regions and execute it in the closest region to the caller (latency-based routing). You can't restrict the execution to a specific region only.

You can find more information about the regions and how you can check where your actions are being executed here - [Multiple Regions](../guides/reference/multiple_regions.md).

## System Limits
**Which limits are imposed onto actions?**  
All available limits (and the default values) are listed here: [System Settings](../guides/using/system_settings.md). Notable limits are the timeout for functions and the maximum payload that can get posted to a function.

## Developer Support
You can use the [Adobe I/O Runtime Forums](https://forums.adobe.com/community/adobe-io/adobe-io-runtime) for developer support related questions. 

