# View environment data<a name="ag-env-view"></a>

You can view environment detail data using either the console or the AWS CLI\.

You can view lists of environments with details and individual environments with detail data by using the [AWS Proton console](https://console.aws.amazon.com/proton/)\.

1. To view a list of your environments, choose **Environments** in the navigation pane\.

1. To view detail data, choose the name of an environment\.

   View your environment detail data\.

You can also use the AWS CLI for AWS Proton by using the get or list operations as shown in the following example command and response\. You can get or list environments\.

Command:

```
aws proton get-environment --name "MySimpleEnv"
```

Response:

```
{
    "environment": {
        "arn": "arn:aws:proton:region-id:123456789012:environment/MySimpleEnv",
        "createdAt": "2020-11-11T23:03:05.405000+00:00",
        "deploymentStatus": "SUCCEEDED",
        "lastDeploymentAttemptedAt": "2020-11-11T23:03:05.405000+00:00",
        "lastDeploymentSucceededAt": "2020-11-11T23:03:05.405000+00:00",
        "name": "MySimpleEnv",
        "protonServiceRoleArn": "arn:aws:iam::123456789012:role/ProtonServiceRole",
        "spec": "proton: EnvironmentSpec\nspec:\n  my_sample_input: \"the first\"\n  my_other_sample_input: \"the second\"\n",
        "templateMajorVersion": "1",
        "templateMinorVersion": "0"
    }
}
```