<p align="center">
<img src="https://github.com/kura-labs-org/kuralabs_deployment_1/blob/main/Kuralogo.png">
</p>
<h1 align="center">C4_deployment-3<h1>

Demonstrate your ability deploy a fully automated Elastic Beanstalk deployment.

- Create a separate GitHub repository for this application

- Download the files from this repository and upload them to your newly created repository

- Be sure to follow the deployment instructions from this repository

- Document your progress in a .md file in your repository. Also, document any issues you may run into and what you did to fix them.

- Make sure your documentation includes these sections:

  - Purpose
  - Issues
  - Steps
  - System Diagram
  - Optimization (How would make this deployment more efficient)

- Lastly, save your documentation and diagram into your repository. Submit your repository link to the LMS

## Deployment instructions Link:

- Link to instructions: https://github.com/kura-labs-org/c4_deployment-3/blob/main/Deployment-instructions.md

<p align="center">
<img src="https://github.com/kura-labs-org/kuralabs_deployment_1/blob/main/Kuralogo.png">
</p>

## Deployment Instructions:

1. Create your own Jenkins Server and install the following on the server:
   - Install "python3.10-venv", "python-pip", "unzip"
2. Create a multibranch pipeline and run the build for the application
   - You'll see an option called branch sources. Choose GitHub and enter your GitHub link and credentials.
3. Follow the install [AWS EB CLI](https://scribehow.com/shared/How_to_install_AWS_EB_CLI__J6eBRB9FQl2fGenfUVemlA) instructions
4. Then, add this stage to your Jenkins file and rerun your build: `stage ('Deploy') {
steps {
sh '/var/lib/jenkins/.local/bin/eb deploy'
}
}
`
5. **IF** your application redeployed successfully, what did you notice?
6. Configure a [Webhook](https://scribehow.com/shared/Setting_up_a_GitHub_webhook_for_Jenkins_deployment__OCRQGNvARfWF4clyeFcsGQ)
7. **BONUS:** Once you've configured your webhook, change the background or some text in the application. **HINT** Look into the HTML or CSS file and ask chatGPT for help
8. Did the application redeploy?
