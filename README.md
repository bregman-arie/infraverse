<p align="center"><img src="images/infraverse.png"/></p>

The most ambitious crossover in history since the MCU.
An educational repository regarding the different platforms and projects in the infrastructure world.

Disclaimer: the project in some parts is opininated

- [Cloud](#cloud)
  - [Services](#services)
- [CI/CD](#cicd)
  - [CI/CD - Platforms](#cicd---platforms)
  - [CI/CD - Configuration](#cicd---configuration)
- [Configuration Management](#configuration-management)
- [Dashboards](#dashboards)
- [Provisioning](#provisioning)
- [Monitoring](#monitoring)
- [More Infra related projects](#more-infra-related-projects)
  - [Contribute](#contribute)
  - [License](#license)


## Cloud 

### Services
<!-- ALL-TOPICS-LIST:START -->
<!-- prettier-ignore-start -->
<!-- markdownlint-disable -->
<center>
<table>
  <tr>
    <td align="center"><b></b></td>
    <td align="center"><a href="#git"><img src="images/aws.png" width="80px;" height="75px;"/><br /><b>AWS</b></a></td>
    <td align="center"><a href="#git"><img src="images/azure.png" width="80px;" height="75px;"/><br /><b>Azure</b></a></td>
    <td align="center"><a href="#ansible"><img src="images/googlecloud.png" width="75px;" height="75px;"/><br /><b>GCP</b></a></td>
    <td align="center"><a href="#openstack"><img src="images/openstack.png" width="80x;" height="75px;"/><br /><b>OpenStack</b></a></td>
    <td align="center"><b>Open Source Alternatives or Solutions</b></a></td>

  </tr>
  <tr>
    <td align="center">Compute<b></b></td>
    <td align="center"><a href="#ec2"><img src="images/ec2.png" width="80px;" height="75px;"/><br /><b>EC2</b></a></td>
    <td align="center"><a href="#virtual-machines"><img src="images/azure/virtual_machine.svg" width="75px;" height="75px;"/><br /><b>Virtual Machine</b></a></td>
    <td align="center"><a href="#compute-engine"><img src="images/gcp_compute_engine.png" width="120px;" height="75px;"/><br /><b>Compute Engine</b></a></td>
    <td align="center"><a href="#nova"><img src="images/openstack_nova.png" width="75px;" height="75px;"/><br /><b>Nova</b></a></td>
    <td align="center"><a href="#ovirt"><img src="images/ovirt.png" width="75px;" height="75px;"/><br /><b>oVirt</b></a></td>
  </tr>
    <tr>
    <td align="center">Network<b></b></td>
    <td align="center"><a href="#ec2"><img src="images/aws/vpc.png" width="80px;" height="75px;"/><br /><b>VPC</b></a></td>
    <td align="center"><a href="#virtual-network"><img src="images/azure/virtual_network.png" width="75px;" height="75px;"/><br /><b>Virtual Network</b></a></td>
    <td align="center"><a href="#compute-engine"><img src="images/gcp/vpc.png" width="90px;" height="75px;"/><br /><b>VPC</b></a></td>
    <td align="center"><a href="#neutron"><img src="images/openstack/neutron.png" width="75px;" height="75px;"/><br /><b>Neutron</b></a></td>
  </tr>
    <tr>
    <td align="center">Object Storage<b></b></td>
    <td align="center"><a href="#ec2"><img src="images/aws/s3.png" width="80px;" height="75px;"/><br /><b>s3</b></a></td>
    <td align="center"><a href="#virtual-machines"><img src="images/azure/blob_storage.png" width="75px;" height="75px;"/><br /><b>Blob Storage</b></a></td>
    <td align="center"><a href="#compute-engine"><img src="images/gcp/cloud_storage.png" width="90px;" height="75px;"/><br /><b>Cloud Storage</b></a></td>
    <td align="center"><a href="#neutron"><img src="images/openstack/swift.png" width="75px;" height="75px;"/><br /><b>Swift</b></a></td>
  </tr>
    <tr>
    <td align="center">Block Storage<b></b></td>
    <td align="center"><a href="#ec2"><img src="images/aws/ebs.png" width="80px;" height="75px;"/><br /><b>EBS</b></a></td>
    <td align="center"><a href="#disk-storage"><img src="images/azure/disk_storage.svg" width="75px;" height="75px;"/><br /><b>Disk Storage</b></a></td>
    <td align="center"><a href="#compute-engine"><img src="images/gcp/persistent_disk.png" width="90px;" height="75px;"/><br /><b>Persistent Disk</b></a></td>
    <td align="center"><a href="#neutron"><img src="images/openstack/cinder.png" width="75px;" height="75px;"/><br /><b>Cinder</b></a></td>
  </tr>
    <tr>
    <td align="center">Image<b></b></td>
    <td align="center"><a href="#ec2"><img src="images/aws/ami.png" width="80px;" height="75px;"/><br /><b>AMI</b></a></td>
    <td align="center"><a href="#virtual-machines"><img src="images/azure/images.svg" width="75px;" height="75px;"/><br /><b>Images</b></a></td>
    <td align="center"><a href="#compute-engine"></br><br /></br><b>Images</b></a></td>
    <td align="center"><a href="#neutron"><img src="images/openstack/glance.png" width="75px;" height="75px;"/><br /><b>Glance</b></a></td>
  </tr>
      <tr>
    <td align="center">Identity<b></b></td>
    <td align="center"><a href="#ec2"><img src="images/aws/iam.svg" width="80px;" height="75px;"/><br /><b>IAM</b></a></td>
    <td align="center"><a href="#virtual-machines"><img src="images/azure/active_directory.png" width="75px;" height="75px;"/><br /><b>Active Directory</b></a></td>
    <td align="center"><a href="#compute-engine"><img src="images/gcp/identity.png" width="90px;" height="75px;"/><br /><b>Identity</b></a></td>
    <td align="center"><a href="#neutron"><img src="images/openstack/keystone.png" width="75px;" height="75px;"/><br /><b>Keystone</b></a></td>
  </tr>
    <tr>
    <td align="center">Load Balancer<b></b></td>
    <td align="center"><a href="#elastc-load-balancing"><img src="images/aws/elastic_load_balancing.png" width="80px;" height="75px;"/><br /><b>Elastic Load Balancing</b></a></td>
    <td align="center"><a href="#virtual-machines"><img src="images/azure/load_balancer.png" width="150px;" height="75px;"/><br /><b>Load Balancer</b></a></td>
    <td align="center"><a href="#compute-engine"><img src="images/gcp/load_balancing.png" width="90;" height="75px;"/><br /><b>Load Balancing</b></a></td>
    <td align="center"><a href="#neutron"><img src="images/openstack/octavia.png" width="75px;" height="75px;"/><br /><b>Octavia</b></a></td>
    <td align="center"><br /><b>Traefik<br>NGINX<br>HAProxy<br>Seesaw</b></a></td>
  </tr>
  <tr>
    <td align="center">Event/Data Streaming<b></b></td>
    <td align="center"><a href="#kinesis"><img src="images/aws/kinesis.png" width="80px;" height="75px;"/><br /><b>Kinesis</b></a></td>
    <td align="center"><a href="#stream_analytics"><img src="images/azure/stream_analytics.png" width="80px;" height="50px;"/><br /><b>Stream Analytics</b></a></td>
    <td align="center"><a href="#pub_sub"><img src="images/gcp/pub_sub.svg" width="80px;" height="50px;"/><br /><b>Pub/Sub</b></a></td>
    <td align="center"><a><img src="images/sad.png" width="64px;" height="64px;"/><br /><b></b></a></td>
    <td align="center"><a><img src="images/kafka.png" width="64px;" height="64px;"/><br /><b>Kafka</b></a></td>
  </tr>
</table>
</center>
<!-- markdownlint-enable -->
<!-- prettier-ignore-end -->
<!-- ALL-TOPICS-LIST:END -->

<a name="cicd" href="#cicd"></a>
## CI/CD 

<a name="cicdplatforms"></a>

### CI/CD - Platforms
<!-- ALL-TOPICS-LIST:START -->
<!-- prettier-ignore-start -->
<!-- markdownlint-disable -->
<center>
<table>
  <tr>
    <td align="center"><b></b></td>
    <td align="center"><a href="#git"><img src="images/jenkins.png" width="54px;" height="64px;"/><br /><b>Jenkins</b></a></td>
    <td align="center"><a href="#git"><img src="images/gitlab.png" width="55px;" height="55px;"/><br /><b>GitLab CI</b></a></td>
    <td align="center"><a href="#ansible"><img src="images/circleci.png" width="55px;" height="55px;"/><br /><b>CircleCI</b></a></td>
    <td align="center"><a href="#bamboo"><img src="images/bamboo.png" width="202px;" height="55px;"/><br /><b>Bamboo</b></a></td>
     <td align="center"><a href="#oc_pipelines"><img src="images/openshift_pipelines.png" width="64;" height="64px;"/><br /><b>OpenShift Pipelines</b></a></td>
    <td align="center"><a href="#teamcity"><img src="images/team_city.png" width="180px;" height="75px;"/><br /><b>TeamCity</b></a></td>

  </tr>
  <tr>
    <td align="center">OPEN SOURCE<b></b></td>
    <td align="center"><a href="#"><img src="images/yes.png" width="50px;" height="64px;"/><br /><b></b></a></td>
    <td align="center"><a href="#"><img src="images/yes.png" width="50px;" height="64px;"/><br /><b></b></a></td>
    <td align="center"><a href="#"><img src="images/no.png" width="50px;" height="64px;"/><br /><b></b></a></td>
    <td align="center"><a href="#"><img src="images/no.png" width="50px;" height="64px;"/><br /><b></b></a></td>
     <td align="center"><a href="#"><img src="images/yes.png" width="50px;" height="64px;"/><br /><b></b></a></td>
     <td align="center"><a href="#"><img src="images/no.png" width="50px;" height="64px;"/><br /><b></b></a></td>
  </tr>
    <tr>
    <td align="center">Deployment Options<b></b></td>
    <td align="center"><a href="#"><br /><b>Managed service,<br>On-premise</b></a></td>
     <td align="center"><a href="#"><br /><b>Hosted,<br>On-premise</b></a></td>
    <td align="center"><a href="#"><br /><b>Hosted,<br>On-premise</b></a></td>
    <td align="center"><a href="#"><br /><b>Managed service,<br>On-premise</b></a></td>
    <td align="center"><a href="#"><br /><b>Depends on how OpenShift was deployed</b></a></td>
    <td align="center"><a href="#"><br /><b>Managed Service, On-Premise</b></a></td>
  </tr>
    <tr>
    <td align="center">Plugins<b></b></td>
    <td align="center"><a href="#"><img src="images/yes.png" width="50px;" height="64px;"/><br /><b>Over thousand plugins</b></a></td>
    <td align="center"><a href="#"><img src="images/no.png" width="50px;" height="64px;"/><br /><b></b></a></td>
     <td align="center"><a href="#"><img src="images/no.png" width="50px;" height="64px;"/><br /><b></b></a></td>
    <td align="center"><a href="#"><img src="images/yes.png" width="50px;" height="64px;"/><br /><b></b></a></td>
    <td align="center"><a href="#"><img src="images/yes.png" width="50px;" height="64px;"/><br /><b>Tekton Hub</b></a></td>
    <td align="center"><a href="#"><img src="images/yes.png" width="50px;" height="64px;"/><br /><b></b></a></td>
  </tr>
    <tr>
    <td align="center">Pipeline/Job/Task Format<b></b></td>
    <td align="center"><a href="#ec2"><br /><b>Groovy,<br>Pipeline DSL</b></a></td>
    <td align="center"><a href="#ec2"><br /><b>YAML</b></a></td>
    <td align="center"><a href="#ec2"><br /><b>YAML</b></a></td>
    <td align="center"><a href="#ec2"><br /><b>Java TaskType Module definition</b></a></td>
    <td align="center"><a href="#ec2"><br /><b>Kubernetes YAMLs</b></a></td>
    <td align="center"><a href="#ec2"><br /><b>Kotlin DSL</b></a></td>
  </tr>
  </tr>
    <tr>
    <td align="center">Best Use Case (imho)<b></b></td>
    <td align="center"><a href="#ec2"><br /><b>Total Freedom (+ You are not afraid of using Groovy)</b></a></td>
    <td align="center"><a href="#ec2"><br /><b>When your code is already in Gitlab</b></a></td>
    <td align="center"><a href="#ec2"><br /><b>When you just want out-of-the-box working CI/CD</b></a></td>
    <td align="center"><a href="#ec2"><br /><b>No idea</b></a></td>
    <td align="center"><a href="#ec2"><br /><b>You don't want to maintain a CI/CD server and your CI/CD is mainly containers based</b></a></td>
    <td align="center"><a href="#ec2"><br /><b>You want versatile CI/CD but don't care about open source</b></a></td>
  </tr>

</table>
</center>
<!-- markdownlint-enable -->
<!-- prettier-ignore-end -->
<!-- ALL-TOPICS-LIST:END -->

<a name="cicdconfiguration"></a>

### CI/CD - Configuration
<!-- ALL-TOPICS-LIST:START -->
<!-- prettier-ignore-start -->
<!-- markdownlint-disable -->
<center>
<table>
  <tr>
    <td align="center"><b></b></td>
    <td align="center"><a href="#git"><img src="images/jenkins.png" width="74px;" height="74px;"/><br /><b>Jenkins</b></a></td>
    <td align="center"><a href="#git"><img src="images/gitlab.png" width="75px;" height="75px;"/><br /><b>GitLab CI</b></a></td>
    <td align="center"><a href="#ansible"><img src="images/circleci.png" width="75px;" height="75px;"/><br /><b>CircleCI</b></a></td>
    <td align="center"><a href="#openstack"><img src="images/bamboo.png" width="180px;" height="75px;"/><br /><b>Bamboo</b></a></td>

  </tr>
  <tr>
    <td align="center">Set Node/Worker/Runner<b></b></td>
    <td align="center"><a href="cicd/jenkins/node.md">Slave<br /><b></b></a></td>
    <td align="center"><a href="cicd/gitlab/node.md">Runner<br /><b></b></a></td>
    <td align="center"><a href="cicd/circleci/node.md">Runner<br /><b></b></a></td>
    <td align="center"><a href="cicd/bamboo/node.md">Agent<br /><b></b></a></td>
  </tr>

</table>
</center>
<!-- markdownlint-enable -->
<!-- prettier-ignore-end -->
<!-- ALL-TOPICS-LIST:END -->

## Configuration Management
<!-- ALL-TOPICS-LIST:START -->
<!-- prettier-ignore-start -->
<!-- markdownlint-disable -->
<center>
<table>
  <tr>
    <td align="center"><b></b></td>
    <td align="center"><a href="#git"><img src="images/ansible.png" width="74px;" height="74px;"/><br /><b>Ansible</b></a></td>
    <td align="center"><a href="#git"><img src="images/puppet.png" width="75px;" height="75px;"/><br /><b>Puppet</b></a></td>
    <td align="center"><a href="#ansible"><img src="images/chef.png" width="75px;" height="75px;"/><br /><b>Chef</b></a></td>


  </tr>
  <tr>
    <td align="center">OPEN SOURCE<b></b></td>
    <td align="center"><a href="#"><img src="images/yes.png" width="50px;" height="64px;"/><br /><b></b></a></td>
    <td align="center"><a href="#"><img src="images/yes.png" width="50px;" height="64px;"/><br /><b></b></a></td>
    <td align="center"><a href="#"><img src="images/yes.png" width="50px;" height="64px;"/><br /><b></b></a></td>
  </tr>
    <tr>
    <td align="center">Agent<br> vs.<br> Agentless<b></b></td>
    <td align="center"><a href="#"><br /><b>Agentless</b></a></td>
    <td align="center"><a href="#"><br /><b>Master-Agent</b></a></td>
    <td align="center"><a href="#"><br /><b>Master-Agent</b></a></td>
  </tr>
    <tr>
    <td align="center">Underlying<br>Programming Language<b></b></td>
    <td align="center"><a href="#"><br /><b>Python</b></a></td>
    <td align="center"><a href="#"><br /><b>Ruby</b></a></td>
    <td align="center"><a href="#"><br /><b>Ruby</b></a></td>
  </tr>
  <tr>
    <td align="center">Push vs. Pull<b></b></td>
    <td align="center"><a href="#"><br /><b>Both supported.<br>Push is the default</b></a></td>
    <td align="center"><a href="#"><br /><b>Both supported.<br>Pull is the default</b></a></td>
    <td align="center"><a href="#"><br /><b>Pull</b></a></td>
  </tr>

</table>
</center>
<!-- markdownlint-enable -->
<!-- prettier-ignore-end -->
<!-- ALL-TOPICS-LIST:END -->

## Dashboards
<!-- ALL-TOPICS-LIST:START -->
<!-- prettier-ignore-start -->
<!-- markdownlint-disable -->
<center>
<table>
  <tr>
    <td align="center"><b></b></td>
    <td align="center"><a href="#git"><img src="images/kibana.png" width="74px;" height="74px;"/><br /><b>Kibana</b></a></td>
    <td align="center"><a href="#git"><img src="images/grafana.png" width="75px;" height="75px;"/><br /><b>Grafana</b></a></td>
    <td align="center"><a href="#ansible"><img src="images/reportportal.png" width="75px;" height="75px;"/><br /><b>ReportPortal</b></a></td>


  </tr>
  <tr>
    <td align="center">OPEN SOURCE<b></b></td>
    <td align="center"><a href="#"><img src="images/yes.png" width="50px;" height="64px;"/><br /><b></b></a></td>
    <td align="center"><a href="#"><img src="images/yes.png" width="50px;" height="64px;"/><br /><b></b></a></td>
    <td align="center"><a href="#"><img src="images/yes.png" width="50px;" height="64px;"/><br /><b></b></a></td>
  </tr>
    <tr>
    <td align="center">Querying<b></b></td>
    <td align="center"><a href="#"><img src="images/yes.png" width="50px;" height="64px;"/><br /><b>Lucene and KQL</b></a></td>
    <td align="center"><a href="#"><img src="images/yes.png" width="50px;" height="64px;"/><br /><b>Based on the<br>data source</b></a></td>
    <td align="center"><a href="#"><img src="images/no.png" width="50px;" height="64px;"/><br /><b></b></a></td>
  </tr>
    <tr>
    <td align="center">Supports multiple<br>data sources<b></b></td>
    <td align="center"><a href="#"><img src="images/no.png" width="50px;" height="64px;"/><br /><b>Only Elasticsearch</b></a></td>
    <td align="center"><a href="#"><img src="images/yes.png" width="50px;" height="64px;"/><br /><b></b></a></td>
    <td align="center"><a href="#"><img src="images/yes.png" width="50px;" height="64px;"/><br /><b></b></a></td>
  </tr>
      <tr>
    <td align="center">Visualizations<b></b></td>
    <td align="center"><a href="#"><br /><b>Pie charts, Line charts<br> Data tables, Markdown<br>Geo Maps, Metrics<br>Heat Map</b></a></td>
    <td align="center"><a href="#"><br /><b>Pie charts, Line charts<br> Data tables, Markdown<br>Geo Maps, Metrics<br>Heat Map</b></a></td>
     <td align="center"><a href="#"><br /><b>Pie charts, Line charts<br> Data tables</b></a></td>
  </tr>
  <tr>
    <td align="center">Best suited for<b></b></td>
    <td align="center"><a href="#"><br /><b>Logs Analysis</b></a></td>
    <td align="center"><a href="#"><br /><b>Metrics Analysis</b></a></td>
    <td align="center"><a href="#"><br /><b>Pattern Analysis</b></a></td>
  </tr>

</table>
</center>
<!-- markdownlint-enable -->
<!-- prettier-ignore-end -->
<!-- ALL-TOPICS-LIST:END -->

## Provisioning

Note: Many systems and tools can be used for provisioning (e.g. Ansible). This is focusing on those who were built mainly for this purpose.
<!-- ALL-TOPICS-LIST:START -->
<!-- prettier-ignore-start -->
<!-- markdownlint-disable -->
<center>
<table>
  <tr>
    <td align="center"><b></b></td>
    <td align="center"><a href="#git"><img src="images/terraform.png" width="74px;" height="74px;"/><br /><b>Terraform</b></a></td>
    <td align="center"><a href="#git"><img src="images/pulumi.svg" width="75px;" height="75px;"/><br /><b>Pulumi</b></a></td>
    <td align="center"><a href="#ansible"><img src="images/cloudformation.png" width="75px;" height="75px;"/><br /><b>CloudFormation</b></a></td>


  </tr>
  <tr>
    <td align="center">OPEN SOURCE<b></b></td>
    <td align="center"><a href="#"><img src="images/yes.png" width="50px;" height="64px;"/><br /><b></b></a></td>
    <td align="center"><a href="#"><img src="images/yes.png" width="50px;" height="64px;"/><br /><b></b></a></td>
    <td align="center"><a href="#"><img src="images/no.png" width="50px;" height="64px;"/><br /><b></b></a></td>
  </tr>
    <tr>
    <td align="center">Language<b></b></td>
    <td align="center">DSL (HCL)</td>
    <td align="center">Python, C#, JavaScript,<br> Go and TypeScript </td>
    <td align="center">JSON or YAML</td>
  </tr>
    <tr>
    <td align="center">Cloud Agnostic<b></b></td>
    <td align="center"><a href="#"><img src="images/yes.png" width="50px;" height="64px;"/><br /><b></b></a></td>
    <td align="center"><a href="#"><img src="images/yes.png" width="50px;" height="64px;"/><br /><b></b></a></td>
    <td align="center"><a href="#"><img src="images/no.png" width="50px;" height="64px;"/><br /><b></b></a></td>
  </tr>
      <tr>
    <td align="center">Written in<b></b></td>
    <td align="center">Go</td>
    <td align="center">Go, Typescript and Python</td>
    <td align="center">?</td>
  </tr>
  <tr>
    <td align="center">Main Advantage<b></b></td>
    <td align="center">Large community and<br>many supported providers</td>
    <td align="center">Supports multiple languages</td>
    <td align="center">AWS services coverage<br>and rolling updates management</td>
  </tr>

</table>
</center>
<!-- markdownlint-enable -->
<!-- prettier-ignore-end -->
<!-- ALL-TOPICS-LIST:END -->

## Monitoring

<!-- ALL-TOPICS-LIST:START -->
<!-- prettier-ignore-start -->
<!-- markdownlint-disable -->
<center>
<table>
  <tr>
    <td align="center"><b></b></td>
    <td align="center"><a href="#git"><img src="images/prometheus.png" width="74px;" height="74px;"/><br /><b>Prometheus</b></a></td>
    <td align="center"><a href="#git"><img src="images/graphite.png" width="75px;" height="75px;"/><br /><b>Graphite</b></a></td>
    <td align="center"><a href="#ansible"><img src="images/nagios.png" width="75px;" height="75px;"/><br /><b>Nagios</b></a></td>


  </tr>
  </tr>
    <tr>
    <td align="center">Main Purpose<b></b></td>
    <td align="center">Time series DB and monitoring system</td>
    <td align="center">Time Series DB and Graph rendering of the data</td>
    <td align="center">Monitoring system focused specifically on servers and network</td>
  </tr>
  <tr>
    <td align="center">OPEN SOURCE<b></b></td>
    <td align="center"><a href="#"><img src="images/yes.png" width="50px;" height="64px;"/><br /><b></b></a></td>
    <td align="center"><a href="#"><img src="images/yes.png" width="50px;" height="64px;"/><br /><b></b></a></td>
    <td align="center"><a href="#"><img src="images/yes.png" width="50px;" height="64px;"/><br /><b></b></a></td>
  </tr>
    <tr>
    <td align="center">Written in<b></b></td>
    <td align="center">Go</td>
    <td align="center">Python</td>
    <td align="center">C</td>
  </tr>
    <tr>
    <td align="center">API<b></b></td>
    <td align="center">RESTful HTTP and JSON<b></b></td>
    <td align="center">HTTP API Sockets</td>
    <td align="center">RESTful HTTP via Addon installation</td>
  </tr>
      <tr>
    <td align="center">Written in<b></b></td>
    <td align="center">Go</td>
    <td align="center">Go, Typescript and Python</td>
    <td align="center">?</td>
  </tr>
  <tr>
    <td align="center">Data Gathering<b></b></td>
    <td align="center">Pull (Exporters)</td>
    <td align="center">Push</td>
    <td align="center">Pull (Agents)</td>
  </tr>
  <tr>
    <td align="center">Alerts<b></b></td>
    <td align="center"><a href="#"><img src="images/yes.png" width="50px;" height="64px;"/><br /><b></b></a></td>
    <td align="center"><a href="#"><img src="images/no.png" width="50px;" height="64px;"/><br /><b></b></a></td>
    <td align="center"><a href="#"><img src="images/yes.png" width="50px;" height="64px;"/><br /><b></b></a></td>
  </tr>
  <tr>
    <td align="center">Queries<b></b></td>
    <td align="center"><a href="#"><img src="images/yes.png" width="50px;" height="64px;"/><br /><b></b></a></td>
    <td align="center"><a href="#"><img src="images/no.png" width="50px;" height="64px;"/><br /><b></b></a></td>
    <td align="center"><a href="#"><img src="images/yes.png" width="50px;" height="64px;"/><br /><b></b></a></td>
  </tr>
  <tr>
    <td align="center">Visualizations<b></b></td>
    <td align="center"><a href="#"><img src="images/yes.png" width="50px;" height="64px;"/><br /><b>Users mainly use Grafana for dashboards</b></a></td>
    <td align="center"><a href="#"><img src="images/yes.png" width="50px;" height="64px;"/><br /><b></b></a></td>
    <td align="center"><a href="#"><img src="images/yes.png" width="50px;" height="64px;"/><br /><b></b></a></td>
  </tr>

</table>
</center>
<!-- markdownlint-enable -->
<!-- prettier-ignore-end -->
<!-- ALL-TOPICS-LIST:END -->


## More Infra related projects

<p align="center"><a href="https://github.com/bregman-arie/howtheydevops"><img src="images/how_they_devops.png"/></a></p>
<p align="center"><a href="https://github.com/bregman-arie/devops-resources"><img src="images/devops_resources.png"/></a></p>
<p align="center"><a href="https://github.com/bregman-arie/devops-exercises"><img src="images/devops_exercises.png"/></a></p>

### Contribute
Contributions welcome! Read the [contribution guidelines](contributing.md) first.

### License
[![CC0](https://mirrors.creativecommons.org/presskit/buttons/88x31/svg/cc-zero.svg)](https://creativecommons.org/publicdomain/zero/1.0)
