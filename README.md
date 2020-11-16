# chaos-ssm-documents
A collection of AWS SSM Documents to perform FMEA (Failure Mode Effect Analysis)

Heavily influenced by [Adrian Hornsby](https://github.com/adhorn/chaos-ssm-documents).

### How to execute

Each of the executable items is an SSM document.
To use them they need to be uploaded to an AWS account using the following commands.

Using the CLI:

```aws ssm create-document --content file://instance-stop.yml --name "instance-stop" --document-type "Command" --document-format YAML```

To update the document:

```aws ssm update-document --content file://instance-stop.yml --name "instance-stop" --document-version '$LATEST'```


