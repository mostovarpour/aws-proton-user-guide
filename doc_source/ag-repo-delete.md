# Delete a repository link<a name="ag-repo-delete"></a>

You can delete a repository link by using the console or the AWS CLI\.

**Note**  
Deleting a repository link only removes the registered link that AWS Proton has in your AWS account\. It does not delete any information from your repository\.

------
#### [ AWS Management Console ]

**Delete a repository link using the console\.**

**In the repository detail page\.**

1. In the [AWS Proton console](https://console.aws.amazon.com/proton/), choose **Repositories**\.

1. In the list of repositories, choose the radio button to the left of the repository that you want to delete\.

1. Choose **Delete**\.

1. A modal prompts you to confirm the Delete action\.

1. Follow the instructions and choose **Yes, delete**\.

------
#### [ AWS CLI ]

**Delete a repository link\.**

Run the following command:

```
$ aws proton delete-repository \
    --name myrepos/templates \
    --provider"GITHUB"
```

Response:

```
{
    "repository": {
        "arn": "arn:aws:proton:region-id:123456789012:repository/github:myrepos/templates",
        "name": "myrepos/templates",
        "provider": "GITHUB"
    }
}
```

------