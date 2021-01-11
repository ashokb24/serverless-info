# serverless-info

1) Install node
2) npm package comes along with the installation of Node
3) Install the serverless framework using the command --> npm install -g serverless
4) While installing the serverless framework on my Mac, i got the persmission issue. The work around I have found was to install it locally as suggested in this portal. ( https://forum.serverless.com/t/solved-serverless-cli-install-failure-on-macos/3639/4 )
5) If you have experienced persmission issue and solved it using the above post, create a alias sls in ur bash_profile as alias sls = "/Users/<useraccountname>/<local_folder_name>/node_modules/.bin/serverless"
6) Next step is to create a aws IAM User with relevant access to AWS resources. To keep it simple, I have created a IAM user with Administrative Access. Downloaded the Access key ID,Secret access key pair. 
7) Once you have dowloaded the Key pair from ur AWS account, its time to introduce your AWS account to Serverless framework. This can be done using the below command.
	sls config credentials --provider aws --key <KEY_ID> --secret <SECRET>
