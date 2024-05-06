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
      <h2>Create a git repositry: Using GitHub </h2>For this project there are two options either to use AWS CodeCommit or to use GitHub to store the project repo.
    </li>
      <li>Creating an IAM user: Go to IAM </li>
    <li>Configure your AWS CLI on your local machine. For this we will be using VS Code. Go to your **Terminal** and paste the follwoing command: </li>
  </ul>
  </li>
</ol>
