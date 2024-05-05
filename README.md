# AWS-Serverless-Website
Building a serverless web application using aws services 
<h1>Application Architecture</h1>
<p>The application architecture uses AWS Lambda, Amazon API Gateway, Amazon DynamoDB, Amazon Cognito, and AWS Amplify Console. Amplify Console provides continuous deployment and hosting of the static web resources including HTML, CSS, JavaScript, and image files which are loaded in the user's browser.Also, Amplify provides a good UI to make simple web applications as an absolute beginner in AWS. JavaScript executed in the browser sends and receives data from a public backend API built using Lambda which is then connected to API Gateway. Amazon Cognito provides user management and authentication functions to secure the backend API. Finally, DynamoDB provides a persistence layer where data can be stored by the API's Lambda function.</p>
<br>
![Serverless_Architecture d930970c77b382db6e0395198aacccd8a27fefb7](https://github.com/yashdeored/AWS-Serverless-Website/assets/152061059/30de3828-4c3a-4dce-a696-8e713f5bc882)
</br>
<ul>
  <ol><h1>AWS Amplify</h1> hosts static web resources including HTML, CSS, JavaScript, and image files which are loaded in the user's browser.</ol>
  <ol><h1>Amazon Cognito</h1> provides user management and authentication functions to secure the backend API.</ol>
  <ol><h1>Amazon DynamoDB</h1> provides a persistence layer where data can be stored by the API's Lambda function.</ol>
  <ol><h1>Rest API</h1> JavaScript executed in the browser sends and receives data from a public backend API built using Lambda and API Gateway.</ol>
</ul>
<h1>Prerequisites</h1>
<p>To complete this tutorial, you will need an AWS account, <a href="https://docs.aws.amazon.com/cli/latest/userguide/getting-started-install.html">AWS CLI</a> installed, an account with <a href="https://www.arcgis.com/sharing/oauth2/authorize?client_id=arcgisonline&response_type=code&state=%7B%22portalUrl%22%3A%22https%3A%2F%2Fwww.arcgis.com%22%2C%22uid%22%3A%22RdbAUp2qODs-VliUiBqh2R2IOJi-ccUQXqgameGfiks%22%2C%22useLandingPage%22%3Atrue%2C%22clientId%22%3A%22arcgisonline%22%7D&expiration=20160&locale=en-gb&redirect_uri=https%3A%2F%2Fwww.arcgis.com%2Fhome%2Faccountswitcher-callback.html&force_login=true&redirectToUserOrgUrl=true&code_challenge=h2jXxZEBaJnnNyyr1J8tGKZZ0VQMr1zHa9ycMATy57Y&code_challenge_method=S256&display=default&hideCancel=true&showSignupOption=true&canHandleCrossOrgSignIn=true&signuptype=esri&allow_verification=true">ArcGIS</a> to add mapping to your app, a text editor, and a web browser. If you don't already have an AWS account, you can follow the Setting Up Your AWS Environment getting started guide for a quick overview.</p>
<h1>Cost to complete</h1>
<p>Each service used in this architecture is eligible for the AWS Free Tier. If you are outside the usage limits of the Free Tier, completing this tutorial will cost you less than $0.25*.</p>
<h1>AWS Services used</h1>
<ul>
  <li>An AWS account**</li>
  <li>AWS CLI</li>
  <li>An ArcGIS account to add mapping to your app</li>
  <li>A text editor</li>
  <li>Recommended browser: The latest version of Chrome</li>
  <li>AWS Lambda</li>
  <li>Amazon API Gateway</li>
  <li>AWS Amplify</li>
  <li>Amazon DynamoDB</li>
  <li>Amazon Cognito</li>
</ul>
