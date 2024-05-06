<p>In the initial phase of this project, we will utilize AWS Amplify for web hosting of static resources for our website. This platform also offers a git-based workflow, facilitating continuous deployment of the website. Subsequently, we will proceed to develop dynamic pages employing JavaScript to invoke remote RESTful APIs constructed with Amazon Lambda, a serverless computing service enabling function creation, in conjunction with Amazon API Gateway for seamless integration of applications or services via APIs.
</p>
<br>
![image](https://github.com/yashdeored/AWS-Serverless-Website/assets/152061059/9dd009e0-bc36-4c00-be9f-311786dd31e9)
</br>
<p>The architecture for this project states that the backend of the website which will consist of HTML, CSS, Javascript will be managed by AWS Amplify. Users will then access this website through Public URL hosted by AWS Amplify. If you have your own domain name then you can link it with the service.
</p>
<ol><img width="1437" alt="Screenshot 2024-05-06 at 3 07 29 PM" src="https://github.com/yashdeored/AWS-Serverless-Website/assets/152061059/c1d950b3-4b58-4f2a-9696-052213d6e91b">

  <li><h2>Select an AWS Region: </h2>You can select any region you are comfortable but for this project we will be using the default region US East (N. Virginia)</li>
  <li>
    <ul>
    <li>
      <h2>Create a git repositry: Using CodeCommit </h2>For this project we will be using AWS CodeCommit
    </li>
      <li>Creating an IAM user: Go to IAM -> Users -> Create User</li>
      <img width="1440" alt="Screenshot 2024-05-06 at 3 19 44 PM" src="https://github.com/yashdeored/AWS-Serverless-Website/assets/152061059/73fdf473-5b8b-4dd9-bdd0-84de765cdf71">
      <li>User Name: ANYTHING YOU LIKE -> Hit Next</li>
      <img width="1440" alt="Screenshot 2024-05-06 at 11 06 38 PM" src="https://github.com/yashdeored/AWS-Serverless-Website/assets/152061059/b418d3c7-4050-4af3-9dfb-57e71d169011">
      <li>Attach Policies Directly --> Select CodeCommitFullAccess --> Hit Next</li>
      <img width="1440" alt="Screenshot 2024-05-06 at 3 28 36 PM" src="https://github.com/yashdeored/AWS-Serverless-Website/assets/152061059/e50d7bcf-3fb7-464b-b18b-19821682e9ec">
      <li>Finally Create User</li>
      <img width="1440" alt="Screenshot 2024-05-06 at 3 31 13 PM" src="https://github.com/yashdeored/AWS-Serverless-Website/assets/152061059/26f9dcdc-42c7-4c05-9c03-e1895cac6e23">
      <li>A message pops up saying User has been created</li>
      <img width="1440" alt="Screenshot 2024-05-06 at 4 20 09 PM" src="https://github.com/yashdeored/AWS-Serverless-Website/assets/152061059/5615a31d-8ca0-4099-9247-0374f51ab0aa">
      <li>Now Login into the AWS Console using that credentials</li>
  </ul>
  </li>
  <li>Configuring Git on Cloud9: </li>
  <ul>
    <li>Go to your Cloud9 Service and setup an environment just like shown in the video: </li>
  </ul>
  <li>Setting up your CodeCommit repository</li>
  <ul>
    <li>
First, create a new CodeCommit repository from within your Cloud9 terminal window:
      
```
aws codecommit create-repository \
  --repository-name wild-rydes
```
Clone the existing (not new) workshop repository from GitHub:
```   
git clone https://github.com/aws-samples/aws-serverless-webapp-workshop.git
```
Change into the workshop repository directory:
```
cd aws-serverless-webapp-workshop
```
Split out the WildRydesVue code into its own branch:
```
sudo yum install git-subtree -y
git subtree split -P resources/code/WildRydesVue -b WildRydesVue
```

Note: You may get the error message git: 'subtree' is not a git command on Cloud9 and Amazon Linux 2. Run sudo yum install git-subtree as a workaround, as this is not installed by default with git in these environments.

Create a new directory for your CodeCommit repo:
```
mkdir ../wild-rydes && cd ../wild-rydes
```
Initialize a new git repository:
```
git init
```
Pull the WildRydesVue branch into your new repo:
```
git pull ../aws-serverless-webapp-workshop WildRydesVue
```
Add your CodeCommit repository as a remote:
```
git remote add origin codecommit://wild-rydes
```
Push the code to your new CodeCommit repository:
```
git push -u origin master
```
Remove the temporary local repository you created in step 2: 
```
rm -rf ../aws-serverless-webapp-workshop</li>
```
  </ul>
</ol>
