The previous policy is wrong because it allows all access to objects in the S3 resource without least privilege.
I modified the Action and Resources permissions for wildcats to allow read-only access to objects, ensuring they have the least privilege necessary for the resources they can access.
These changes matter because  leaked credentials can be used to run up expensive resources.
Least privilege was applied to allow "s3:GetObject" on a specific bucket ARN. This indicates the permitted actions.
