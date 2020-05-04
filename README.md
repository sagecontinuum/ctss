# Cloud Training Software Stack (CTSS)

#### Lead: [Wolfgang Gerlach](mailto:wolfgang@uchicago.edu)

### Overview:

Sage nodes will collect data that can be used for building machine learning models. Scientists and students need a standardized software environment for constructing models that can subsequently be tested and transferred to edge nodes and scheduled for execution. CTSS will provide interfaces (API and tools) and documentation with end-to-end examples for users to allow them to build and bundle the components necessary to test on a Virtual Waggle and then Real Waggle.
### Requirements:

CTSS will be available as a downloadable software environment as well as a cloud-hosted service. It needs to support NVIDIA platforms and x86 systems. CTSS will also have documented links to training data.  The cloud service will use token-based authentication (e.g. OAuth2) to access training. Initial version will be hosted at SDSC and Chameleon.

### Use Cases:
#### User Getting Started:
* Get account and log into Chameleon or an SDSC machine
* Find documentation on how to train and build sage models
#### Train an ML model for deployment:
* Use Chameleon, SDSC machine, or local laptop with CTSS downloaded and installed
* Find Sage training data sets and sample Sage ML codes (smoke detector)
* Run training code, build new Edge Model from scratch.
* Package model for execution on Virtual Waggle
#### Test Edge Model on Virtual Waggle:
* Launch VW
* Transfer and run model with fixed inputs from training batch
* Check that Waggle Plugins sent correct data to the Test-and-Development Beehive
#### Test Edge Model on Real Waggle:
* Via Chameleon scheduler, request exclusive access to a Waggle Node
* Launch Edge Model onto Real Waggle
* Run model with fixed inputs from the training batch
* Collect performance and correctness statistics, saved to database
* Upload test Edge Model into ECR, along with performance data

### Milestones:
* Publish CTSS Design Document.
* Make initial prototype available to Sage team on Chameleon.
* Demonstrate continuous integration on Chameleon and SDSC nodes.
* Release CTSS V1.0 with tutorials and examples.
