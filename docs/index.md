# Get Started with Open Banking Accelerator

Welcome to our product page of Open Banking Accelerator. Open Banking Accelerator provides a set of tools and resources which you can use to start your open banking journey and achieve the open banking compliant status fast. Our Aim is to accelerate your Open banking journey with a blinding speed.

## How do we do it?

We provide a set of tools out of the box which you can plug and play to get started quickly. The tools are as follows -

**Backstage Scaffolder** - with the power of backstage scaffolder, you can create your initial code respositories in your remote organization repositories very quickly with all the starter code already written. You just have to integrate with your backend services. You can choose to scaffold the following templates from the create menu on the left hand side of the Backstage page -

1. ***OBA-Spec_service*** - This provides a adapter service which accepts open banking APIs and returns the responses in the desired format. The services should call the bank's internal APIs in Core banking systems to get the appropriate response. The conversion will be different for the each bank.
2. ***OBA-Kong_gateway*** - Kong is a popular gateway service. All the APIs reaching OBA-Spec_service pass through it.
3. ***AWS API Gateway Terraform Template*** - The terraform scripts to automate the creation of an API Gateway in AWS for various open banking microservices like Accounts and transactions, Confirmation of funds, Payment initiation, Events and Notifications. These scripts will generate all the required resources and proxy any incoming API request to the required server. Our OBA microservices run in different ports, and this gateway creates a uniform endpoint for accessing these services.
4. ***Open Banking project*** - In order to show the capability of our OBA Translation layer, we are using the open source Open Banking Project(OBP) as our core legacy bank system. OBA internally makes API calls to OBP, which has a fully functional banking environment enabled for us. We can get accounts, check balances and make transactions using the OBP APIs. It returns the response in its own format, which later is converted to an Open Bankig API Request and response structure by our translation layer Open Banking Accelerator, thereby highlightinng the real purpose of OBA's integration with legacy banks.


### OBA Architecture
![](../images/OBA_Architecture.png)

### Usage of templates
To use any tempalte, follow the following steps:

1. Choose the required template.
2. Fill the required fields in the template form eg: Owner, Name, Description, Access etc.
3. In the Store Path field, provide the Github URL of the repository that will be created while filling the template form.
4. Click on Next Step.
5. Review the details you entered and click create.
6. A new repository will be created in your Github account with the name and description you provided, having some predefined code based on the Template chosen by you.
