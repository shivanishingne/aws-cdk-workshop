# aws-cdk-workshop
Learning AWS CDK


### Prerequisites
- Install CDK toolkit (using npm):
``` 
npm install -g aws-cdk
```
- Check toolkit version:
``` 
cdk --version
```
--- 

### Creating first CDK Project
- After creating a directory, we use cdk init to create a new cdk project:
```
cdk init sample-app --language typescript
```

### Compiling typescript code
- Since TypeScript sources need to be compiled to JavaScript, every time we make a modification to our source files, we would want them to be compiled to .js.

- Open new terminal to start watching for changes:
```
cd cdk-workshop   
```

```
npm run watch
```
- This will start the TypeScript compiler (tsc) in “watch” mode, which will monitor your project directory and will automatically compile any changes to your .ts files to .js.
---
#### Project Structure
> lib/cdk-workshop-stack.ts

..is where your CDK application’s main stack is defined.

> bin/cdk-workshop.ts

..is the entrypoint of the CDK application. It will load the stack class defined in lib/cdk-workshop-stack.ts.

> package.json

..is your npm module manifest.

> cdk.json

..tells the toolkit how to run your app.

> tsconfig.json

.. is your project’s typescript configuration.
---


