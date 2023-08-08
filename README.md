# Vality Webhooks Events API Specification

## Working on specification
### Install

1. Install [Node JS](https://nodejs.org/)
2. Clone repo and `cd`
    + Run `npm install`

### Usage

1. Run `npm start`
2. Checkout console output to see where local server is started. You can use all [links](#links) (except `preview`) by replacing https://github.com/vality/swag-webhook-events.git/ with url from the message: `Server started <url>`
3. Make changes using your favorite editor or `swagger-editor` (look for URL in console output)
4. All changes are immediately propagated to your local server, moreover all documentation pages will be automagically refreshed in a browser after each change
**TIP:** you can open `swagger-editor`, documentation and `swagger-ui` in parallel
5. Once you finish with the changes you can run tests using: `npm test`
6. Share you changes with the rest of the world by pushing to GitHub :smile:

### Generate java-client code

1. Install swagger-codegen with brew `brew install swagger-codegen`
2. Run `npm start`
3. Run `npm run build`
4. Use this command 
`swagger-codegen generate -i web_deploy/swagger.json -l java -o ./java --api-package "com.rbkmoney.swag_webhook_events" --artifact-id "swag-webhook-events" --artifact-version "1.0.8-SNAPSHOT" --group-id "com.rbkmoney" --model-package "com.rbkmoney.swag_webhook_events" --library resttemplate --additional-properties dateLibrary=java8`
