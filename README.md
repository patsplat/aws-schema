# AWSchema

AWSchema decorates the AWS PHP SDK with useful methods.

AWS applications often involve a wider collection of services than what is supported by CloudFormation alone.  The initial focus is to add "createENTITYIfNotExists" and "ddeleteENTITYIfExists" methods.  Pull requests for any other functionality which improves the maintenance and migration of AWS clusters will be entertained.


```php
require 'vendor/autoload.php';

use patsplat\awschema\AWSchema;

# same signature as Aws::factory
$aws = new AWSchema(array(
    'profile' => 'my_profile',
    'region'  => 'us-east-1',
));
```

## Supported Services

Not yet.

## TODO (aka Unsupported Services)

### AutoScaling

* (AutoScalingGroup)[http://docs.aws.amazon.com/aws-sdk-php/v2/api/class-Aws.AutoScaling.AutoScalingClient.html#_createAutoScalingGroup]
* (LaunchConfiguration)[http://docs.aws.amazon.com/aws-sdk-php/v2/api/class-Aws.AutoScaling.AutoScalingClient.html#_createLaunchConfiguration]
* (Tags)[http://docs.aws.amazon.com/aws-sdk-php/v2/api/class-Aws.AutoScaling.AutoScalingClient.html#_createOrUpdateTags]

### CloudFormation

* (Stack)[http://docs.aws.amazon.com/aws-sdk-php/v2/api/class-Aws.CloudFormation.CloudFormationClient.html#_createStack]

### CloudFront

* (CannedPolicy)[http://docs.aws.amazon.com/aws-sdk-php/v2/api/class-Aws.CloudFront.CloudFrontClient.html#_createCannedPolicy]
* (CloudFrontOriginAccessIdentity)[http://docs.aws.amazon.com/aws-sdk-php/v2/api/class-Aws.CloudFront.CloudFrontClient.html#_createCloudFrontOriginAccessIdentity]
* (Distribution)[http://docs.aws.amazon.com/aws-sdk-php/v2/api/class-Aws.CloudFront.CloudFrontClient.html#_createDistribution]
* (Invalidation)[http://docs.aws.amazon.com/aws-sdk-php/v2/api/class-Aws.CloudFront.CloudFrontClient.html#_createInvalidation]
* (StreamingDistribution)[http://docs.aws.amazon.com/aws-sdk-php/v2/api/class-Aws.CloudFront.CloudFrontClient.html#_createStreamingDistribution]

### CloudHSM

* (Hapg)[http://docs.aws.amazon.com/aws-sdk-php/v2/api/class-Aws.CloudHsm.CloudHsmClient.html#_createHapg]
* (Hsm)[http://docs.aws.amazon.com/aws-sdk-php/v2/api/class-Aws.CloudHsm.CloudHsmClient.html#_createHsm]
* (LunaClient)[http://docs.aws.amazon.com/aws-sdk-php/v2/api/class-Aws.CloudHsm.CloudHsmClient.html#_createLunaClient]

### CloudSearch

* (Domain)[http://docs.aws.amazon.com/aws-sdk-php/v2/api/class-Aws.CloudSearch.CloudSearchClient.html#_createDomain]

### CloudTrail

* (Trail)[http://docs.aws.amazon.com/aws-sdk-php/v2/api/class-Aws.CloudTrail.CloudTrailClient.html#_createTrail]

### CloudWatchLogs

* (LogGroup)[http://docs.aws.amazon.com/aws-sdk-php/v2/api/class-Aws.CloudWatchLogs.CloudWatchLogsClient.html#_createLogGroup]
* (LogStream)[http://docs.aws.amazon.com/aws-sdk-php/v2/api/class-Aws.CloudWatchLogs.CloudWatchLogsClient.html#_createLogStream]

### CodeDeploy

* (Application)[http://docs.aws.amazon.com/aws-sdk-php/v2/api/class-Aws.CodeDeploy.CodeDeployClient.html#_createApplication]
* (Deployment)[http://docs.aws.amazon.com/aws-sdk-php/v2/api/class-Aws.CodeDeploy.CodeDeployClient.html#_createDeployment]
* (DeploymentConfig)[http://docs.aws.amazon.com/aws-sdk-php/v2/api/class-Aws.CodeDeploy.CodeDeployClient.html#_createDeploymentConfig]
* (DeploymentGroup)[http://docs.aws.amazon.com/aws-sdk-php/v2/api/class-Aws.CodeDeploy.CodeDeployClient.html#_createDeploymentGroup]

