- 👋 Hi, I’m @abinandan
- 👀 I’m interested in Test Automation, JavaScript,
- 🌱 I’m currently learning TypeScript
- 💞️ I’m looking to collaborate on UIAutomation stuff
- 📫 Reach me @ abinandan1989@gmail.com

<!---
abinandan-qa/abinandan-qa is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->

# PeopleData E2E Testing Framework - Events 2.0

Test Automation framework built using NodeJS tech stack [cucumber.js, supertest.js, chai.js] designed for adding Events V2 E2E Tests.

## Background

Events Adapter is an application which processes data from WorkDay and publishes events to downstreams [Events V2].This framework was refactored primarily to support E2E testing of this application. This framework can be be extended to add API and Serving layer tests.

### Prerequisites

Node JS 14.x.x and above
VSCode IDE (preferred)

#### Environmental Variables

1.WORKDAY_API_PRIVATE_KEY<br />
2.WORKDAY_API_CLIENT_ID<br />
3.WORKDAY_API_USERNAME<br />
4.WORKDAY_API_AUDIENCE<br />
5.WORKDAY_API_JWT_EXPIRY_TIME<br />
6.WORKDAY_API_SIGN_ALGORITHM<br />
7.GCP_PROJECT<br />
8.baseUrl<br />
9.tokenUrl<br />
10.staffingAPIUrl<br />
11.recruitingAPIurl<br />
12.compensationAPIurl<br />
13.integrationAPIurl<br />
14.datastoreKind<br />
15.projectID<br />
16.locationID<br />
17.testRunEnvironment<br />
18.GOOGLE_APPLICATION_CREDENTIALS(Note: The value should be the path of the service account file in your local)<br />

Note:
Please refer to vault => Techops-PeopleData-QA => wd-sbx-exports

### Setting up in your local

1.Clone this repository,
2.Export the above environmental variables
3.Navigate to the parent directory
4.Run npm install

## Running the tests

To run all e2e tests 
```
 ./node_modules/.bin/cucumber-js ./features/eventsV2/

```

To run specific e2e test
```
 npm run <script-name>

 e.g. npm run hire-v2-e2e-test [Please refer to package.json]

```
